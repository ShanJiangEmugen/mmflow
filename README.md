# MMFlow
Forked from OpenMMLab --> this repo will automaticly update when original aurthers make changes!
    
Great for GPU accelarated Optical Flow calculations    

## Usage
- Demo:

```
python demo/video_demo.py demo/demo.mp4 \
    configs/raft/raft_8x2_100k_mixed_368x768.py \
    checkpoints/raft_8x2_100k_mixed_368x768.pth \
    raft_demo.mp4 --gt demo/demo_gt.mp4
```

- on custome data/videos:
```
python demo/video_demo.py {video_input.mp4} \
    configs/raft/raft_8x2_100k_mixed_368x768.py \
    checkpoints/raft_8x2_100k_mixed_368x768.pth \
    {output_fn.mp4}
```

This algorithm takes lots of Memory in both RAM and GPU!    
    
Try to split input videos in to smaller pieces, so that they can fit in the limited resources!
    
A 5 minutes video could fit in perfect in my setting:
- 10900X
- 32GB * 2 RAM
- RTX 3080Ti 12GB * 2 --> not sure if I can use both for the same task
