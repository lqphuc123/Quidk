# Quidk - Text Summarization

**Quidk** is a summarization website for essays, scientific papers, thesis, web pages,... brings convenience in learning for students and teachers.

## Functionality

The website is capable of performing 2 kinds of text summarization tasks:

- By raw text:

![image](https://user-images.githubusercontent.com/58034112/167919156-3609cb40-9518-4f1b-ba84-98ff295f2971.png)

- By link embedded:

![image](https://user-images.githubusercontent.com/58034112/167920052-5d5d1668-ed36-4a81-b8bb-00581e640fa9.png)

***- NEW UPDATE: Add translate options for 2 languages: Vietnamese and English***

![image](https://user-images.githubusercontent.com/58034112/168003602-7b3db63f-db37-44fd-80a8-478994f6f561.png)

## Prerequisites
- [Flask](https://flask.palletsprojects.com/en/2.1.x/)
- [TensorFlow](https://www.tensorflow.org/)
- [PyTorch](https://pytorch.org/)
- [Beautiful Soup](https://realpython.com/beautiful-soup-web-scraper-python/)
- [Hugging Face Transformers](http://huggingface.co/docs/transformers)
- [Googletrans](https://py-googletrans.readthedocs.io/en/latest/)

## Installation

### Install Environment

You will need [Python 3.7 or later](https://www.python.org/downloads/) and [a C++14 compiler](https://osdn.net/projects/mingw/). Also, we highly recommend installing an [Anaconda](https://www.anaconda.com/distribution/#download-section) environment to get a high-quality BLAS library (MKL).

### Install Dependencies

All the libraries need for Botiris are in [requirements.txt](requirements.txt).</br>

Use `pip install -r .\requirements.txt` to install.

### Setup for discrete GPU (optional)

This program uses CPU by default. </br> We highly recommend using discrete GPU for the better performance.

If you want to run with **NVIDIA GPU** support, install:
- [NVIDIA CUDA](https://developer.nvidia.com/cuda-downloads) 10.2 or above.
- [NVIDIA cuDNN](https://developer.nvidia.com/cudnn) v7 or above.
- If you want to build on Windows, [Visual Studio 2017/2019 with MSVC toolset, and NVTX](https://visualstudio.microsoft.com/vs/older-downloads/) are also needed.
- [Compiler](https://gist.github.com/ax3l/9489132) compatible with CUDA.

or follow some tutorial videos for [Windows](https://youtu.be/hHWkvEcDBO0?t=50) or [Debian-based Linux distros](https://youtu.be/EFPxYotTwDI).

**_Note:_** You could refer to the [cuDNN Support Matrix](https://docs.nvidia.com/deeplearning/cudnn/pdf/cuDNN-Support-Matrix.pdf) for cuDNN versions with the various supported CUDA, CUDA driver and NVIDIA hardwares.

If you want to disable CUDA support, export the environment variable `USE_CUDA=0`.
Other potentially useful environment variables may be found in `tracking.py`.

If you want to run with **AMD GPU** support, install:
- [AMD ROCm](https://rocmdocs.amd.com/en/latest/Installation_Guide/Installation-Guide.html) 4.0 and above installation.
- ROCm is currently supported only for **Linux systems**.

or follow [this tutorial video](https://youtu.be/efKjfBkjPlM) for **Debian-based Linux distros**.

If you want to disable ROCm support, export the environment variable `USE_ROCM=0`.
Other potentially useful environment variables may be found in `tracking.py`.

**_CUDA and ROCm are not supported on macOS._**

**_After that_**, install [PyTorch](https://pytorch.org/get-started/locally/) via Conda or pip wheels.

**_Note:_** If you are building for NVIDIA's Jetson platforms (Jetson Nano, TX1, TX2, AGX Xavier), Instructions to install PyTorch for Jetson Nano are [available here](https://devtalk.nvidia.com/default/topic/1049071/jetson-nano/pytorch-for-jetson-nano/) or you can follow [tutorial video](https://youtu.be/UiZaM-Wbc6A).

## Running the tests

Use `python .\run.py` to run the website.</br>

Default address: http://127.0.0.1:5000

## Acknowledgments
- [AI Blog Post Summarization with Hugging Face Transformers & Beautiful Soup Web Scraping](https://youtu.be/JctmnczWg0U)
- [Google Translate API with Python](https://www.youtube.com/watch?v=VIc_DDBpE7U)

## Credits
[Le Quang Phuc](https://www.facebook.com/phuc.lequang.9081/)</br>
[Huynh Tan Phuc](https://www.facebook.com/HtPuc)

## Feedback and contributions

If you have a feature request or run into issues using the website, please [fill an issue](https://github.com/lqphuc123/Quidk/issues).</br>
Thank you for your contributing.

## License

Quidk has a MIT license, as found in the [LICENSE](LICENSE) file.
