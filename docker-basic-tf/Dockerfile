FROM python:3.6

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN apt-get install -y curl
RUN apt-get install -y unzip
RUN apt-get install -y build-essential
RUN apt-get install -y libfreetype6-dev
RUN apt-get install -y libhdf5-serial-dev
RUN apt-get install -y libpng-dev
RUN apt-get install -y libzmq3-dev
RUN apt-get install -y pkg-config
RUN apt-get install -y vim
RUN apt-get install wget
RUN apt-get -y install python3-pip

RUN pip3 install dill
RUN pip3 install ipykernel
RUN pip3 install jupyter
RUN pip3 install keras 
RUN pip3 install matplotlib
RUN pip3 install mpld3 
RUN pip3 install natsort
RUN pip3 install numpy
RUN pip3 install pandas
RUN pip3 install plotly
RUN pip3 install sklearn   
RUN pip3 install tensorflow
RUN pip3 install tqdm
RUN pip3 install utils
RUN python3 -m ipykernel.kernelspec

# For Jupyter notebook
EXPOSE 8888

CMD bash

