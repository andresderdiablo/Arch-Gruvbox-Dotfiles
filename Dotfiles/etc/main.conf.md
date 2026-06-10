Modificar línea **```#ControllerMode = dual```** por:
```
ControllerMode = bredr
```

Modificar línea **```#AutoEnable=false```** por:
```
AutoEnable=true
```

---

Luego ejecutar en Terminal:
```
sudo systemctl restart bluetooth.service
```