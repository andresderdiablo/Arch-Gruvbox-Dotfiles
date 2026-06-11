```
{
    "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",
    "logo": {
        "type": "none"
    },
    "display": {
        "separator": " "
    },
    "modules": [
        // ================= SECTION 1: LOGO + HARDWARE =================
        {
            "type": "custom",
            "format": "                    {#36}/\\              {#cyan}╭─────┬──────────{#bright_cyan}「 Hardware 」───────────╮"
        },
        {
            "type": "host",
            "key": "     {#90}  {#31}          {#36}/  \\             {#cyan}󰌢 PC:",
            "keyColor": "cyan"
        },
        {
            "type": "cpu",
            "key": "     {#32}  {#33}         {#36}/    \\            {#cyan}│ ├─󰻠 :",
            "keyColor": "cyan"
        },
        {
            "type": "gpu",
            "key": "     {#34}  {#35}        {#36}/      \\           {#cyan}│ ├─󰍛 :",
            "keyColor": "cyan"
        },
        {
            "type": "disk",
            "key": "     {#36}  {#37}       {#36}/   ,,   \\          {#cyan}│ ├─󰋊 :",
            "keyColor": "cyan"
        },
        {
            "type": "memory",
            "key": "     {#38}  {#39}      {#36}/   |  |   \\         {#cyan}└ ╰─ :",
            "keyColor": "cyan"
        },
        {
            "type": "custom",
            "format": "              {#36}/_-''    ''-_\\        {#cyan}╰─────┴───────────────────────────────────╯"
        },
        "break",
        // ================= SECTION 2: SOFTWARE + RICE =================
        {
            "type": "custom",
            "format": "  {#red}╭─────┬────{#bright_red}「 Software 」────╮"
        },
        {
            "type": "os",
            "key": "  󰣇 SO:",
            "keyColor": "red"
        },
        {
            "type": "title",
            "key": "  │ ├─ :",
            "format": "{#green}{user-name}{#red}@{#blue}{host-name}",
            "keyColor": "red"
        },
        {
            "type": "de",
            "key": "  │ ├─ :",
            "keyColor": "red"
        },
        {
            "type": "lm",
            "key": "  │ ├─󰧨 :",
            "keyColor": "red"
        },
        {
            "type": "shell",
            "key": "  └ ╰─ :",
            "keyColor": "red"
        },
        {
            "type": "custom",
            "key": "  {#red}╰─────┴──────────────────────╯"
        },
        {
            "type": "custom",
            "format": "  \u001b[7A\u001b[34C{#magenta}╭─────┬────────────{#bright_magenta}「 Rice 」─────────────╮"
        },
        {
            "type": "theme",
            "key": "  \u001b[34C󰉼 TM:",
            "keyColor": "magenta"
        },
        {
            "type": "icons",
            "key": "  \u001b[34C│ ├─󰀻 :",
            "keyColor": "magenta"
        },
        {
            "type": "cursor",
            "key": "  \u001b[34C│ ├─󰆽 :",
            "keyColor": "magenta"
        },
        {
            "type": "font",
            "key": "  \u001b[34C│ ├─ :",
            "keyColor": "magenta"
        },
        {
            "type": "disk",
            "key": "  \u001b[34C{#magenta}└ ╰─ :",
            "folders": "/",
            "format": "{create-time:10} [{days} days]"
        },
        {
            "type": "custom",
            "key": "  \u001b[34C{#magenta}╰─────┴───────────────────────────────────╯"
        },
        "break",
    ]
}

```