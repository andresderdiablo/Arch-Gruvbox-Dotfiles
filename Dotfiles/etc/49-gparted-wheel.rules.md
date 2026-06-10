```
polkit.addRule(function(action, subject) {
    if (action.id == "org.gnome.gparted" &&
        subject.isInGroup("wheel")) {
        return polkit.Result.YES;
    }
});
```