Bootstrap: docker
From: pytorch/pytorch:1.3-cuda10.1-cudnn7-runtime

%post

    apt-get update
    apt-get install -y libasound-dev portaudio19-dev libportaudio2 libportaudiocpp0 ffmpeg libav-tools libmp3lame0 libavcodec-extra
    apt-get install -y libsndfile1
    
    echo $PATH
    ls /opt/conda/bin/
    
    export PATH = /opt/conda/bin:$PATH

    conda install -c anaconda pip 
    
    pip install audiomate librosa
