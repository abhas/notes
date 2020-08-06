---
date: 2020-08-06
tags:
  - desktop
  - monitor
---

# Configuring your Ultra Wide monitor to work

To use an ultrawide monitor with an 21:9 aspect ratio at its native resolution of 2560x1080, run the following snippets on each boot:

```bash
#!/bin/bash

xrandr --newmode  "2560x1080x60.00" 185.58 2560 2624 2688 2784 \
  1080 1083 1093 1111
xrandr --addmode HDMI-1 2560x1080x60.00
xrandr --output HDMI-1 --mode 2560x1080x60.00
```

You need to change **`HDMI-1`** to match your connection. Eg: **`HDMI-2`** and **`DISPLAYPORT-0`**.

Thanks for this snippet, [Nishant](http://codemarauder.org/).