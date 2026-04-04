# Task 2 – Frame Reconstruction Video

Extracted 1800 frames from a 1-minute video clip at 30 fps using ffmpeg.

Command used:

ffmpeg -i clip_1min.mp4 -vf fps=30 frames_%04d.png

Reconstructed video from frames:

ffmpeg -framerate 30 -i frames_%04d.png reconstructed_video.mp4
