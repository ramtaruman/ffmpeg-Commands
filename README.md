# ffmpeg-Commands
Quick rundown of some ffmpeg commands I found personally useful. Also some extrapolation of certain useful functionalities.


# Image + Audio = Video
```powershell
ffmpeg -loop 1 -i ima.jpg -i audio.wav -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest out.mp4
```