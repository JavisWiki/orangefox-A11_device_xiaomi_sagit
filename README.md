# 本项目fork自0ranko0P/twrp_device_xiaomi_sagit，暂无修改，感谢@0ranko0P的贡献。

## 本项目可用于编译OrangeFox_11，按以下步骤编译：

打开并按以下顺序执行网站中的编译教程：https://wiki.orangefox.tech/en/dev/building

1、执行步骤0、1A

2、步骤2调整为：

  cd ~/fox_11.0  
  git clone https://github.com/JavisWiki/orangefox-A11_device_xiaomi_sagit.git -b android-11 device/xiaomi/sagit
  
3、执行步骤3，其中最终启动编译的命令使用：

  lunch twrp_sagit-eng && mka recoveryimage


以上。



# android_device_xiaomi_sagit
Tree for building TWRP for Xiaomi MI 6

## Note
Only compatible with Android 11 and newer

## To compile

repo init --depth=1 -b twrp-11 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git

. build/envsetup.sh && lunch twrp_sagit-eng

mka adbd recoveryimage

## Device specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core (4x2.45 GHz Kryo & 4x1.9 GHz Kryo)
Chipset | Qualcomm MSM8998 Snapdragon 835
GPU     | Adreno 540
Memory  | 6 GB RAM
Shipped Android Version | 7.1.1
Storage | 64/128 GB
Battery | Li-Po 3350 mAh battery
Display | 1080 x 1920 pixels, 5.15 inches (~428 ppi pixel density)
Rear Camera  | Dual 12 MP (27mm, f/1.8, OIS 4-axis & 52mm, f/2.6), phase detection autofocus, dual-LED (dual tone) flash


## Device picture

![Xiaomi Mi 6](https://xiaomi-mi.com/uploads/CatalogueImage/xiaomi-mi-6-exclusive-edition-6gb128gb-dual-sim-ceramic-black-01_15554_1492602917.jpg "Xiaomi Mi 6 in black")

## Kernel Source

https://github.com/Miccia94/kernel_xiaomi_msm8998/tree/twrp
