# 1f Static Files and Javascript
- Pretty much like css
- create `static/js` and a new file there called `main.js`
``` js title="main.js"
console.log('This is JS from your About page.')
```
- And need to add a script element after the link element in about.html
``` html title="about.html"
<script src="{% static 'js/main.js' %}"></script>
```

