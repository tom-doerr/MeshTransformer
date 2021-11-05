#from nvidia/cuda:10.1-cudnn7-devel-ubuntu18.04
#from ubuntu:20.04
from nvidia/cuda:11.4.2-cudnn8-devel-ubuntu20.04

# Disable interactive input.
env DEBIAN_FRONTEND=noninteractive


run apt-get update && apt-get install -y \
    git

run git clone https://github.com/NVIDIA/apex.git



#run apt-get update && apt-get install -y \
    #python3 \
    #python3-pip


run apt install -y software-properties-common
run add-apt-repository ppa:deadsnakes/ppa
run apt update
run apt install -y python3.7
run apt install -y python3-pip

run python3 --version




run pip3 install torch==1.4.0

# install zlib
run apt-get install -y zlib1g-dev

# install libjpeg
run apt-get install -y libjpeg-dev



run pip3 install torchvision==0.5.0
#run pip3 install numpy

#run cd apex && python3 setup.py install --cuda_ext --cpp_ext
run pip3 install matplotlib

run git clone --recursive https://github.com/microsoft/MeshTransformer.git
run cd MeshTransformer && python3 setup.py build develop && pip3 install -r requirements.txt

run cd MeshTransformer && pip install ./manopth/.

RUN apt-get install ffmpeg libsm6 libxext6 -y

run apt-get install libosmesa6-dev -y
#run apt-get install libglu1-mesa-dev -y


run pip3 install opendr


