# pad-your-args

A vscode extension that will highlight unpadded parentheses in Lua.

```lua
local mieou = function ( x, y ) end -- :)
local woof = function (x, y) end    -- :(
local baa = meiou( 3, 4 );          -- :)
local moo = woof(3, 4);             -- :(
```

Find it on the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/items?itemName=benjaminporter.pad-your-args).

Consider making the highlight stand out more by adding this to your vscode settings:

```json
"editor.tokenColorCustomizations": {
    "textMateRules": [{
        "scope": "invalid.illegal",
        "settings": {
            "foreground": "#FF0000",
            "fontStyle": "bold underline",
        }
    }]
}
```