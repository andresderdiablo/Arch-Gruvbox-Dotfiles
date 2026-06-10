```
polkit.addRule(function(action, subject) {
    if (action.id == "com.ubuntu.pkexec.lightdm-gtk-greeter-settings" &&
        subject.isInGroup("wheel")) {
        return polkit.Result.YES;
    }
});
```
