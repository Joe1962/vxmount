vxmount (previously vl-hot) is a purely udev based automount system for any kind of pluggable storage device that conforms to the mass storage device specification and so uses scsi emulation. It was officially included in Vector Linux 5.1 SOHO and subsequent releases. Hardware known to work with vxmount are USB pendrives, hard disks, digital cameras and memory card readers, PCCARD (or PCMCIA) memory cards and drives; Firewire devices should work, but there are no user reports on this kind of hardware yet.

Working specifications of vxmount:
- The mount base directory will be "/mnt/vl-hot/".
- Each drive will have a "sd?" directory (where "?" represents a letter of the alphabet).
- Each mounted partition will have a "vol#" directory (where "#" represents a number) within the drive directory. An exception to this rule is in the case of non-MBR devices, where there is no partition table.
- Desktop icons are dynamically created/deleted (currently only for KDE) and these have unmount options in the context (right-click) menu. There is a conventional unmount (should be used normally) as well as options for unmount with signalling to the process that is holding open the mount and unmount with killing of said process (the last two should be tried in that order, when the normal unmount fails).
- The unmount operation has completed succesfully once the desktop icon dissapears.

