# Eazy Face Recognition (Demo)
[![LeTian Space](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://lloydztw.github.io/mysite/)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
[![LeTian FB](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/letian.chang)
[![](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lloydz.tw@gmail.com)

OCR server written in pytorch

------------------------------------------------------------------

## History
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
- http://download.jeteazy.com/LeTian/EzFace/EzFaceDemo_Setup_1.0.3.2.exe
- http://download.jeteazy.com/LeTian/EzFace/requirements.txt 
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
------------------------------------------------------------------
(2) 安裝 python 3.8 虛擬環境,<br/> 
    用 command line 執行:
```
conda create -n face_cn python=3.8
```
成功後,手動鍵入:
```    
conda activate face_cn
```
------------------------------------------------------------------
(3) 安裝 python 第三方套件,<br/>

(3.1) 下載並安裝 CMake 與 Visual Studio 2022

(3.2) 用 command line 執行:
```
conda install --yes --file requirements.txt
```
##### 或
```
pip install -r requirements.txt
```

##### ( 檔案 requirements.txt 條列有所需要的第三方套件 ) <br/><br/>

------------------------------------------------------------------
(4) 安裝 C# demo 程式專案,<br/>
    用 command line 執行:
```
EzFaceDemo_Setup.exe
```
------------------------------------------------------------------
(5) 用 visual studio 2022 開啟專案
- D:\AUTOMATION\Eazy Face Demo\C#\EzFaceClientDemo_CN.sln

------------------------------------------------------------------
# Author
**[LeTian Chang](mailto:lloydz.tw@gmail.com)**
<br/>

![](https://scontent.fkhh1-2.fna.fbcdn.net/v/t1.6435-9/94496580_3289259774417998_6021738680945737728_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=174925&_nc_ohc=58aiZPHed7gAX_6vKw5&_nc_ht=scontent.fkhh1-2.fna&oh=00_AT8By9vZ7G_MIRGxsr_sPpJdVepuxVMk8szf0ts3L1U7Ig&oe=62FD3DAD)    
