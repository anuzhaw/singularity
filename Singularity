Bootstrap: docker
From: pytorch/pytorch:1.3-cuda10.1-cudnn7-runtime

%post

    apt-get update
    apt-get install -y libasound-dev portaudio19-dev libportaudio2 libportaudiocpp0 ffmpeg libav-tools libmp3lame0 libavcodec-extra
    apt-get install -y libsndfile1
    
    echo 'export PATH=/opt/conda/bin:$PATH' >>$SINGULARITY_ENVIRONMENT

    
    CMAKE_PREFIX_PATH="$(dirname $(which conda))/../" pip install audiomate librosa
