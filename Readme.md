### Apple M3 Max - AI with MLX

GApple delivery MLX yesterday, it is a framework to help to run Numpy, Pytorch and others using Macbook Pro but kind Silicon.


#### Docs

mlx -> https://developer.apple.com/metal/pytorch/


#### How to install?


	curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
	sh Miniconda3-latest-MacOSX-arm64.sh



	conda install pytorch torchvision torchaudio -c pytorch-nightly


#### To Test

	import torch
	if torch.backends.mps.is_available():
	    mps_device = torch.device("mps")
	    x = torch.ones(1, device=mps_device)
	    print (x)
	else:
	    print ("MPS device not found.")
