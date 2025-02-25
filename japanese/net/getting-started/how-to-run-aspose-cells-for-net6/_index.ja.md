﻿---
title: .Net6 で Aspose.Cells を実行する方法
type: docs
description: .Net6 で Aspose.Cells を実行する方法
weight: 138
url: /ja/net/how-to-run-aspose-cells-for-net6/
---
## 概要

.NET6 (またはそれ以降) プラットフォームの場合、以前のプラットフォーム (.netcore31 以前) と比較すると、グラフィック ライブラリに関する重要な違いがあります。
この公式では[Microsoft ドキュメント](https://learn.microsoft.com/en-gb/dotnet/core/compatibility/core-libraries/6.0/system-drawing-common-windows-only).NET6 以降のリリースでは、グラフィック ライブラリ "System.Drawing.Common" は Windows でのみサポートされることを説明し、グラフィック ライブラリを置き換えることを推奨しています。

Apose.Cells 製品については、評価を実施し、グラフィック ライブラリの移行を完了しました。 Microsoft の公式ドキュメントで提案されているように、Windows 以外のシステムでは System.Drawing.Common の代わりに SkiaSharp を使用します。この重要な変更は、.Net6 の Aspose.Cells 22.10.1 以降で有効になることに注意してください。

.netcore31 以前では、互換性と安定性のために、現在も "System.Drawing.Common" グラフィック ライブラリを使用しています。 .netcore31 以前の依存関係は次のとおりです。
- System.Drawing.Common、4.7.0。
- System.Security.Cryptography.Pkcs、5.0.1。
- System.Text.Encoding.CodePages、4.7.0。

## Windows で .Net6 に対して Aspose.Cells を実行します。

まず、VS2022 で .net6 アプリケーションを作成してから、次のインストール オプションを選択できます。

### nuget からインストール

1. NuGet から Aspose.Cells を検索:[Aspose.Cells for .NET NuGet パッケージ](https://www.nuget.org/packages/Aspose.Cells/). 
VS2022 の Nuget パッケージ マネージャーから Aspose.Cells をインストールすることもできます。

2. "SkiaSharp" または "System.Drawing.Common" は、プロジェクトの "ターゲット OS" 構成に依存する .Net6 プラットフォームの Aspose.Cells 22.10.1 以降の依存関係として自動的にインストールされます。
- プロジェクトの「ターゲット OS」を「Windows」に設定します。.Net6 プロジェクトの Windows システムへの依存関係として「System.Drawing.Common」を使用します。この構成では、描画の結果は .netcore31 以前に近くなります。
**![ターゲットOSの設定](TargetOS.png)**
- プロジェクトの「ターゲット OS」を「なし」またはその他のオプションに設定します。.Net6 プロジェクトの Windows システムへの依存関係として「SkiaSharp」を使用します。現在、SkiaSharp は Windows で EMF などの形式をサポートしていないことに注意してください。

### msi または DLL を使用してインストールする

1. [Aspose.Cells.msi または DLL をダウンロード](https://releases.aspose.com/cells/net/)

2. インストール ディレクトリまたは DLL ディレクトリを開き、以下の手順 3 または 4 を選択します。

3. 「net6.0-windows」サブディレクトリを見つけ、その中の Aspose.Cells.dll を .net6 アプリケーションに追加します。次の nuget パッケージを .net6 プロジェクトに手動で追加します。
- System.Drawing.Common、4.7.0。
- System.Security.Cryptography.Pkcs、6.0.1。
- System.Text.Encoding.CodePages、4.7.0。

このようにして、「System.Drawing.Common」を .Net6 プロジェクトの Windows システムへの依存関係として使用します。この構成では、描画の結果は .netcore31 以前に近くなります。

4. 「net6.0」サブディレクトリを見つけ、その中の Aspose.Cells.dll を .net6 アプリケーションに追加します。次の nuget パッケージを .net6 プロジェクトに手動で追加します。
- スキアシャープ、2.88.3。
- System.Security.Cryptography.Pkcs、6.0.1。
- System.Text.Encoding.CodePages、4.7.0。

このようにして、.Net6 プロジェクトの Windows システムへの依存関係として "SkiaSharp" を使用します。現在、SkiaSharp は Windows で EMF などの形式をサポートしていないことに注意してください。

## Linux で .Net6 に対して Aspose.Cells を実行します。

Windows のインストール方法を参照してください。Linux システムでは、グラフィックス ライブラリの依存関係として SkiaSharp のみを選択できます。

Linux で SkiaSharp を適切に使用するには、次の追加操作を行う必要があります。

1. Linux システムで次のコマンドを実行します。
```
apt-get update && apt-get install -y libfontconfig1
```
また
```
apk update && apk add fontconfig 
```

2. nuget パッケージ「SkiaSharp.NativeAssets.Linux 2.88.3」を .net6 プロジェクトに追加します。

3. または、上記の 2 つの手順の代わりに、nuget パッケージ "SkiaSharp.NativeAssets.Linux.NoDependencies 2.88.3" を .net6 プロジェクトに追加することもできます。

### Ubuntu の Dockerfile の例

1. nuget パッケージ "SkiaSharp.NativeAssets.Linux 2.88.3" を .net6 プロジェクトに追加します。

2. 次の Dockerfile を使用します。
{{< highlight "plain" >}}
# Ubuntu 20.04
FROM mcr.microsoft.com/dotnet/runtime:6.0-focal AS base
WORKDIR /app

# add "libfontconfig1" package if using "SkiaSharp.NativeAssets.Linux" in your project
# Or you need to use "SkiaSharp.NativeAssets.Linux.NoDependencies" in your project
RUN apt-get update && apt-get install -y libfontconfig1

# Copy fonts from local to docker
# For example, put a "fonts" folder in your project folder, and put the font files in it,
# then, use the following line:
COPY fonts/ /usr/share/fonts

FROM mcr.microsoft.com/dotnet/sdk:6.0-focal AS build
WORKDIR /src
COPY ["Ubuntu_Docker.csproj", "."]RUN dotnet restore "./Ubuntu_Docker.csproj"
COPY . .
WORKDIR "/src/."
RUN dotnet build "Ubuntu_Docker.csproj" -c Release -o /app/build

FROM build AS publish
RUN dotnet publish "Ubuntu_Docker.csproj" -c Release -o /app/publish

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "Ubuntu_Docker.dll"]{{< /highlight >}}

### Alpine の Dockerfile の例

1. nuget パッケージ "SkiaSharp.NativeAssets.Linux 2.88.3" を .net6 プロジェクトに追加します。

2. 次の Dockerfile を使用します。
{{< highlight "plain" >}}
# Alpine 3.16
FROM mcr.microsoft.com/dotnet/runtime:6.0-alpine3.16 AS base
WORKDIR /app

# add "fontconfig" package if using "SkiaSharp.NativeAssets.Linux" in your project
# Or you need to use "SkiaSharp.NativeAssets.Linux.NoDependencies" in your project
RUN apk update && apk add fontconfig 

# Copy fonts from local to docker
# For example, put a "fonts" folder in your project folder, and put the font files in it,
# then, use the following line:
COPY fonts/ /usr/share/fonts

FROM mcr.microsoft.com/dotnet/sdk:6.0-alpine3.16 AS build
WORKDIR /src
COPY ["Alpine_Docker.csproj", "."]RUN dotnet restore "./Alpine_Docker.csproj"
COPY . .
WORKDIR "/src/."
RUN dotnet build "Alpine_Docker.csproj" -c Release -o /app/build

FROM build AS publish
RUN dotnet publish "Alpine_Docker.csproj" -c Release -o /app/publish

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "Alpine_Docker.dll"]{{< /highlight >}}
