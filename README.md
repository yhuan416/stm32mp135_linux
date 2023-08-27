# stm32mp135_linux

## 拉取源码

``` sh
git clone git@github.com:yhuan416/stm32mp135_linux.git linux
```

## 构建

``` sh
./build.sh
```

## 配置内核

``` sh
make ARCH=arm CROSS_COMPILE=arm-none-linux-gnueabihf- menuconfig
make ARCH=arm CROSS_COMPILE=arm-none-linux-gnueabihf- savedefconfig
cp defconfig arch/arm/configs/stm32mp1_atk_defconfig
```
