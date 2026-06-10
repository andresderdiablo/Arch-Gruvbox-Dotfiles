```
polkit.addRule(function(action, subject) {
    if (action.id == "in.teejeetech.pkexec.timeshift-gtk" &&
        subject.isInGroup("wheel")) {
        return polkit.Result.YES;
    }
});
```
