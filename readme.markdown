# arduino-starter

basic command-line script to compile and flash arduinos

# install

First install the arduino and avr toolchains.

Linux:

```
$ sudo apt-get install arduino python-pip gcc-avr avr-libc binutils-avr avrdude
```

Mac:

```
$ brew install caskroom/cask/brew-cask python
$ brew cask install arduino crosspack-avr

```

# flash and run

To flash the connected arduino with the program in `main.ino`, do:

```
$ ./make.sh
```

# vendor packages

Put vendor packages in `./vendor`. For example:

```
$ mkdir -p vendor/shield
$ git clone git@github.com:adafruit/Adafruit-Motor-Shield-library.git vendor/shield
```

Then you can `#include` them like so:

``` c
#include <AFMotor.h>
```
