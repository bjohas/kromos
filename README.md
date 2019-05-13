# kromos
keyboard experiments for Chrome OS - k-(ch)rom(e)-OS

Some keyboard experiments based on other existing keyboard plugins, mainly https://github.com/OTL/emacs_shortcuts_ime but with additional inspiration from https://github.com/bjohas/extra-keyboards-for-chrome-os.


## Installation (from https://github.com/bjohas/extra-keyboards-for-chrome-os)

1. Go to chrome://extensions.
2. Click on "Load unpacked extensions...".
3. Pick the directory containing the manifest for the extension you want to
enable.
4. Logout and then login again. (This may not be necessary.)
5. Go to chrome://settings/languages.
6. Add the relevant language, e.g. French for the bepo keyboard layout.
7. Select the relevant keyboard layout and input method.
8. Optionally, remove any keyboard layouts or input methods that are no longer
required.

## How to Use

1. Press Ctrl + Shift + Space to cycle through the enabled keyboard languages.
2. Type away…
3. Ctrl + Space to toggle between the most recently used keyboard languages.

## Known Limitations
- These extensions are not allowed on the login/lock screen.
- These extensions are not allowed on password fields.
- Some keyboard shortcuts only work when an input field has focus.
- Some mappings seem to be slow to respond

## Other similar repos:
- https://github.com/ento/chromeos-key-remapper
- https://bitbucket.org/sharat87/keyboard-fu https://github.com/sharat87/keyboard-fu
- https://github.com/philc/vimium/blob/master/README.md

# Issues
Keyboard remapping isn't very flexible. E.g. currently (Chrome OS 74) it doesn't seem possible to remap dictation (search+d) to another key. This means that search+d isn't available e.g. for forward delete. C.f. also https://bugs.chromium.org/p/chromium/issues/detail?id=211906 for some details about how this is set in the source.

For many custom keyboard shortcuts letters must be used, making it impossible to assign e.g. alt-[.

Keyboard mapping in Linux/X11 container may well follow non-Linux mechanisms? https://chromium.googlesource.com/chromiumos/platform2/+/413a646b5b7067a989bab2ef9fca0c3a4515cc22/vm_tools/sommelier/README.md#accelerators

It may be possible to circumvent some of this in developer mode? (Not sure!)
