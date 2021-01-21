# Realtek wifi driver
- we going to  install wifi drivers from github
*Note : if the error like command not found then follow 
```
$ sudo apt install command // write your command space of command
```

- follow these step

```
$ git clone https://github.com/kelebek333/rtl8188fu.git
$ cd rtl8188fu
$ make 
$ sudo make install
```

-Then, if there's the following problem:

```
$ make
make ARCH=x86_64 CROSS_COMPILE= -C /lib/modules/4.15.0-20-generic/build M=/home/^/rtl8188fu  modules
make[1]: Entering directory '/usr/src/linux-headers-4.15.0-20-generic'
Makefile:976: "Cannot use CONFIG_STACK_VALIDATION=y, please install libelf-dev, libelf-devel or elfutils-libelf-devel"
  CC [M]  /home/^/rtl8188fu/core/rtw_cmd.o
  CC [M]  /home/^/rtl8188fu/core/rtw_security.o
  CC [M]  /home/^/rtl8188fu/core/rtw_debug.o
  CC [M]  /home/^/rtl8188fu/core/rtw_io.o
  CC [M]  /home/^/rtl8188fu/core/rtw_ioctl_query.o
  CC [M]  /home/^/rtl8188fu/core/rtw_ioctl_set.o
  CC [M]  /home/^/rtl8188fu/core/rtw_ieee80211.o
  CC [M]  /home/^/rtl8188fu/core/rtw_mlme.o
  CC [M]  /home/^/rtl8188fu/core/rtw_mlme_ext.o
  CC [M]  /home/^/rtl8188fu/core/rtw_wlan_util.o
  CC [M]  /home/^/rtl8188fu/core/rtw_vht.o
  CC [M]  /home/^/rtl8188fu/core/rtw_pwrctrl.o
  CC [M]  /home/^/rtl8188fu/core/rtw_rf.o
  CC [M]  /home/^/rtl8188fu/core/rtw_recv.o
  CC [M]  /home/^/rtl8188fu/core/rtw_sta_mgt.o
  CC [M]  /home/^/rtl8188fu/core/rtw_ap.o
  CC [M]  /home/^/rtl8188fu/core/rtw_xmit.o
  CC [M]  /home/^/rtl8188fu/core/rtw_p2p.o
  CC [M]  /home/^/rtl8188fu/core/rtw_tdls.o
  CC [M]  /home/^/rtl8188fu/core/rtw_br_ext.o
  CC [M]  /home/^/rtl8188fu/core/rtw_iol.o
  CC [M]  /home/^/rtl8188fu/core/rtw_sreset.o
  CC [M]  /home/^/rtl8188fu/core/rtw_btcoex.o
  CC [M]  /home/^/rtl8188fu/core/rtw_beamforming.o
  CC [M]  /home/^/rtl8188fu/core/rtw_odm.o
  CC [M]  /home/^/rtl8188fu/core/efuse/rtw_efuse.o
  CC [M]  /home/^/rtl8188fu/os_dep/osdep_service.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/os_intfs.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/usb_intf.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/usb_ops_linux.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/ioctl_linux.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/xmit_linux.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/mlme_linux.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/recv_linux.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/ioctl_cfg80211.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/wifi_regd.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/rtw_proc.o
  CC [M]  /home/^/rtl8188fu/os_dep/linux/ioctl_mp.o
  CC [M]  /home/^/rtl8188fu/hal/hal_intf.o
  CC [M]  /home/^/rtl8188fu/hal/hal_com.o
  CC [M]  /home/^/rtl8188fu/hal/hal_com_phycfg.o
  CC [M]  /home/^/rtl8188fu/hal/hal_phy.o
  CC [M]  /home/^/rtl8188fu/hal/hal_dm.o
  CC [M]  /home/^/rtl8188fu/hal/hal_btcoex.o
  CC [M]  /home/^/rtl8188fu/hal/hal_mp.o
  CC [M]  /home/^/rtl8188fu/hal/hal_hci/hal_usb.o
  CC [M]  /home/^/rtl8188fu/hal/led/hal_usb_led.o
  CC [M]  /home/^/rtl8188fu/hal/HalPwrSeqCmd.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/Hal8188FPwrSeq.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_sreset.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_hal_init.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_phycfg.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_rf6052.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_dm.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_rxdesc.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/rtl8188f_cmd.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/usb/usb_halinit.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/usb/rtl8188fu_led.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/usb/rtl8188fu_xmit.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/usb/rtl8188fu_recv.o
  CC [M]  /home/^/rtl8188fu/hal/rtl8188f/usb/usb_ops.o
  CC [M]  /home/^/rtl8188fu/hal/efuse/rtl8188f/HalEfuseMask8188F_USB.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_debug.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_antdiv.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_antdect.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_interface.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_hwconfig.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/halphyrf_ce.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_edcaturbocheck.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_dig.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_pathdiv.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_rainfo.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_dynamicbbpowersaving.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_powertracking_ce.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_dynamictxpower.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_adaptivity.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_cfotracking.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_noisemonitor.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_acs.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/phydm_beamforming.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/txbf/halcomtxbf.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/txbf/haltxbfinterface.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/halhwimg8188f_bb.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/halhwimg8188f_mac.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/halhwimg8188f_rf.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/halhwimg8188f_fw.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/phydm_regconfig8188f.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/halphyrf_8188f.o
  CC [M]  /home/^/rtl8188fu/hal/phydm/rtl8188f/phydm_rtl8188f.o
  CC [M]  /home/^/rtl8188fu/core/rtw_mp.o
  CC [M]  /home/^/rtl8188fu/core/rtw_mp_ioctl.o
  LD [M]  /home/^/rtl8188fu/rtl8188fu.o
  Building modules, stage 2.
  MODPOST 1 modules
  CC      /home/^/rtl8188fu/rtl8188fu.mod.o
  LD [M]  /home/^/rtl8188fu/rtl8188fu.ko
make[1]: Leaving directory '/usr/src/linux-headers-4.15.0-20-generic'
```

- That will probably generate the following:
```
$ sudo make install
install -p -m 644 .ko  /lib/modules/4.15.0-20-generic/kernel/drivers/net/wireless/
install: cannot stat '.ko': No such file or directory
Makefile:481: recipe for target 'install' failed
make: *** [install] Error 1
```
Do:
```
sudo apt install libelf-dev
```
Then:
```
cd rtl8188fu
make clean
cd
sudo dkms add ./rtl8188fu
sudo dkms install rtl8188fu/1.0
```

Now, reboot. Your Wi-Fi should now be working!

Thanks a lot and all the best!
