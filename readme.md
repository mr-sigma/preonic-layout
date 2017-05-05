# Preonic layout - similar to my Ergodox

## Contributing

Clone the qmk_firmware repository, then clone this repo under `.../qmk_firmware/keyboards/preonic/keymaps/`:

```
git clone https://github.com/qmk/qmk_firmware.git
cd qmk_firmware/keyboards/preonic/keymaps
git clone https://github.com/mr-sigma/preonic-layout.git cadden
```

Run the installation script located under the `/utils` to ensure the Linux Distro has the appropriate programs installed:

```
# Change to the qmk_firmware directory before executing this
sudo util/install_dependencies.sh
```

## Compiling

Plug in the board, press the reset switch on the board and then run the following:

```
sudo make clean && sudo make KEYMAP=cadden dfu
```

The keymap should compile and load!
