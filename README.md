# isoroot

先将kernel.img, rootfs.img文件拷贝到本目录，然后用如下命令创建可以启动的ISO镜像文件：    

    mkisofs -o nvs.iso -b isolinux/isolinux.bin -c isolinux/boot.cat -no-emul-boot -boot-load-size 4 -boot-info-table isoroot

