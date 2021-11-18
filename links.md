---
title: Static Links
lang: de
---

## CSS

```html
<link rel="stylesheet" type="text/css" href="URL">
```

- [bootstrap.min.css](node_modules/bootstrap/dist/css/bootstrap.min.css)
- [animate.min.css](node_modules/animate.css/animate.min.css)
- [highlight.min.css](node_modules/@highlightjs/cdn-assets/styles/default.min.css)
- [prism.css](node_modules/prismjs/themes/prism.css)
- [slick.css](node_modules/slick-carousel/slick/slick.css)
- [slick-theme.css](node_modules/slick-carousel/slick/slick-theme.css)
- [normalize.css](node_modules/normalize.css/normalize.css)
- [tailwind.min.css](tailwind.min.css)
- [bulma.min.css](node_modules/bulma/css/bulma.min.css)
- [tabler.min.css](node_modules/@tabler/icons/iconfont/tabler-icons.min.css)
- [bootstrap-icons.css](node_modules/bootstrap-icons/font/bootstrap-icons.css)

<br>

## JavaScript

```html
<script src="URL" type="text/javascript"></script>
```

- [vue.min.js](node_modules/vue/dist/vue.min.js)
- [jquery.min.js](node_modules/jquery/dist/jquery.min.js)
- [popper.min.js](node_modules/@popperjs/core/dist/umd/popper.min.js)
- [bootstrap.min.js](node_modules/bootstrap/dist/js/bootstrap.min.js)
- [isMobile.min.js](node_modules/ismobilejs/dist/isMobile.min.js)
- [validator.min.js](node_modules/validator/validator.min.js)
- [darkmode-js.min.js](node_modules/darkmode-js/lib/darkmode-js.min.js)
- [highlight.min.js](node_modules/@highlightjs/cdn-assets/highlight.min.js)
- [prism.js](node_modules/prismjs/prism.js)
- [slick.min.js](node_modules/slick-carousel/slick/slick.min.js)
- [feather.min.js](node_modules/feather-icons/dist/feather.min.js)

<div id="package" style="text-align: center; margin-top: 6rem; margin-bottom: 2.5rem;">[package.json](package.json) und [package-lock.json](package-lock.json)</div>

<script type="text/javascript" src="node_modules/darkmode-js/lib/darkmode-js.min.js"></script>
<script type="text/javascript" src="node_modules/ismobilejs/dist/isMobile.min.js"></script>
<script>
    var options = {}
    if (isMobile.phone) {
        options.bottom = "15px";
        options.right = "15px";
    
        document.getElementById("package").style.marginTop = "5.5rem";
        document.getElementById("package").style.marginBottom = "3.5rem";
    } else {
        options.bottom = "20px";
        options.right = "20px";
    }
    const darkmode =  new Darkmode(options);
    window.addEventListener("load", darkmode.showWidget());
    function refreshBackground() {
        if (darkmode.isActivated()) {
            document.documentElement.style.background = "black";
        } else {
            document.documentElement.style.background = "white";
        }
    }
    refreshBackground();
    document.getElementsByTagName("button")[0].setAttribute("onclick", "refreshBackground()");
</script>
