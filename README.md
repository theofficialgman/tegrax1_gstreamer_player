# tegrax1_gstreamer_player

Tegra Gstreamer video player still in the works
Don't expect great compatibility or reliability

Run the player as seen below for youtube videos

./mp4_player_best_vp9 $(youtube-dl --format "bestvideo[vcodec=vp9][height<=?1080][protocol=https]+bestaudio[ext=m4a][protocol=https]" --get-url https://www.youtube.com/watch?v=Y8fiOMU-dQQ)
