S60X keyboard firmware
======================
DIY compact keyboard by Massdrop.

## S60X Resources
- [Massdrop page](https://www.massdrop.com/buy/sentraq-60-diy-keyboard-kit)


## Build
Move to this directory then just run `make` like:

    $ make

Use `make -f Makefile.pjrc` if you want to use PJRC stack but I find no reason to do so now.


## Keymap
Several version of keymap are available in advance but you are recommended to define your favorite layout yourself. To define your own keymap create file named `keymap_<name>.c` and see keymap document(you can find in top README.md) and existent keymap files.

To build firmware binary hex file with a certain keymap just do `make` with `KEYMAP` option like:

    $ make KEYMAP=<name>


### 1  Default Keymap

[keymap_default.c](keymap_default.c) is a SpaceFn keymap designed by Julien Pecqueur.


#### 1.0 Default layer
    ,-----------------------------------------------------------.
    |`  |  1|  2|  3|  4|  5|  6|  7|  8|  9|  0|  -|  =|Backsp |
    |-----------------------------------------------------------|
    |Tab  |  Q|  W|  E|  R|  T|  Y|  U|  I|  O|  P|  [|  ]|    \|
    |-----------------------------------------------------------|
    |Ctrl  |  A|  S|  D|  F|  G|  H|  J|  K|  L|  ;|  '|Return  |
    |-----------------------------------------------------------|
    |Shift   |  Z|  X|  C|  V|  B|  N|  M|  ,|  .|  /|Shift     |
    |-----------------------------------------------------------|
    |Fn1 |Gui |Alt |        SpaceFn         |Alt |Gui |App |BTN2|
    `-----------------------------------------------------------'


#### 1.1 Function layer
    ,-----------------------------------------------------------.
    |Esc| F1| F2| F3| F4| F5| F6| F7| F8| F9|F10|F11|F12|Delete |
    |-----------------------------------------------------------|
    |     |Prv|Ply|Nxt|   |   |PUp|Hom|Up |End|Psc|Slk|Pau|Ins  |
    |-----------------------------------------------------------|
    |Caps  |Vl-|Mut|Vl+|   |   |PDn|Lef|Dow|Rig|   |   |PEnt    |
    |-----------------------------------------------------------|
    |        |   |   |   |   |   |   |Ly0|Ly1|Ly2|Ly3|          |
    |-----------------------------------------------------------|
    |    |    |    |                        |    |    |    |    |
    `-----------------------------------------------------------'
