---
title: "DACSC_Basic web 01"
description: "大安電研網頁設計範例程式碼"
published: 2025-11-06
---

# 簡報原始檔  
<a href="https://github.com/peterqgogzq/-/blob/main/dacsc_web/web_html.pdf">下載處</a>  

# 範例程式碼  

## 01  
```html
<!DOCTYPE html>
<html>
  <head>
    <title>This is a title</title>
  </head>
  <body>
    <p>Hello world!</p>
  </body>
</html>
```

<samp>Hello world!</samp>  

## 02  

AI寫出來的狗屁遊戲，就交給你們來改良了  

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>恐怖文字冒險遊戲</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        #output {
            border: 1px solid #ccc;
            padding: 10px;
            min-height: 200px;
            background-color: #f9f9f9;
            margin-bottom: 10px;
        }
        #input {
            width: 100%;
            padding: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>恐怖文字冒險遊戲</h1>
        <div id="output">
            <p>你醒來發現自己在一個陰暗的房間裡，四周一片漆黑。</p>
            <p>你可以在這裡看到一扇鐵門和一扇木門。</p>
        </div>
        <input type="text" id="input" placeholder="請輸入你的行動...">
    </div>

    <script>
        const output = document.getElementById('output');
        const input = document.getElementById('input');

        input.focus();

        input.addEventListener('keydown', function(event) {
            if (event.key === 'Enter') {
                const action = input.value.toLowerCase().trim();
                input.value = '';
                handleAction(action);
            }
        });

        function handleAction(action) {
            const actions = {
                '打開鐵門': function() {
                    output.innerHTML += "<p>你打開了鐵門，突然一陣寒風吹進來，你感到一陣不祥的預感...</p>";
                },
                '打開木門': function() {
                    output.innerHTML += "<p>你打開了木門，裡面是一條陰暗的走廊，你聽到了一些奇怪的聲音...</p>";
                },
                '逃跑': function() {
                    output.innerHTML += "<p>你試圖逃跑，但房間的門突然關上了，你無法離開...</p>";
                },
                '探索房間': function() {
                    output.innerHTML += "<p>你仔細搜索房間，找到了一個看似古老的日記...</p>";
                }
            };

            if (actions[action]) {
                actions[action]();
            } else {
                output.innerHTML += "<p>你的行動無效。</p>";
            }
        }
    </script>
</body>
</html>
```


