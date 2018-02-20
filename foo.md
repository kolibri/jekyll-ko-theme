---
layout: page
title: Foo
permalink: /foo/
---

# Foo


```css
@import url("http://fonts.googleapis.com/css?family=Inder");
@import url("http://fonts.googleapis.com/css?family=Droid+Sans+Mono");



* {
    margin: 0;
    padding: 0;
    font-size: 1em;
}

body {
    width: 100%;
    height: 100%;
    font-family: 'Inder', sans-serif;
}


@mixin ko($background, $contrast) {
    background-color: $background;
    position: relative;
    width: 96vw;
    height: 96vh;
    padding: 1vh 1vw;
    margin: 0;
    margin-bottom: 8vh;

    >header,
    >main,
    >.main,
    >footer {
        width: 95vw;
        border-right: 1vw $contrast solid;
    }

    >header {
        height: 3vw;
        border-top: 1vw $contrast solid;
    }
    >header>* {
        margin-right: 3vw;
        float: left;
    }

    >main,
    >.main,
    >main::before,
    >.main::before {
        height: 83vh;
    }

    >footer,
    >footer::before {
        height: 8vw;
    }

    >header::before,
    >main::before,
    >.main::before,
    >footer::before {
        content: ' ';
        display: block;
        width: 10vw;
        background: repeating-linear-gradient(90deg, $contrast, $contrast 2vw, $background 2vw, $background 4vw);
        float: left;
    }

    >header::before {
        height: 3vw;
    }
```
