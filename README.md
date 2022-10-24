# Robustness of Multimodal Learning in an Adversarial Setting

The code provided in this repository is for MDA on MMBT-Hateful Memes

We first need to download the specified versions of `torch` and `torchvision` and jsonlines, before installing mmf (causes an issue). 
They python version may also cause issue, the python version we are using is Python 3.7.15

```python
pip install jsonlines torch==1.6.0 torchvision==0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
```

Please cd into the mmf directory and run the following command to set up the environment
```c
cd Multimodal-Attack/mmf
```
```python
pip install --editable .
```

Now, you can run the mutimodal attack through the follow command:
```python
python occlusion_test.py
```
