# ffmpeg-Commands
Quick rundown of some ffmpeg commands I found personally useful. Also some extrapolation of certain useful functionalities.


## Image + Audio = Video
```powershell
ffmpeg -loop 1 -i img.png -i in.mp3 -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest out.mp4
```
## compresses input video (mp4)
```powershell
ffmpeg -i input.mp4 -vcodec libx265 -crf 28 output.mp4
```
