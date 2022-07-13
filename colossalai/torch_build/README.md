# Torch Build

This folder contains all the official PyTorch distributions for different CUDA and PyThon versions. 
All the URLs to the torch build files will be put in the `wheel_urls` folders. Each text file is with respect to a particular combination of PyTorch and CUDA. The format of the text file name will be `<torch-version>-cuda<cuda-version>`. Only the torch versions with the highest revision number, will be kept. For example, we only keep v1.8.1 and ignore v1.8.0 for torch 1.8. The format of each line in the text file will be `<pip/conda> <wheel-url> <python-version> <conda-flags>. The <conda-flags> is only present if we use conda install and the flags are joined by `+` into one string.