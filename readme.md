## What happens?
Any link having the attribute `target="_blank"` opening a new window containing `window.close()`, will be able to close your tab.

## What should happen
According to the specs a [`window.close`](https://developer.mozilla.org/en-US/docs/Web/API/Window/close) call be able to close a windows __that were opened by a script using the `window.open()` method__

> This method is only allowed to be called for windows that were opened by a script using the window.open() method. If the window was not opened by a script, an error similar to this one appears in the console: Scripts may not close windows that were not opened by script.

## Demo

Click on the first link and then on the second one to see your browser tab closing immediately
[demo](https://dreipol.github.io/firefox-window-close-bug/index.html)

# Specs

This issue appears only on firefox

Firefox versions tested
- v51.0a2
- v49.0.2