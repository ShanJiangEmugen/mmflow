MMFlow cmd 

run demo:
python demo/video_demo.py demo/demo.mp4 \
    configs/raft/raft_8x2_100k_mixed_368x768.py \
    checkpoints/raft_8x2_100k_mixed_368x768.pth \
    raft_demo.mp4 --gt demo/demo_gt.mp4
    
custom videos:
python demo/video_demo.py {video_input.mp4} \
    configs/raft/raft_8x2_100k_mixed_368x768.py \
    checkpoints/raft_8x2_100k_mixed_368x768.pth \
    {output_fn.mp4}
