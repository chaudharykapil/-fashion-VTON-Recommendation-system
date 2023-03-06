# fashion-VTON-Recommendation-system
## Python Version :- 3.10.9 (base conda)
## Steps :-
#
## Library Installation

conda install pytorch=0.4.1 torchvision=0.2.1 -c pytorch \
pip install -r requirements.txt
#
## Prepare Dataset
download zip file from https://1drv.ms/u/s!Ai8t8GAHdzVUiQRFmTPrtrAy0ZP5?e=rS1aK8
and unzip to "data" folder 

Download the pre-trained models from here: https://1drv.ms/u/s!Ai8t8GAHdzVUiQA-o3C7cnrfGN6O?e=EaRiFP
and replace your "checkpoints" folder with "checkpoints" folder inside downloaded zip file

Download pre-train Model for recommendation system from : https://drive.google.com/file/d/1CedoKtVbQ7OIrrlSCE7AeElMntYQRAAS/view?usp=share_link

unzip the file inside "static" folder


#
## Run the following command in root folder
### python cp-vton-plus/test.py --name GMM --stage GMM --workers 4 --datamode test --result_dir static/vton/out --data_list test_pairs.txt --checkpoint checkpoints/GMM/gmm_final.pth
# 
"warp-cloth" and "warp-mask" folders inside the "static/vton/out/GMM/test/" directory. Copy the "warp-cloth" and "warp-mask" folders into your data directory, for example inside "data/test" folder.
#
## run app.py file to start local server
All cloth images are inside cloth folder and all model images are inside image folder in your root folder 
#

for training your own model please refer : https://github.com/minar09/cp-vton-plus

