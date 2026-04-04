# Task 3 – Merge Audio with Video

Trimmed audio to 1 minute duration:

ffmpeg -i input_audio.mp3 -t 60 audio_1min.mp3

Merged trimmed audio with reconstructed video:

ffmpeg -i final_video.mp4 -i audio_1min.mp3 -c:v copy -c:a aac video_with_audio.mp4
