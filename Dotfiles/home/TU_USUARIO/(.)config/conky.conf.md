NOTA: Cambia la configuración de localización en la sección del clima según tu ubicación preferida.

```
conky.config = {
    alignment = 'bottom_right',
    gap_x = 20,
    gap_y = -15,
    minimum_width = 210,       
    minimum_height = 225,
    
    background = true,
    border_width = 0,
    cpu_avg_samples = 2,
    default_color = '#D4BE98',
    double_buffer = true,
    draw_borders = false,
    draw_graph_borders = false,
    draw_outline = false,
    draw_shades = false,
    
    font = 'JetBrains Mono Nerd Font:size=9',
    
    net_avg_samples = 2,
    no_buffers = true,
    out_to_console = false,
    out_to_ncurses = false,
    out_to_stderr = false,
    out_to_x = true,
    
    own_window = true,
    own_window_class = 'Conky',
    own_window_type = 'desktop',
    own_window_transparent = true,
    own_window_argb_visual = true,
    own_window_argb_value = 0,
    own_window_hints = 'undecorated,below,sticky,skip_taskbar,skip_pager',
    
    update_interval = 2.0,
    use_xft = true,
}

conky.text = [[
${goto 19}╭───────────────────────────╮
${goto 19}│ ${goto 35} ${goto 53}CPU ${goto 185}${cpu cpu0}%${goto 215}│
${goto 19}│ ${goto 35}${cpubar 2,170}${goto 215}│
${goto 19}│ ${goto 35} ${goto 53}RAM ${goto 185}${memperc}%${goto 215}│
${goto 19}│ ${goto 35}${membar 2,170}${goto 215}│
${goto 19}│ ${goto 35}󰋊${goto 53}HDD ${goto 185}${fs_used_perc /}%${goto 215}│
${goto 19}│ ${goto 35}${fs_bar 2,170 /}${goto 215}│
${goto 19}╰───────────────────────────╯
${voffset -20}
${goto 19}╭───────────────────────────╮
${goto 19}│ ${goto 35}${goto 53}Mérida, VE${goto 140}󰖞 ${execi 900 curl -s "https://api.open-meteo.com/v1/forecast?latitude=8.5983&longitude=-71.1449&current=temperature_2m,relative_humidity_2m,wind_speed_10m" | jq -r '.current.relative_humidity_2m'}%${goto 215}│
${goto 19}│ ${goto 35}${goto 53}${execi 900 curl -s "https://api.open-meteo.com/v1/forecast?latitude=8.5983&longitude=-71.1449&current=temperature_2m,relative_humidity_2m,wind_speed_10m" | jq -r '.current.temperature_2m | round' | tr -d '\n'}°C${font}${goto 140}󰖝 ${execi 900 curl -s "https://api.open-meteo.com/v1/forecast?latitude=8.5983&longitude=-71.1449&current=temperature_2m,relative_humidity_2m,wind_speed_10m" | jq -r '.current.wind_speed_10m' | tr -d '\n'}km/h${goto 215}│
${goto 19}╰───────────────────────────╯
]]
```
