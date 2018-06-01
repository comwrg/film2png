# film2png
```bash

#!/bin/sh

for i in `seq -w 0 7200`
do
    mplayer -ss $i -noframedrop -nosound -vo png:z=9 -frames 1 Kimi.No.Na.Wa.2016.1080p.1080p.BluRay.x264.DTS-HDC.mkv
    mv 00000001.png $i.png
done
```
