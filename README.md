# milan85board_uboot_v2015_10
mx6q/dl/s/spl milan85board u-boot v2015.10 
 
# Download repository
    git clone https://github.com/Miian85-FedevelLinuxCourse/milan85board-uboot-v2015.10.git
    cd milan85board-uboot-v2015.10
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make mx6qmilan85board_config
    make
    cp u-boot.imx /tftp/uboot-mx6qopenrex.imx
 
# Build (imx6dl)
    Will not be used
 
# Build (imx6s)
    Will not be used
