# Eazy Face Recognition (Demo)
[![LeTian Space](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://lloydztw.github.io/mysite/)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
[![LeTian FB](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/letian.chang)
[![](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lloydz.tw@gmail.com)

OCR server written in pytorch

------------------------------------------------------------------

## History
- 27 Feb 2023 - Version 2.1.1.0
    - 辨識可以指定部分參與人員
    - 限定某些接口 (http 端點) 只能在本機操作.
    - 加入註冊碼機制來綁定單機使用.
    - Revised by [@letian Chang](https://lloydztw.github.io/mysite/).    
    <br/>

- 07 Jan 2023 - Version 2.0.0.1
    - 使用新模型, 可以偵測 有戴口罩 之人像
    - 必須使用 cuda 11.3
    - Revised by [@letian Chang](https://lloydztw.github.io/mysite/).    
    <br/>

- 26 Dec 2022 - Version 1.0.3.2
    - 增加繪製辨識結果圖
    - 增加連續辨識範例 (performConiRecognition)
    - asyncRun 使用 BeginInvoke (thread)
    - Revised by [@letian Chang](https://lloydztw.github.io/mysite/).    
    <br/>
- 22 Dec 2022 - Version 1.0.2.2
    - 改使用 .Net FrameWork 4.8 
    - Revised by [@letian Chang](https://lloydztw.github.io/mysite/).    
    <br/>
- 21 Dec 2022 - Version 1.0.1
    - 創建版
    - Revised by [@letian Chang](https://lloydztw.github.io/mysite/).


## Install dependencies
### Requirements
- anaconda
- python 3.8
- CMake
- visual studio 2022


<br/><br/>

# 如何 【全部重新】 安裝
(0) 下載以下檔案 
- http://download.jeteazy.com/LeTian/EzFace/EzFaceDemo_Setup_2.1.1.0.exe
- http://download.jeteazy.com/LeTian/EzFace/requirements_2.txt 

<br/> 
至暫存資料夾, <br/>

開啟 windows command line 視窗 (anaconda 專用的) 
依序 鍵入 以下指令:

------------------------------------------------------------------
(1) 安裝 anaconda 到 C:\anaconda3 <br/>

------------------------------------------------------------------
(2) 移除舊的 anaconda python 3.9 環境,用 command line 執行: <br/>
    (如果是新機安裝, 或目前已經有 python 3.8 名稱為 face_cn 的虛擬環境, 可跳過此步驟.)
```
conda deactivate
conda env remove -n face_cn
```
(2.1) 安裝 python 3.8 虛擬環境,<br/> 
    用 command line 執行:<br/> 
    (如果目前已經有 python 3.8 名稱為 face_cn 的虛擬環境, 可跳過此步驟.)
```
conda create -n face_cn python=3.8
```
(2.2) 進入 face_cn 虛擬環境<br/>
成功後,手動鍵入:
```    
conda activate face_cn
```
------------------------------------------------------------------
(3) 安裝 c++/c# 第三方套件,<br/>
- 下載並安裝 Visual Studio 2022
- 下載並安裝 CMake
- 下載並安裝 nVidia CUDA tool kits 11.3 (or 11.7)

------------------------------------------------------------------
(4) 安裝 python 第三方套件,<br/>
(4.1) 安裝 pytorch 用 command line 執行:
```
conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch
```
(4.2) 用 command line 執行:
```
pip install -r requirements_2.txt
```
##### 或
```
conda install --yes --file requirements_2.txt
```

##### ( 檔案 requirements_2.txt 條列有所需要的第三方套件 ) <br/><br/>

------------------------------------------------------------------
(5) 安裝 C# demo 程式專案,<br/>
    用 command line 執行:
```
EzFaceDemo_Setup_2.x.x.x.exe
```
------------------------------------------------------------------
(6) 用 visual studio 2022 開啟專案
- D:\AUTOMATION\Eazy Face Demo\C#\EzFaceClientDemo_CN.sln

------------------------------------------------------------------
# Author
**[LeTian Chang](mailto:lloydz.tw@gmail.com)**
<br/>

![](https://scontent.fkhh1-2.fna.fbcdn.net/v/t1.6435-9/94496580_3289259774417998_6021738680945737728_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=174925&_nc_ohc=58aiZPHed7gAX_6vKw5&_nc_ht=scontent.fkhh1-2.fna&oh=00_AT8By9vZ7G_MIRGxsr_sPpJdVepuxVMk8szf0ts3L1U7Ig&oe=62FD3DAD)    
