## A Cut Above The Rest
### Analyzing the Impact of Shot Detection Algorithms on the Quality of Chunk Encoded Videos

I read [this post about the Dynamic Optimizer](https://netflixtechblog.com/dynamic-optimizer-a-perceptual-video-encoding-optimization-framework-e19f1e3a277f) from Netflix's engineering blog. Dynamic optimizer is a framework for optimizing video encoding, which relies on, ammong other things, chunk based encoding.

The question with this project is, how important is it to detect accurate shot transitions when splitting videos into chunks for encoding?
This study examines whether suboptimal shot detection, such as failing to capture a hard shift with SAD or HD, significantly affects the final encoded video's quality.

This project uses simulated video files processed through both SAD and ECR shot detection algorithms and encoded with Google's VP9 codec, and final video quality is measured by and compared using Video Multi-method Assessment Fusion (VMAF) scores.

