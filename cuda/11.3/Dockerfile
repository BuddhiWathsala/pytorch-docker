FROM nvidia/cuda:11.3.0-base-ubuntu20.04

RUN apt -y update
RUN apt -y install python3.9
RUN ln -sf /usr/bin/python3.9 /usr/bin/python3 
RUN apt -y install python3-pip
RUN pip install torch==1.12.0+cu113 torchvision==0.13.0+cu113 torchaudio==0.12.0 --extra-index-url https://download.pytorch.org/whl/cu113
RUN pip install pyg-lib torch-scatter torch-sparse -f https://data.pyg.org/whl/torch-1.12.0+cu113.html
RUN pip install torch-geometric==2.2.0
RUN pip install networkx==3.1
RUN pip install pyyaml==6.0
RUN pip install debugpy==1.6.3
