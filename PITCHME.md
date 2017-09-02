### 友達にLINEの通知うざいーわと
### アピールしたい時に

千葉工業大学　

4年 大川晶也(@masamasa9841)

~~LT初めてですので、やさしくしてください~~

---

### LINEの通知数が多い = リア充

![line](./line.png)


LINEの通知数を自作自演して、リア充になろうYO

---

### 通知数を自作自演する為に

[LINEのAPI](https://devdocs.line.me/ja/#push-message)を使いました。

---

### 今回はシェルでAPIを叩きます

``` bash
#! /usr/bin/env bash
curl -X POST \
-H 'Content-Type:application/json' \
-H 'Authorization: Bearer {ENTER_ACCESS_TOKEN}' \
-d '{
    "to": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
    "messages":[
        {
            "type":"text",
            "text":"Hello, world1"
        },
        {
            "type":"text",
            "text":"Hello, world2"
        }
    ]
}' https://api.line.me/v2/bot/message/push
```

---

### 実際にやってみたいと思いまっす

---

### これで今日からリア充だね!

