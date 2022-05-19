Execution

Put .jpg files (e.g., test.jpg) into the image folder or you can modified the extension in yml file like .PNG, .JPEG
  E.g., image/moon.jpg

Run the following command
  python main.py --config argument.yml

Corresponding depth map estimated by MiDaS
  E.g. depth/moon.npy, depth/moon.png

Inpainted 3D mesh (Optional: User need to switch on the flag save_ply)
  E.g. mesh/moon.ply
  
Rendered videos with more then 15+ effects in the same result folder.

For Python dependencies listed in requirements.txt
  To get started, please run the following commands:
  conda create -n 3DP python=3.7 anaconda
  conda activate 3DP
  pip install -r requirements.txt
  conda install pytorch==1.4.0 torchvision==0.5.0 cudatoolkit==10.1.243 -c pytorch

Next, please download the model weight using the following command:
  chmod +x download.sh
  ./download.sh
  
  
Acknowledgments
We thank Pratul Srinivasan for providing clarification of the method Srinivasan et al. CVPR 2019.
We thank the author of Zhou et al. 2018, Choi et al. 2019, Mildenhall et al. 2019, Srinivasan et al. 2019, Wiles et al. 2020, Niklaus et al. 2019 for providing their implementations online.
Our code builds upon EdgeConnect, MiDaS and pytorch-inpainting-with-partial-conv
