## fork 自 [paldier 的 K3C 项目](https://github.com/paldier/K3C)，修复了一些编译错误。  

### Ubuntun 20.04 TLS 为例  
`sudo apt-get update`  
`sudo apt-get upgrade`  
`sudo apt-get install git make gcc g++ libncurses-dev zlib1g-dev libssl-dev unzip python2.7 cmake`  
`git clone https://github.com/swordv2/K3C.git`  
`./scripts/feeds update -a`  
`/scripts/feeds install -a`  
`make menuconfig` (***load k3cxx.config***)  
`make tools/download`  
`make toolchain/download`  
`make toolchain/install`  


>This is the buildsystem for the OpenWrt Linux distribution  
>
>Please use "make menuconfig" to configure your appreciated  
>configuration for the toolchain and firmware.  
>
>You need to have installed gcc, binutils, patch, bzip2, make(>=V3.81),   
>gettext, pkg-config, unzip, libz-dev and libc headers.  
>
>Simply running 'make' will build your firmware.  
>It will download all sources, build the cross-compile toolchain,   
>the kernel and all choosen applications.  
>
>The OpenWrt system is documented in docs/. You will need a LaTeX distribution  
>and the tex4ht package to build the documentation. Type make -C docs/ to build it.  
>
>Building your own firmware you need to have access to a Linux, BSD or MacOSX system.  
>Cygwin will not be supported because of the lack of case sensitiveness.  
>
>Sunshine!  
>	Your OpenWrt Project  
>	http://openwrt.org  
>
>
>NOTE:  
>	This environment is modified by Lantiq:  
>	The number of targets and packages is reduced and some default   
>	configurations are provided. Please use the script  
>		./scripts/ltq_change_environment.sh  
>	to "list", "switch" or "save" these configurations.  
>
