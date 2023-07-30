# karabiner-tripleclick

## TL;DR
Karabiner Elements-compatible JSON defining a complex modification for modifying input device behavior in single, double, triple click/tap, and hold actions.

This can also serve as a template for other double, triple, and hold key definitions to be used in Karabiner Elements.

## What is it?
This is a settings file designed to modify the behavior of the middle mouse button to perform copy, cut, and paste actions. It is particularly useful for those familiar with X11/Emacs middle mouse key clipboard actions.

When enabled, the mouse's middle key will behave as follows:
- Single click: Middle key
- Double click: Cmd-c (copy)
- Triple click: Cmd-x (cut)
- Hold for 200ms: Cmd-v (paste)

### Emacs Integration
To enhance clipboard actions between Emacs and other macOS apps, the following is an example configuration snippet for Emacs:

```lisp
(custom-set-variables
 '(select-enable-primary t)
 '(select-enable-clipboard t)
 '(save-interprogram-paste-before-kill t)
 '(mouse-drag-copy-region t)
)
```

## Karabiner Elements
Karabiner Elements is a macOS-only, open-source software used for sophisticated remapping of keyboard and mouse inputs.

### Usage
To use this modification, copy the provided JSON file to your `~/.config/karabiner/assets/complex_modifications/` directory. Then, in the Karabiner Elements settings, navigate to `Complex Modifications` and click on `Add Rule` to apply the modification.

<!-- ## TLDR -->
<!-- Karabiner Elements compitable JSON that defines a complex modification for modifying input device behaviour in single, double, triple click/tap, and hold actions. -->

<!-- ## What is it -->

<!-- A settings file that is useful for making the middle mouse button to do copy, cut and paste actions.  Someone who is used to X11/emacs middle mouse key clipboard actions would find this useful. -->

<!-- If you enable this file it will make your mouse middle key behave in this way: -->

<!-- Single click: middle key -->
<!-- Double click: cmd-c -->
<!-- Trible click: cmd-x -->
<!-- Hold for 200ms: cmd-v -->

<!-- ### emacs integration -->

<!-- In conjunction with the following, I found clipboard actions natural between emacs and other mac apps. -->

<!-- ```lisp -->
<!-- (custom-set-variables -->
<!--  '(select-enable-primary t) -->
<!--  '(select-enable-clipboard t) -->
<!--  '(save-interprogram-paste-before-kill t) -->
<!--  '(mouse-drag-copy-region t) -->
<!-- ) -->
<!-- ``` -->

<!-- ## Karabiner Elements -->

<!-- A mac os only software that is FOSS and sophisicated in remapping keyboard and mouse. -->

<!-- ### Usage -->

<!-- copy `JSON` file to your `~/.config/karabiner/assets/complex_modifications/` directory, and in Karabiner Element settings, choose `Complex Modifications`, `Add Rule`. -->
