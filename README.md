# 使用源成像分析脑区功能连接性
## 环境配置
```
conda create -n mne python=3.9
conda install -r requirements.txt
```
## FreeSurfer version 7
- **安装链接**: https://surfer.nmr.mgh.harvard.edu/fswiki/DownloadAndInstall
- **使用教程**: https://surfer.nmr.mgh.harvard.edu/fswiki/Tutorials
## 数据集下载
以下数据集均为公开数据集，可以直接进入官网下载
- **High Gamma Dataset**: https://github.com/robintibor/high-gamma-dataset
- **BrianLat Dataset**: https://www.synapse.org/Synapse:syn51549340
## 运行
- 运行前需要准备的数据：
  - **EEG数据**: `.set`等文件类型
  - **MRI数据**: `.t1w.nii.gz`等文件类型
  - **头模型文件**: 安装FreeSurfer后运行`recon-all -s subject_id -i /path/to/mri_image.nii.gz -all`即可生成头模型，其中subject_id为自行指定的id。
- 修改对应的`.ipynb`文件中以上的文件路径即可运行