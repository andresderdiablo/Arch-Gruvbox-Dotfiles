```
polkit.addRule(function(action, subject) {
    if (action.id == "org.freedesktop.policykit.exec") {
        var program = action.lookup("program");
        if ((program === "/usr/sbin/bitmask-root" || program === "/usr/bin/bitmask-root") &&
            subject.isInGroup("wheel")) {
            return polkit.Result.YES;
        }
    }
});
```