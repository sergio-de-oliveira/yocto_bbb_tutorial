# YOCTO BEAGLEBONE BLACK TUTORIAL<br>INSTALL PACKAGES

<!---------------------------------------------------------------->
### Prerequisites

Se how to configure, build and flash a Yocto image for Beaglebone Black on [introduction](../01_introduction/README.md) steps.
<br>
<br>

<!---------------------------------------------------------------->
## STEP 1: Source the Build Enviroment Setup Script
Source oe-init-build-env:
```
source oe-init-build-env
```
<br>
<br>

<!---------------------------------------------------------------->
## STEP 2: Verify desired recipes packages
Verify desired recipes packages (ex.: pyhton3 and git):
```
bitbake-layers show-recipes python3
bitbake-layers show-recipes git
```
<br>
<br>

<!---------------------------------------------------------------->
## STEP 3: Configure desired packages
Add the desired packages on local.conf:
```
IMAGE_INSTALL:append = " python3 "
IMAGE_INSTALL:append = " git "
```
<br>
<br>

<!---------------------------------------------------------------->
## STEP 4: Build the image
Follow [introduction](../01_introduction/README.md) steps.
<br>
<br>

<!---------------------------------------------------------------->
## STEP 5: Flash image to Beaglebone eMMC
Follow [introduction](../01_introduction/README.md) steps.
<br>
<br>

<!---------------------------------------------------------------->
## REFERENCE LINKS
- [Munawar-git/YoctoTutorials](https://github.com/Munawar-git/YoctoTutorials)

<br>

<!---------------------------------------------------------------->
## REFERENCE VIDEOS
- [Yocto Tutorial - 00 Introduction to Yocto - Building Linux for BeagleBone Black (STEP WISE!!)](https://www.youtube.com/watch?v=5fj05BWryhM)
- [Yocto Tutorial - 01 Flashing Yocto Built Custom Linux OS onto BeagleBone Black (STEP-BY-STEP!!)](https://www.youtube.com/watch?v=S3NG7ch3Xgw)
- [Yocto Tutorial - 02 Understanding the local.conf in Yocto: How to Customize Linux Distribution](https://www.youtube.com/watch?v=CQw02-PMNrA)
- [Yocto Tutorial - 03 Understanding the bblayers.conf File in Yocto (IN-DEPTH GUIDE!!)](https://www.youtube.com/watch?v=GyLRWAe-b7k)
- [Yocto Tutorial - 04 Adding Packages (IMAGE_INSTALL) - Customizing OS with Yocto (Step by Step)](https://www.youtube.com/watch?v=naszh2WoHAM)
- [Yocto Tutorial - 05 Create and Add Layer with Yocto (Detailed!!)](https://www.youtube.com/watch?v=-atEGK1DzIQ)
- [Yocto Tutorial - 06 Understand Basic Yocto Variables (WITH EXAMPLES!!) | PN PV PR WORKDIR S D B](https://www.youtube.com/watch?v=g3Xfckd-mE8)
- [Yocto Tutorial - 07 Variable Assignment Operators (Part-1) | Types of Variable Assignment Operators](https://www.youtube.com/watch?v=kCl6D5WwBXQ)
- [Yocto Tutorial - 07 Variable Assignment Operators (Part-2) | Setting Default Value ?=, ??=](https://www.youtube.com/watch?v=KsU11k5lEX0)
- [Yocto Tutorial - 07 Variable Assignment Operators(Part-3) | Overriding Default Value =, :=](https://www.youtube.com/watch?v=axyktiRLXgs)
- [Yocto Tutorial - 07 Variable Assignment Operators (Part-4) | Append(+=) and Prepend(=+) with Spaces](https://www.youtube.com/watch?v=G4qoy1me7fY)
- [Yocto Tutorial - 07 Variable Assignment Operators (Part-5) | Append(.=) & Prepend(=.) without Spaces](https://www.youtube.com/watch?v=hP2zG6icS1Y)
- [Yocto Tutorial - 07 Variable Assignment Operators (Part-6) | :append :prepend and :remove](https://www.youtube.com/watch?v=U4QRXAO4AfA)
- [Yocto Tutorial - 08 Creating a Simple Hello World Yocto Recipe(FROM SCRATCH!) | With C Program](https://www.youtube.com/watch?v=YSITCPhk_qU)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-1) | A Brief Description](https://www.youtube.com/watch?v=a6dB7Z2HlNM)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-2) | do_fetch (With Example!!)](https://www.youtube.com/watch?v=ZIJACtKHN84)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-3) | do_unpack (With Example!!)](https://www.youtube.com/watch?v=1KpKzFY9rw0)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-4) | do_patch (With Example!!)](https://www.youtube.com/watch?v=H3LVO1zRpBA)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-5) | do_configure (With Example!!)](https://www.youtube.com/watch?v=YuB_bxjFePs)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-6) | do_compile (With Example!!)](https://www.youtube.com/watch?v=RtAAO6uZ59k)
- [Yocto Tutorial - 09 Yocto Build Tasks (Part-7) | do_install (With Example!!)](https://www.youtube.com/watch?v=ZKIcylBUNw8)
- [Yocto Tutorial - 10 How to create a Patch for a Recipe | Step by Step in Detail Guide](https://www.youtube.com/watch?v=jeMzB8N-wR0)
- [Yocto Tutorial - 11 How to Add Runtime Dependencies | RDEPENDS | A Comprehensive Guide](https://www.youtube.com/watch?v=x4CgMt7VqNo)
- [Yocto Tutorial - 12 Demystifying RPROVIDES | With Easy to Understand Examples](https://www.youtube.com/watch?v=H4aRXJq5yK4)
- [Yocto Tutorial - 13 Managing Package Conflicts with RCONFLICTS | Clear Cut Examples](https://www.youtube.com/watch?v=PT51np3hxzs)
- [Yocto Tutorial - 14 Exploring Build Dependencies (PART-1) | DEPENDS | Example with Testing](https://www.youtube.com/watch?v=mF-VpN6Rc88)
- [Yocto Tutorial - 14 Exploring Build Dependencies (PART-2) | DEPENDS | Example with Testing](https://www.youtube.com/watch?v=ycbQYm1s37s)
- [Yocto Tutorial - 15 Build Dependencies Management | PROVIDES](https://www.youtube.com/watch?v=qT3IuaRfjCg)
- [Yocto Tutorial - 16 Customizing Package Provider | PREFERRED_PROVIDER](https://www.youtube.com/watch?v=JGOtX6ZAwak)
- [Yocto Tutorial - 17 Mastering Package Version Selection with PREFERRED_VERSION | With EXAMPLE](https://www.youtube.com/watch?v=jI2f3lCD4WE)
- [Yocto Tutorial - 18 Comprehensive Guide to use oe_runmake | Building with Makefile](https://www.youtube.com/watch?v=_7nQHSvqtbI)
- [Yocto Tutorial - 19 Customizing Builds with EXTRA_OEMAKE | Passing Additional Parameters](https://www.youtube.com/watch?v=it1aYiWmTHQ)
- [Yocto Tutorial - 20 BBMASK | Recipe Control for Debugging](https://www.youtube.com/watch?v=K4GY8C3SMf4)
- [Yocto Tutorial - 21 BBappend File | Modifying Recipe using bbappend File](https://www.youtube.com/watch?v=IxXSABanxEQ)
- [Yocto Tutorial - 22 FILESEXTRAPATHS in bbappend | Extending Resources Path](https://www.youtube.com/watch?v=thOvmzsVbrA)
- [Yocto Tutorial - 23 Cleaning Up Recipes (Part-1) | Bitbake 'clean,' 'cleansstate' & 'cleanall' Tasks](https://www.youtube.com/watch?v=lfORqtu8pJg)
- [Yocto Tutorial - 23 Cleaning Up Recipes (Part-2) | Bitbake 'clean,' 'cleansstate' & 'cleanall' Tasks](https://www.youtube.com/watch?v=0D35Ophz-v4)
- [Yocto Tutorial - 23 Cleaning Up Recipes (Part-3) | Bitbake 'clean,' 'cleansstate' & 'cleanall' Tasks](https://www.youtube.com/watch?v=52_rmFnr0Vo)
- [Yocto Tutorial - 24 Integrating SystemD (Part-1) | Understanding Init Manager](https://www.youtube.com/watch?v=_M1EjgY2S0Q)
- [Yocto Tutorial - 24 Integrating SystemD (Part-2) | Understanding Init Manager](https://www.youtube.com/watch?v=5iFZZK4l6mM)
- [Yocto Tutorial - 25 SystemD Service Recipes (Part-1) | A Step-by-Step Tutorial](https://www.youtube.com/watch?v=nSeaZ1khchA)
- [Yocto Tutorial - 25 SystemD Service Recipes (Part-2) | A Step-by-Step Tutorial](https://www.youtube.com/watch?v=TXfTY2rfl0Q)
- [Yocto Tutorial - 26 Kernel Configuration | Menuconfig](https://www.youtube.com/watch?v=Q0dWV9jWwkM)
- [Yocto Tutorial - 27 Kernel Configuration with defconfig | savedefconfig](https://www.youtube.com/watch?v=5BmEig-D2lA)
- [Yocto Tutorial - 28 Kernel Configuration using Config Fragments | diffconfig](https://www.youtube.com/watch?v=uErrAUtxgt4)
- [Yocto Tutorial - 29 Kernel Development | Out of Tree Kernel Module](https://www.youtube.com/watch?v=aLL3cUDoz10)
- [Yocto Tutorial - 30 Kernel Development | Character Device Driver/Module](https://www.youtube.com/watch?v=gdHBmgsux1E)
- [Yocto Tutorial - 31 Kernel Development | Device Driver Integration in Mainline Kernel (Part 1)](https://www.youtube.com/watch?v=0BaNjmVsXNY)
- [Yocto Tutorial - 31 Kernel Development | Device Driver Integration in Mainline Kernel (Part 2)](https://www.youtube.com/watch?v=IavTmJY5atg)
- [Yocto Tutorial - 31 Kernel Development | Device Driver Integration in Mainline Kernel (Part 3)](https://www.youtube.com/watch?v=VFRrbMVboyE)
- [Yocto Tutorial - 32 Classes & bbclass File | SIMPLIFIED!!!](https://www.youtube.com/watch?v=oAfWQTqAe8g)
- [Yocto Tutorial - 33 Creating Custom Class | inherit | bbclass Example](https://www.youtube.com/watch?v=XTqKMRkLlyU)
- [Yocto Tutorial - 34 More About Classes | Nested Class | INHERIT in Conf](https://www.youtube.com/watch?v=6NLuUIMDzeI)
- [Yocto Tutorial - 35 Search a Recipe Locally | bitbake-layers | show-recipes | SIMPLIFIED !!!](https://www.youtube.com/watch?v=jLjsNr8-E9c)
- [Yocto Tutorial - 36 Search Recipe in all Layers Locally | Using find Command | Like a Pro](https://www.youtube.com/watch?v=2PD8fpqgbXc)
- [Yocto Devtool Tutorial - 37 Introduction to Devtool | Brief and Comprehensive](https://www.youtube.com/watch?v=HfbwRfurNfM)
- [Yocto Devtool Tutorial - 38 Create Recipe with Devtool | add & build Commands](https://www.youtube.com/watch?v=Apfwyf_yEzI)
- [Yocto Devtool Tutorial - 39 Testing With Devtool | deploy-target & undeploy-target Commands](https://www.youtube.com/watch?v=S5cX9op1pYk)
- [Yocto Devtool Tutorial - 40 Export Recipe to Meta Layer | devtool finish command](https://www.youtube.com/watch?v=2K2yNtt7YqI)
- [Yocto Devtool Tutorial - 41 Patch with Devtool Modify | Make Changes in Source](https://www.youtube.com/watch?v=Z65gY6ot3Ug)
- [Yocto Devtool Tutorial - 42 Upgrading Recipes using devtool upgrade & devtool rename](https://www.youtube.com/watch?v=us9YE7sBDBU)
- [Yocto Devtool Tutorial - 48 Creating Kernel Module Recipe with Devtool](https://www.youtube.com/watch?v=LN_ulwXvE0k)
- [Yocto Devtool Tutorial - 49 Creating Recipe for CMake Based Build](https://www.youtube.com/watch?v=5ERPwxeeGNA)
- [Yocto Devtool Tutorial - 50 Creating Recipe for autotools Based Build](https://www.youtube.com/watch?v=yr-fOtUpc3Y)
- [Yocto Tutorial - 51 What is a Distro? | Poky Distro | Distro Variables & Features](https://www.youtube.com/watch?v=US2aRdAL4ZU)
- [Yocto Tutorial - 52 Create Custom Distro | A Guide from Scratch | Create, Build & Verify](https://www.youtube.com/watch?v=qJbI4tk227M)
- [Yocto Tutorial - 53 Conditionally Add or Remove Packages and Kernel Configs | Comment Special](https://www.youtube.com/watch?v=whs1T9zat-s)
- [Yocto Tutorial - 54 What is a Machine? | Understanding Machine File and its Variables](https://www.youtube.com/watch?v=zu8vcy9EWcU)