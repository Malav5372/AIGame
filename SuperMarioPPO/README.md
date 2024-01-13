![giphy](https://github.com/Malav5372/SuperMarioPPO/assets/144440737/f0db61b8-0e8e-410f-8ce3-5e59ca0e66fb)

### Introduction

Implemented with Proximal Policy Optimization (PPO), my Python source code showcases the application of AI in mastering Super Mario Bros. The focus lies on training an agent through the PPO algorithm as detailed in the Proximal Policy Optimization Algorithms paper. The agent's performance is notable, successfully completing 31 out of 32 levels, exceeding initial expectations. This achievement highlights the efficacy of AI in gaming scenarios.

### Refer
Proximal Policy Optimization (PPO) algorithm introduced in the paper **Proximal Policy Optimization Algorithms** [paper](https://arxiv.org/abs/1707.06347).



## PPO in SuperMarioBros in action : 

<p align="left">
  <img src="demo/video-1-1.gif" width="250">
  <img src="demo/video-1-2.gif" width="250">
  <img src="demo/video-1-3.gif" width="250">
  <img src="demo/video-1-4.gif" width="250"><br/>
  <img src="demo/video-2-1.gif" width="250">
  <img src="demo/video-2-2.gif" width="250">
  <img src="demo/video-2-3.gif" width="250">
  <img src="demo/video-2-4.gif" width="250"><br/>
  <img src="demo/video-3-1.gif" width="250">
  <img src="demo/video-3-2.gif" width="250">
  <img src="demo/video-3-3.gif" width="250">
  <img src="demo/video-3-4.gif" width="250"><br/>
  <img src="demo/video-4-1.gif" width="250">
  <img src="demo/video-4-2.gif" width="250">
  <img src="demo/video-4-3.gif" width="250">
  <img src="demo/video-4-4.gif" width="250"><br/>
  <img src="demo/video-5-1.gif" width="250">
  <img src="demo/video-5-2.gif" width="250">
  <img src="demo/video-5-3.gif" width="250">
  <img src="demo/video-5-4.gif" width="250"><br/>
  <img src="demo/video-6-1.gif" width="250">
  <img src="demo/video-6-2.gif" width="250">
  <img src="demo/video-6-3.gif" width="250">
  <img src="demo/video-6-4.gif" width="250"><br/>
  <img src="demo/video-7-1.gif" width="250">
  <img src="demo/video-7-2.gif" width="250">
  <img src="demo/video-7-3.gif" width="250">
  <img src="demo/video-7-4.gif" width="250"><br/>
  <img src="demo/video-8-1.gif" width="250">
  <img src="demo/video-8-2.gif" width="250">
  <img src="demo/video-8-3.gif" width="250"><br/>
  <i>PPO results</i>
</p>


## How to use my code

With my code, you can:

* **Train your model** by running `python train.py`. For example: `python train.py --world 5 --stage 2 --lr 1e-4`
* **Test your trained model** by running `python test.py`. For example: `python test.py --world 5 --stage 2`

**Note**: If you got stuck at any level, try training again with different **learning rates**. You could conquer 31/32 levels like what I did, by changing only **learning rate**. Normally I set **learning rate** as **1e-3**, **1e-4** or **1e-5**. However, there are some difficult levels, including level **1-3**, in which I finally trained successfully with **learning rate** of **7e-5** after failed for 70 times.


## Why there is still level 8-4 missing?

In world 4-4, 7-4 and 8-4, map consists of puzzles where the player must choose the correct the path in order to move forward. If you choose a wrong path, you have to go through path you visited again. With some hardcore setting for the environment, the first 2 levels are solved. But the last level has not been solved yet.
