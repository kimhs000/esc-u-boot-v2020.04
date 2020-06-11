# esc_uboot_v2020_04
mx6q/dl/s/spl esc u-boot v2020.04 
 
# Download repository
    git clone https://github.com/kimhs000/esc-uboot-v2020.04.git
    cd openrex-uboot-v2015.10
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make mx6qesc_config
    make
    cp u-boot.imx /tftp/uboot-mx6qesc.imx
 
# Build (imx6dl)
    TODO
 
# Build (imx6s)
    TODO
