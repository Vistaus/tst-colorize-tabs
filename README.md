[![Mozilla Add-on Version](https://img.shields.io/amo/v/tst-colorize-tabs?label=version&color=blue)](https://addons.mozilla.org/firefox/addon/tst-colorize-tabs/)
[![Mozilla Add-on](https://img.shields.io/amo/users/tst-colorize-tabs?color=%23FF6611&label=users&logo=Firefox)](https://addons.mozilla.org/firefox/addon/tst-colorize-tabs/)
[![Mozilla Add-on Stars](https://img.shields.io/amo/stars/tst-colorize-tabs)](https://addons.mozilla.org/firefox/addon/tst-colorize-tabs/)
![CI/CD](https://github.com/emvaized/TST-Colorize-Tabs/workflows/CI/CD/badge.svg)

# <sub align="bottom"><img height="40px" src="./src/images/color.png"></sub> TST Colorize Tabs

This extension allows to set individual color for each tab in order to highlight them. Currently available colors: red, green, blue, yellow, brown, purple, orange. [Tree Style Tabs](https://addons.mozilla.org/firefox/addon/tree-style-tab/) extension is required for it to run. 

<a href="https://addons.mozilla.org/firefox/addon/tst-colorize-tabs/"><img src="https://user-images.githubusercontent.com/585534/107280546-7b9b2a00-6a26-11eb-8f9f-f95932f4bfec.png" alt="Get for Firefox"></a>

> Huge thanks to [@irvinm](https://github.com/irvinm) for many contributions to this project! 🎉 <br> Check out his addon [TST Lock](https://github.com/irvinm/TST-Lock)


## Important notes

- Extension may conflict with other extensions which change tabs color, such as [VivaldiFox](https://addons.mozilla.org/firefox/addon/vivaldifox/) or [TST Colored Tabs](https://addons.mozilla.org/firefox/addon/tst-colored-tabs/)

- When you close a tab or window and then use Firefox to "restore" these tabs, they will not have the original Tab IDs assigned.  Because of this (and no great way of mapping "new tabs created\restored" to old closed tabs), once you close a tab\window, the associated color information will be deleted.  
**This means any restored tabs will not have their color information retained and will be treated as "new".**

## Keyboard hotkeys

You can change shortcuts via `about:addons` -> Cogwheel -> Manage Extension Shortcuts ([guide](https://support.mozilla.org/en-US/kb/manage-extension-shortcuts-firefox))

- <kbd>Alt</kbd> + <kbd>1</kbd> – Set red color for selected tabs
- <kbd>Alt</kbd> + <kbd>2</kbd> – Set green color for selected tabs
- <kbd>Alt</kbd> + <kbd>3</kbd> – Set blue color for selected tabs
- <kbd>Alt</kbd> + <kbd>4</kbd> – Set yellow color for selected tabs
- <kbd>Alt</kbd> + <kbd>5</kbd> – Set brown color for selected tabs
- <kbd>Alt</kbd> + <kbd>6</kbd> – Set purple color for selected tabs
- <kbd>Alt</kbd> + <kbd>7</kbd> – Set orange color for selected tabs
- <kbd>Alt</kbd> + <kbd>0</kbd> – Remove color from selected tabs
- <kbd>Alt</kbd> + <kbd>Down</kbd> – Switch to the next colorized tab
- <kbd>Alt</kbd> + <kbd>Up</kbd> – Switch to the previous colorized tab

## How to change colors

To customize colors, you can use TreeStyleTab's custom CSS.
Here are default style rules for each color, which you could override in Tree Style Tabs settings:

```
.tab.self-colored-red tab-item-substance { 
    background-color: rgba(255,0,0,0.2) !important;
}
.tab.self-colored-green tab-item-substance { 
    background-color: rgba(0,255,0,0.2) !important; 
}
.tab.self-colored-blue tab-item-substance { 
    background-color: rgba(0,128,255,0.2) !important;
}
.tab.self-colored-yellow tab-item-substance { 
    background-color: rgba(255,255,0,0.2) !important; 
}
.tab.self-colored-brown tab-item-substance { 
    background-color: rgba(139,69,19,0.2) !important; 
}
.tab.self-colored-purple tab-item-substance { 
    background-color: rgba(75,0,130,0.2) !important; 
}
.tab.self-colored-orange tab-item-substance { 
    background-color: rgba(255,69,0,0.2) !important;
}
```

## Contribution
Any contributions are welcome! Please feel free to fork this extension and create pull request to suggest your changes.

Few ideas to work on: 
- [ ] Ability to change color values on a settings page instead of using CSS (https://github.com/emvaized/tst-colorize-tabs/issues/9)
- [ ] Apply 'light/dark' mode to the CSS color values as well, so that users could specifiy different colors for dark mode
- [ ] List all colorized tabs in the extension popup, with switch to tab on click

-----

Extension logo (color.png) provided by:  <a href="https://www.flaticon.com/free-icons/color-wheel" title="color wheel icons">Color wheel icons created by Hasymi - Flaticon</a>
