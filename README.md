### vnjson.js
<<<<<<< HEAD
>Делаем визуальные новелы на javascript

=======


>>>>>>> origin/master
### Инициализация
```javascript
  vnjs.init({
    scenesDirectory: 'scenes',
    local: 'ru-RU',
    entry: 'start/chapter1'
  });

```

<<<<<<< HEAD





#### Как написать плагин

=======
### Плагины

>>>>>>> origin/master
##### Самовызывающиеся плагины [ autorun ]
```javascript
  vnjs.on(function(){
    console.log('autorun');
  });

```
##### Вызываются из пользовательского скрипта
```javascript
  vnjs.on('alert', function(param, ctx){
    alert(ctx.scene)
  })

```
<<<<<<< HEAD
##### Файловая структура плагина
=======

### Структура сцены *.json
>./scenes/ru-RU/start.json

```json
{
  "labels":{
    "chapter1": [
      {
        "pr": "Привет! Давненько не виделись",
        "left":"prof_norm"
      },
      {
        "al": "Да уж, давненько.",
        "scene": "room_hero",
        "sound": "song1"
      },
      {
        "pr": "Хорош болтать! Погнали в лабараторию"
      },
      {
        "al": "Профессор вы слишком торопитесь. Это еще ни кому не помогало.",
        "scene":"roof"
      },
      {
        "pr": "Алиса не тебе меня поучать!",
        "left":"baka",
        "jump": "start/chapter2"
      }
    ],
    "chapter2": [
      {
        "al": "И как это понимать? Разве мы не должны позаботиться об этих ошибках?",
        "center": "errors",
        "sound": "errors"
      },
      {
        "pr": "Ты так ничему и не научилась..",
        "right": "chapter2"

      }
  ]
  },
  "preload": [
    "/assets/bg.png"
  ],
  "characters": [
    {
      "aliase": "pr",
      "name": "Профессор",
      "color": "green"
    },
    {
      "aliase": "al",
      "name": "Алиса",
      "color": "red"
    },
    {
      "aliase": "ll",
      "name": "Люсиль",
      "color": "grey"
    }
  ]
}


```
####Структура визуальной новеллы
>>>>>>> origin/master

```plane_text
plugins
├── alert
│   ├── index.js
│   ├── package.json
│   └── README.md
├── debug
│   ├── index.js
│   ├── package.json
│   └── README.md

```
<<<<<<< HEAD
#### Библиотеки
Если же вы хотите добавить в зависимость к вашему плагину
библиотеку, то положите файл библиотека в каталог /lib 
=======
>>>>>>> origin/master
