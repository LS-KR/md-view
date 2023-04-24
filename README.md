
# md-view

Use a special html mark `md-block` to show text in markdown syntax.  

## Usage

Simply put, just insert `<md-block>` in the html document. For example:  

``` html
<md-block>
    Something *you* want to show.
</md-block>
```

### Simple use

Import the url: `https://ls-kr.github.io/md-view/js/md-block.js` as a module, like this:  

``` html
<script type="module" src="https://ls-kr.github.io/md-view/js/md-block.js"></script>
```

then you can use the `<md-block>` mark in your html document.  

### In your website

It's worth noticing that `module` can't be run in JavaScript from local files.  
If the debug is necessary, build in localhost.  

Moreover, the `<md-block>` mark doesn't support the use of `style` or `class`. If nessary, place it in a `<div>`. Like this:  

``` html
<!--html-->
<div class="mainfield">
    <md-block>
        Something...
    </md-block>
</div>
```

``` css
/*css*/
div.mainfield {
    background-color: bisque;
    color: black;
}
```

or

``` html
<!--html-->
<div style="background: bisque; color: black;">
    <md-block>
        Something...
    </md-block>
</div>
```