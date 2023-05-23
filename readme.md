# 安装

```
# 创建环境
conda create -n barf python==3.8
conda activate barf

# 安装mamba
conda install mamba -c conda-forge

# 安装pytorch、torchvision、cudatoolkit
mamba install pytorch=1.8.0 torchvision cudatoolkit=11.1.1 -c pytorch

# 安装pytorch3d
wget https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch3d/linux-64/pytorch3d-0.5.0-py38_cu111_pyt180.tar.bz2
conda install -c local pytorch3d-0.5.0-py38_cu111_pyt180.tar.bz2

# 安装程序包和其他依赖
pip install -r  requirements.txt -i https://pypi.doubanio.com/simple/
```


# 测试

运行命令
```
python bop_2_nerf.py
```

运行结果

![20230523135145](https://raw.githubusercontent.com/skykone1/images/main/20230523135145.png)