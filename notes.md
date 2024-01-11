# Summary CSS

## flex

### 1

> HTML Code

```html
<!DOCTYPE html>

<head>
    <title>Index Page</title>
    <link rel="stylesheet" href="CSS/style.css">
</head>

<body>
   <div class="parent">
    <div class="item1 item">
        <p>item1</p>
    </div>
    <div class="item2 item">
        <p>item2</p>
    </div>
    <div class="item3 item">
        <p>item3</p>
    </div>
   </div>
</body>

</html>
```

> CSS Code

``` css
:root {
    --width: 100px;
    --height: 100px;
}

div.parent {
    height: 680px;
    background-color: cadetblue;
    display: flex;
    
    /* flex-direction: row; row is Default || row-reverse || column || column-reverse*/
    flex-direction: row;
    
    /* justify-content: flex-start is Default || flex-end || center || space-between || space-around || space-evenly*/
    justify-content: space-evenly;


    /* align-items: flex-start is Default || flex-end || center*/
    align-items: center;
}

div.parent div.item {
    width: var(--width);
    height: var(--width);
    display: flex;
    justify-content: center;
    align-items: center;
}

div.parent div.item1 {
    background-color: brown;
}

div.parent div.item2 {
    background-color: royalblue;
}

div.parent div.item3 {
    background-color: rebeccapurple;
}
```

### 2

> HTML Code

```html
<!DOCTYPE html>

<head>
    <title>Index Page</title>
    <link rel="stylesheet" href="CSS/style.css">
</head>

<body>
   
    <section>
        <div class="left"></div>
        <div class="right"></div>
    </section>
    
</body>

</html>
```

> CSS Code

```css
section {
    height: 680px;
    display: flex;
    background-color: cadetblue;
}

div.left {
    background-color: brown;
    flex: 1;
}

div.right {
    background-color: darkolivegreen;
    flex: 1;
}
```
