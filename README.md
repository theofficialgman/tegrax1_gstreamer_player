# tegrax1_gstreamer_player

Tegra Gstreamer video player still in the works
Don't expect great compatibility or reliability

Run the player as seen below for youtube videos

```./mp4_player_best_vp9 $(youtube-dl --format "bestvideo[vcodec=vp9][height<=?1080][protocol=https]+bestaudio[ext=webm][protocol=https]" --get-url https://www.youtube.com/watch?v=Y8fiOMU-dQQ)```

Compile as below
``` gcc mp4_player_best_vp9.c -o mp4_player_best_vp9 `pkg-config --cflags --libs gstreamer-video-1.0 gtk+-3.0 gstreamer-1.0` ```
