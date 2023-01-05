# Partial pager Sublime Text plugin

## The problem

When using pageup and pagedown keys to navigate, the file scrolls the full viewport. It would be nice to be able to scroll a fraction of the viewport to make it easier to track the jumps visually.

## The solution

This plugin creates a custom command "partial_pager" that will scroll the page by the provided amount. This command can be then binded to pageup, pagedown keys.

## Create a keybinding

After installing the plugin create a key binding to the command. In this example the viewport is scrolled by half the viewport.

```
    { "keys": ["pageup"], "command": "partial_pager", "args": {"amount": -0.5}},
    { "keys": ["pagedown"], "command": "partial_pager","args": {"amount": 0.5}},
```

## Credits

Full credits for this plugin go to https://forum.sublimetext.com/t/a-better-paging-behaviour/42454/9
