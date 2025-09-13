# Router (imx6ull + OpenWrt)

本仓库提供基于 **imx6ull 开发板** 的 OpenWrt 路由器实现所需的文件与资源。  
相关文件已经过测试，可以直接使用。如需详细编译及移植过程，请参考配套技术文档。  

---

## 📂 文件说明

- **openwrt-19.07.7.tar.gz**  
  OpenWrt 19.07 源码压缩包

- **rootfs.tar.bz2**  
  OpenWrt 编译生成的根文件系统 (rootfs)

- **zImage**  
  OpenWrt 编译生成的 Linux 内核镜像  
  （使用开发板自带内核进行编译）

- **openwrt-imx6-imx6ull-14x14-emmc-4.3-800x480-c.dtb**  
  OpenWrt 编译生成的设备树文件 (DTB)

- **u-boot-imx6ull-14x14-ddr512-emmc.imx**  
  开发板原厂 U-Boot 文件（非 OpenWrt 编译产生）

---

## 🔧 使用说明

1. 准备好 imx6ull 开发板。  
2. 使用仓库中提供的 **u-boot** 或开发板原装的 u-boot。  
3. 烧录流程：  
   - 使用 `zImage`、`rootfs.tar.bz2` 与 `dtb` 文件启动系统  
   - 通过 u-boot 配置启动参数  
   - 加载并运行 OpenWrt  
4. 进入系统后即可使用 OpenWrt 的路由功能。

---

## 📖 技术文档

详细编译过程、启动配置与调试方法，请查阅随附的 **技术文档**。  
