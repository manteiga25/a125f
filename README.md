# rainbow-a125f
building rainbow kernel with proton clang
$ export ARCH=arm64
$ export SUBARCH=arm64
$ export HEADER_ARCH=arm64
$ export PATH="$HOME/pwd:$PATH"
$ export STRIP="$HOME/pwd/strip"
$ export CROSS_COMPILE=/pwd/aarch64-linux-gnu-
$ export CROSS_COMPILE_COMPAT=/pwd/arm-linux-gnueabi-
$ export ANDROID_MAJOR_VERSION=r
$ make -C $(pwd) O=$(pwd)/out KCFLAGS=-w CONFIG_SECTION_MISMATCH_WARN_ONLY=y CC=/pwd/clang LLVM=/pwd/1 LLVM_IAS=/pwd/1 rainbow_defconfig
$ make -C $(pwd) O=$(pwd)/out KCFLAGS=-w CONFIG_SECTION_MISMATCH_WARN_ONLY=y CC=/pwd/clang LLVM=/pwd/1 LLVM_IAS=/pwd/1 nconfig
$ make -C $(pwd) O=$(pwd)/out KCFLAGS=-w CONFIG_SECTION_MISMATCH_WARN_ONLY=y CC=/pwd/clang LLVM=/pwd/1 LLVM_IAS=/pwd/1 -j8
