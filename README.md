Description
======

Open source embedded controller to provide communication and peripheral features to embedded systems.

Requirements
--------------

LibOpenCM3 library is needed, GD32F150G6 currently depends on nasty-gd32f150 branch.

Planned for STM32F103C8 and GD32F150G6 two platforms.

Maybe CH552 support will be included in future.

Support Platforms
--------------

Sipeed Tang series Anlogic FPGA boards. (Prime)

Sipeed MaiX series Kendryte K210 boards. (Go)

Prerequisite
--------------
Needs ARM toolchain. Can be installed system wide, loccally, wherever you want

Report here example of local installation from https://gist.github.com/kprasadvnsi/23de96c0e8d1f9ec9d6878777ff4200f
```
mkdir openec-build

cd openec-build

wget https://developer.arm.com/-/media/Files/downloads/gnu-rm/8-2018q4/gcc-arm-none-eabi-8-2018-q4-major-linux.tar.bz2

tar xvf gcc-arm-none-eabi-8-2018-q4-major-linux.tar.bz2

export ARM_GCC=`pwd`/gcc-arm-none-eabi-8-2018-q4-major/bin
export PATH=$PATH:$ARM_GCC
```

Build
--------------

Enter the src directory, and type "make"

```

mkdir openec-build

cd openec-build

git clone --recurse-submodules -j8  https://github.com/michelepagot/open-ec.git

cd open-ec

cd libopencm3

make

cd ../src

make
```


Flash
--------------

TBD

License
--------------

LGPLv3

