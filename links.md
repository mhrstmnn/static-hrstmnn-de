---
title: Static Links
lang: de
---

## CSS

```html
<link rel="stylesheet" type="text/css" href="URL" />
```

- [bootstrap.min.css](node_modules/bootstrap/dist/css/bootstrap.min.css)
- [animate.min.css](node_modules/animate.css/animate.min.css)
- [highlight.min.css](node_modules/@highlightjs/cdn-assets/styles/default.min.css)
- [prism.css](node_modules/prismjs/themes/prism.css)
- [slick.css](node_modules/slick-carousel/slick/slick.css)
- [slick-theme.css](node_modules/slick-carousel/slick/slick-theme.css)
- [normalize.css](node_modules/normalize.css/normalize.css)

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

<div id="package" style="text-align: center; margin-top: 6rem; margin-bottom: 2.5rem;">[package.json](package.json) und [package-lock.json](package-lock.json)</div>

<script src="node_modules/darkmode-js/lib/darkmode-js.min.js" type="text/javascript"></script>
<script src="node_modules/ismobilejs/dist/isMobile.min.js" type="text/javascript"></script>
<script>
    var options = {}
    if (isMobile.phone) {
        options.bottom = "15px";
        options.right = "15px";
    
        document.getElementById("package").style.paddingTop = "4rem";
        document.getElementById("package").style.paddingBottom = "3rem";
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
