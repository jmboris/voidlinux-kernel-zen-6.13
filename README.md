# voidlinux-kernel-zen-6.13
Kernel 6.13 with patch zen , template for VoidLinux


![image](https://github.com/user-attachments/assets/5b815abe-9f2e-4d31-bb01-68dab60b1c6b)




This repository contains the xsrc folder necesary to build the linux 6.13-zen and linux6.13-zen-headers, as well the template to install kernel 6.13an the path for it from zen-kernel repository.


## NOTE

If you **ONLY** want to use this template you need to download the patch file zst (https://github.com/zen-kernel/zen-kernel/releases/download/v6.13-zen1/linux-v6.13-zen1.patch.zst) , extract it and place it in the patches folder inside the 
linux6.13-zen folder , like the tree below

zen repository (https://github.com/zen-kernel/zen-kernel/releases/tag/v6.13-zen1) 

```bash

linux6.13-zen
├── files
│   ├── arm64-dotconfig
│   ├── i386-dotconfig
│   ├── mv-debug
│   └── x86_64-dotconfig
├── patches
│   ├── fix-musl-btf-ids.patch
│   ├── fix-musl-objtool.patch
│   ├── fixdep-largefile.patch
│   ├── linux-v6.13-zen1.patch
│   ├── x13s-bluetooth-fw.patch
│   └── x13s-camera.patch
└── template

```

You need to create the symbolik link :

`ln -s linux6.13-zen/ linux6.13-zen-headers`

![Captura de pantalla_20250104_134039](https://github.com/user-attachments/assets/286ceabd-ff31-4739-bc59-b465c93e5e7f)

#VOID MANUAL
https://github.com/void-linux/void-packages/blob/master/Manual.md
