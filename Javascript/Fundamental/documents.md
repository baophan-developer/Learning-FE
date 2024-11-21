# **Hello, world!** (https://javascript.info/hello-world)

## The "script" tag:

-   Anywhere into an HTML document
-   The <code><script></code> tag contains Javascript code which is automatically executed when the browser processes the tag.

## Modern markup:

The <code><script></code> tag has a few attributes that are rarely used nowadays but can still be found in old code:

-   **The <code>type</code> attribute <code><script type=...></code>:**
    The old HTML standard, HTML4, required a script to have a type (type="text/javascript"). It's not required anymore.
    The modern HTML standard totally changed the meaning of this attribute. Now, it can be used for javascript modules.
-   **The <code>language</code> attribute <code><script language=...></code>:**
    This attributes was meant to show the language of the script (Javascript is default).
    There is no need to use it.
-   **Comment before and after scripts.**
    <script type="text/javascript"><!--
        ...
    //--></script>
