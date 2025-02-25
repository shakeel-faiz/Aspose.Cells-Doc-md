﻿---
title:  Пользовательские контекстные меню для GridJs
type: docs
weight: 250
url: /ru/net/aspose-cells-gridjs/custommenu/
description: В этой статье описывается, как настроить контекстные меню для GridJ.
keywords: custom menu items, context menu
---
# Пользовательские контекстные меню
У нас есть некоторые встроенные элементы контекстного меню, например, вставка/удаление строки/столбца и т. д.
Однако, если пользователь хочет настроить элементы контекстного меню.
Мы поддерживаем установку пунктов контекстного меню в параметрах загрузки.
Например:
```javascript
        const onMyActionClick1 = (sheet) => {
            console.log('my action clicked1' +  sheet.data.name)
        };
        const onMyActionClick2 = (sheet) => {
            console.log('my action clicked2' + sheet.data.name)
        };
  xs = x_spreadsheet('#gridjs-demo', {
                updateMode: 'server',
                updateUrl: '/GridJs2/UpdateCell',
                showToolbar: true,
                mode: 'edit',
                local: 'en',
                showContextmenu: true,
		//this option is for context menus,we need to set usedefault to false to load custom context menus
                contextMenuItems: {
                    usedefault: false,
                    customItems: [{ 'key': 'key1', 'text': 'c title 11111', 'callback': onMyActionClick1 },
                                  { 'key': 'key2', 'text': 'c title 22222', 'callback': onMyActionClick2 }]
                }
            })
```

Мы поддерживаем указанные ниже JS API для настраиваемых элементов контекстного меню во время выполнения.


- получить пользовательские элементы контекстного меню
```javascript
xs.sheet.getCustomContextMenuItems()
```

- добавить пользовательские пункты контекстного меню
```javascript
xs.sheet.addCustomContextMenuItems(itemsarray)
 // the parameter is:
 itemsarray: the array of custom menu items,the callback function x parameter will be the js variable of xs.sheet
 for example: [{'key':'key4','text':'menu4','callback':(x)=>{console.log('hello4444');}},{'key':'key3','text':'menu3','callback':(x)=>{console.log('hello3333');}}]
```

- удалить пользовательские элементы контекстного меню
```javascript
 xs.sheet.delCustomContextMenuItems(keysarray)()
 // the parameter is:
 keysarray: the array of the keys of the menu items
 for example: ['key4','key3']
```

- вставить пользовательский пункт контекстного меню в указанную позицию
```javascript
xs.sheet.insertCustomContextMenuItem(item,postion)
 // the parameter is:
 item: the custom menu item,the callback function x parameter will be the js variable of xs.sheet
 for example: {'key':'key4','text':'menu4','callback':(x)=>{console.log('hello4444');}} 
 postion:the postion for the inserted item in the items array
```

- обновить пользовательский пункт контекстного меню по ключу
```javascript
xs.sheet.updateCustomContextMenuItem(key,item)
 // the parameter is:
 item: the updated properties that with text or callback
 for example: {'text':'menu updated'}
 key:the key of the menu item
```


- получить пользовательские элементы контекстного меню для изображения/формы
```javascript
xs.sheet.getImageContextMenuItems()
```

- добавить пользовательские элементы контекстного меню для изображения/формы
```javascript
xs.sheet.addImageContextMenuItems(itemsarray)
 // the parameter is:
 itemsarray: the array of custom menu items,the callback function x parameter will be the js variable of xs.sheet
 for example: [{'key':'key4','text':'img operation1','callback':(x)=>{console.log('operation1 on image');}},{'key':'key3','text':'img operation2','callback':(x)=>{console.log('operation2 on image');}}]
```

- удалить пользовательские элементы контекстного меню для изображения/фигуры
```javascript
 xs.sheet.delImageContextMenuItems(keysarray)()
 // the parameter is:
 keysarray: the array of the keys of the menu items
 for example: ['key4','key3']
```

Вы можете найти больше на нашей демонстрационной странице github https://github.com/aspose-cells/Aspose.Cells-for-.NET/blob/master/Examples_GridJs/wwwroot/xspread/index.html.


 
