# my-vim-cheatsheet


### Tricks for selection and vim surround

You must install the [vim-surround](https://github.com/tpope/vim-surround) to apply the tricks.
Also need to make sure that you are on the `normal` mode before you try the tricks.

```
    Vim
    Hello world
```

Put the cursor at the Vim, any word, then type `ysw` + `<h1>`. This will surround the text into `h1` element.
Then cursor on the `Hello world` press `V` + `S` + `<span> will surround the paragraph into `span` element.

```html
   <h1>Vim</h1>
   <span>Hello world</span>
```

Press `V` then go to next line until you select the whole line. Press `S` + `<header>`. This will contain
all of the elements inside teh `header` element

```html
   <header>
     <h1>Vim</h1>
     <span>Hello world</span>
   </header>
```

Move the cursor at `<span>` then press `cst` + `<p>`, will change from `span` into `p`.

```html
   <header>
     <h1>Vim</h1>
     <p>Hello world</p>
   </header>
```

Cursor at the `<p>` then pressing `dit` will delete the content. Alternatively,
you can use `cit` to write immediately. Change the content into `A clever boy`.

```html
   <header>
     <h1>Vim</h1>
     <p>A clever boy</p>
   </header>
```

Cursor at the `<header>` then press `vat` to visually select the element and its content.
`vit` will select its content but not the parent element.
Then press `S` + `<article>` will surround the elements by the `article`.

```html
  <article>
     <header>
       <h1>Vim</h1>
       <p>A clever boy</p>
     </header>
  </article>
```




