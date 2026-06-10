```
polkit.addRule(function(action, subject) {
    if ((action.id == "org.opensuse.cupspkhelper.mechanism.server-settings" ||
         action.id == "org.opensuse.cupspkhelper.mechanism.printer-enable" ||
         action.id == "org.opensuse.cupspkhelper.mechanism.printer-local-edit") &&
        subject.isInGroup("wheel")) {
        return polkit.Result.YES;
    }
});
```