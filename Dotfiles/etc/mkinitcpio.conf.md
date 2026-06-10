Modificar línea **```HOOKS=(...)```** por:
```
HOOKS=(base udev plymouth autodetect microcode modconf kms keyboard keymap consolefont block filesystems fsck)
```

---

Luego ejecutar en Terminal:
```
sudo mkinitcpio -P
```