# MTDF
# Title: MTDF: A Multi-Task-based X-ray Weld Image Detection Framework via State Space Model
This is the open source code for the paper "MTDF: A Multi-Task-based X-ray Weld Image Detection Framework via State Space Model" submitted to Automation in Construction. 

We have released our multi-task datasets.  Supplementary material of the revised manuscript can be viewed on  [Supplementary Material](https://youtu.be/F0Z5kD4nh2E).

# Supplementary material of Demo Video (Inspection Process)
To provide readers with a clearer understanding of the spiral steel pipe production and defect detection process, we have included a demonstration video.
You can directly click on the link [YouTube](https://youtu.be/vKmVoBKwP0Q) to watch our video. Thank you for your watching.
This is a demonstration video of MTDF method in engineering practice. We instantiate MTDF framework in the hardware platform and the constructed intelligent software. 
The proposed framework demonstrates measurable superiority over conventional manual inspection in practical deployment scenarios.  
Future research directions prioritize the deployment of this software framework within practical edge computing infrastructure, constituting a critical focus of our ongoing investigations.
# Supplementary material of Demo Video (Transmission Device)
We demonstrate the real-time detection process of spiral weld defects.  The video can be viewed in the Youtube [Real-time Detection]( https://youtu.be/CEZ-Yzh1kBM). The left panel of the interface displays how the transmission system conveys the steel pipe with circumferential and radial movements during inspection.  Simultaneously, the right panel shows how inspectors manually monitor weld defects in real time throughout the process.

Due to the presence of radioactivity in the testing process, we can only take photos of the returned process of the tested steel pipe in the NDT room after the testing process. The video can be viewed in the Youtube [Transmission Device](https://youtu.be/77YTBS7kYqM).Thank you for your watching. 

# Supplementary material of Demo Video (X-ray Emitter)
To better understand the acquisition principle, we recorded the actual video of the X-ray emission source and the receiver board. You can directly click on the link [X-ray Emitter](https://youtu.be/0UJoFMqeVMY) to watch our video.  A mechanical scribing device integrated with the detector housing is mounted next to the receiver plate, which makes an actual symbol marking on the steel tube surface when a defect is detected.  This synchronous defect marking protocol enhances traceability while maintaining the continuity of uninterrupted inspection.
# The other Ongoing Plans
Furthermore, a QR code tracing module is currently under development within the software ecosystem, designed to facilitate more secure and efficient quality control processes.  Specifically, this innovative module enables the generation of concise digital inspection reports when scanning QR codes affixed to individual steel pipes.  These comprehensive reports document critical quality parameters including: 1) quantitative analysis and categorical classification of manufacturing defects;  2) temporal records of defect identification;  and 3) traceable accountability through identification of responsible inspection personnel.  This dual-component system architecture establishes an auditable quality assurance mechanism while optimizing operational workflow efficiency.

# SDL/WES/DIS Dataset
Datasets can be found at [BaiduYun Drive](https://pan.baidu.com/s/1XbtjL58-aiNg1DxeQo6hmQ?pwd=wm4e) (code: wm4e).
The distribution of the six defect types can be found at [Class_distribution](https://pan.baidu.com/s/1l4vasW8Aid8QyeMOFAvDdQ?pwd=w7ms) (code: w7ms)
The data are used for academic purposes only.
# system

<img width="698" alt="MTDF_系统_Elsevier" src="https://github.com/user-attachments/assets/e42f0cab-34c5-4c80-98a1-d40a740894a5" />

# Framework

<img width="615" alt="模型框架_MTDF_Elsevier_gai" src="https://github.com/user-attachments/assets/639e0942-49a8-44ff-89c2-bf09e3f9274a" />

# Code
Our code is available at  [MTDF](https://pan.baidu.com/s/1FmkXgNJ7eM7EQ566X4JHXQ?pwd=bq3x) (code: bq3x)

# Main results
The main experimental results are provided in [MTDF_Results](https://pan.baidu.com/s/1o0zEplwmF3jEZj8ghe14Wg?pwd=erui) (code: erui)

## 0. Main Environments
```bash
conda create -n vmunet python=3.8
conda activate vmunet
pip install torch==1.13.0 torchvision==0.14.0 torchaudio==0.13.0 --extra-index-url https://download.pytorch.org/whl/cu117
pip install packaging
pip install timm==0.4.12
pip install pytest chardet yacs termcolor
pip install submitit tensorboardX
pip install triton==2.0.0
pip install causal_conv1d==1.0.0  # causal_conv1d-1.0.0+cu118torch1.13cxx11abiFALSE-cp38-cp38-linux_x86_64.whl
pip install mamba_ssm==1.0.1  # mmamba_ssm-1.0.1+cu118torch1.13cxx11abiFALSE-cp38-cp38-linux_x86_64.whl
pip install scikit-learn matplotlib thop h5py SimpleITK scikit-image medpy yacs
```
The .whl files of causal_conv1d and mamba_ssm could be found here. {[Baidu](https://pan.baidu.com/s/1Tibn8Xh4FMwj0ths8Ufazw?pwd=uu5k)}

# Training
1. Download the pre-trained model [VMamba-S]([https://pan.baidu.com/s/1cIX3ruaQqEG6jgb9yCWDqg](https://github.com/MzeroMiko/VMamba)
2. Modify the configuration in `train.py`
3. Run `python train.py` to start training


# User interface
![image](https://github.com/cuiwq777/TRDM/assets/154526698/8ba32b78-daa8-4d96-938e-cd9db82515b6)

# Demo of User interface
![ezgif com-video-to-gif-converted (3)](https://github.com/cuiwq777/TRDM/assets/154526698/0a1213c3-5744-46c5-a2a7-6e7302359a0c)

# Demo of the inspection process
![ezgif com-video-to-gif-converted (4)](https://github.com/cuiwq777/TRDM/assets/154526698/2c2e5eab-8e9c-4ffe-943a-fc65c5512635)

![ezgif com-video-to-gif-converted (5)](https://github.com/cuiwq777/TRDM/assets/154526698/d51f12da-204e-4e10-b900-c5e48b4c1940)







