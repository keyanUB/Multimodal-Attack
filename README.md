# Robustness of Multimodal Learning in an Adversarial Setting

The code provided in this repository is for MUROAN on MMBT-Hateful Memes

We first need to download `jsonlines` and the specified versions of `torch` and `torchvision` , before installing mmf (causes an issue). 
They python version may cause issue, the python version we are using is `Python 3.7.15`
```python
pip install jsonlines torch==1.6.0 torchvision==0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
```

Then, we need to clone the Facebook MMF framework
```c
git clone --branch no_feats --config core.symlinks=true https://github.com/rizavelioglu/mmf.git
```

Please cd into the `mmf` directory and run the following command to set up the environment
```c
cd mmf
```
```python
pip install --editable .
```

Next, let's place the folders `data` and `occluded_samples` and python scripts `occlusion_test.py` and `occlusion_finctions.py` in the `mmf` directory. 

Also, we need to replace the file `mmf/mmf/models/interfaces/mmbt.py` with our `mmbt.py`

Now, you can run the mutimodal attack through the follow command:
```python
python occlusion_test.py
```
