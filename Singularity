Bootstrap: docker
From: pytorch/pytorch:1.3-cuda10.1-cudnn7-runtime

%post

    apt-get update
    apt-get install -y libsndfile1
    apt-get install -y ffmpeg
    
    pip install audioread audiomate
