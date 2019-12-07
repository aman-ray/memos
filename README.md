# memos

## openvino-docker
https://github.com/mateoguzman/openvino-docker

## Miniconda
wget https://repo.continuum.io/miniconda/Miniconda3-4.7.12-Linux-x86_64.sh
bash Miniconda3-4.7.12-Linux-x86_64.sh

## intel python
https://www.isus.jp/products/python-distribution/using-intel-distribution-for-python-with-anaconda/

conda update conda
conda config --add channels intel
conda create -n idp intelpython3_full python=3.6.8
source activate idp
conda install sympy
conda install affine
export ACCEPT_INTEL_PYTHON_EULA=yes
conda install numpy -c intel --no-update-deps

## docker 
### intel python
https://software.intel.com/en-us/articles/docker-images-for-intel-python
docker pull intelpython/intelpython3_full
docker run -it intelpython/intelpython3_full

docker start 1f67861419ca
docker exec -it 1f67861419ca bash

# openvino
wget http://registrationcenter-download.intel.com/akdlm/irc_nas/16057/l_openvino_toolkit_p_2019.3.376.tgz
tar -xf l_openvino_toolkit*
cd l_openvino_toolkit_p_2019.3.376
apt-get update && apt-get -y upgrade && apt-get autoremove -y



