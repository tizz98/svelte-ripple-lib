# svelte-ripple-lib

Shows an issue with using `xrpl.js`/`ripple-lib` in svelte.

1. Running as-is, when loading the browser:
    ```
    Uncaught ReferenceError: exports is not defined
    ```
1. After adding `<script> var exports = {}; </script>` to `index.html`:
    ```
    Uncaught ReferenceError: require is not defined
    ```
