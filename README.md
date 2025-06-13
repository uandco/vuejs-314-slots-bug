# Minimal reproducible example for VueJS 3.5.14+ slots bug

Run `npm install`

Run `vite`


Go to http://localhost:8080
Page displays OK

Change `"vue": "3.5.13"` to `"vue": "3.5.14"` or later

Run `npm install`

Run `vite`

Go to http://localhost:8080

Page doesn't display, throws:

```
uuFaq.vue:5 Uncaught TypeError: item is not a function
    at uuFaq.vue:5:36
    at Proxy._sfc_render (uuFaq.vue:1:1)
```
