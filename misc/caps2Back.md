# Remap CapsLock to Backspce

## Introduction
 *I abhore Caps Lock. After drinking the Colemak Caps Lock Kool-aid, I couldn't stop. Colemak remaps Caps Lock to Backspace which allows for more efficient typing. Stretching your right pinky/ring finger a whole three inches to the upper right is more carpal tunnel inducive than the 2mm stretch with your left pinky.*

## Remap
Using [How-To-Geek](https://www.howtogeek.com/194705/how-to-disable-or-reassign-the-caps-lock-key-on-any-operating-system/)
```
setxkbmap -option caps:backspace
```
```
xmodmap -pke || grep Caps_Lock && xmodmap -pke || grep BackSpace
xmodmap -e "keycode 66 = Backspace Backspace"
```

## Command Explanations
xmodmap modifies keymaps

```xmodmap -pke``` shows the current keyboard mapping
```xmodmap -e``` temporarily changes keys