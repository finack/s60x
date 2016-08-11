S60X keyboard firmware
======================
DIY compact keyboard by Massdrop.

## S60X Resources
- [Massdrop page](https://www.massdrop.com/buy/sentraq-60-diy-keyboard-kit)


## Build Setup

```
brew tap osx-cross/avr
brew install avr-libc
brew install avrdude --with-usb
```


```
make KEYMAP=finack
dfu-programmer atmega32u4 erase && dfu-programmer atmega32u4 flash s60x_lufa.hex && dfu-programmer atmega32u4 start
```
