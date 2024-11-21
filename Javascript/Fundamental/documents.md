# **Hello, world!** [link](https://javascript.info/hello-world)

## The "script" tag:

-   Anywhere into an HTML document
-   The <code><script></code> tag contains Javascript code which is automatically executed when the browser processes the tag.

## Modern markup:

The <code><script></code> tag has a few attributes that are rarely used nowadays but can still be found in old code:

-   **The <code>type</code> attribute <code><script type=...></code>:**
    -   The old HTML standard, HTML4, required a script to have a type (type="text/javascript"). It's not required anymore.
    -   The modern HTML standard totally changed the meaning of this attribute. Now, it can be used for javascript modules.
-   **The <code>language</code> attribute <code><script language=...></code>:**
    -   This attributes was meant to show the language of the script (Javascript is default).
    -   There is no need to use it.
-   **Comment before and after scripts.**

## External scripts:

Script files are attached to HTML with the <code>scr</code> attribute:

```html
<script scr="/path/to/script.js"></script
```

Here, <code>/path/to/script.js</code> is an absolute path to the script from the site root. One can also provide a relative path from the current page.

We can give a full URL as well. For instance:

```html
<script scr="https://cdnjs.cloudflare.com/ajax/libs/lodash.js/4.17.11/lodash.js"></script>
```

To attach several script, use multiple tags:

```html
<script src="/js/script1.js"></script>
<script src="/js/script2.js"></script>
…
```

**Please note:**
<code>
As a rules, only the simplest scripts are put into HTML. More complex ones reside in separate files.
The benefit of a separate files is that the browser will download it and store it in its cache.
Other pages that reference the same script will take it from the cache instead of downloading it, so the file is actually downloaded only once.
The reduces traffic and makes pages faster.
</code>

**If <code>src</code> is set, the script content is ignored**
