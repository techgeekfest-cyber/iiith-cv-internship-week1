# IIITH Computer Vision Internship – Week 1

This repository contains my submissions for Week 1 tasks of the IIITH Computer Vision Internship program.

## Task 1 – Extract Frames from Video

Downloaded a short-duration YouTube video and extracted frames using ffmpeg.

Sample command:

ffmpeg -i input_video.mp4 -vf fps=1 frame_%02d.png

Sample output frames are available in the task1/ directory.


## Task 2 – Generate Video from Frames

Extracted 1800 frames from a 1-minute clip at 30 fps and reconstructed a video using ffmpeg.

Commands used:

ffmpeg -i clip_1min.mp4 -vf fps=30 frames_%04d.png  
ffmpeg -framerate 30 -i frames_%04d.png reconstructed_video.mp4

Output video available in task2/.


## Task 3 – Merge Audio with Video

Trimmed a music clip to 1 minute duration and merged it with reconstructed video.

Commands used:

ffmpeg -i input_audio.mp3 -t 60 audio_1min.mp3  
ffmpeg -i final_video.mp4 -i audio_1min.mp3 -c:v copy -c:a aac video_with_audio.mp4

Final merged output available in task3/.
