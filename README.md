# Traditional Chinese Handwriting Dataset <a href="https://colab.research.google.com/github/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset/blob/master/Data_Deployment_colab.ipynb"><img src="https://img.shields.io/badge/%E5%AF%A6%E4%BD%9C-Colab-yellow.svg?style=popout-square" alt="範例 Colab"></a>
# 繁體中文手寫資料集

![人工智慧 - 自由團隊](https://raw.githubusercontent.com/chenkenanalytic/img/master/af/aifreeteam.png)

## Preface 前言

In the way of data science, we believe every scholar, scientists might have heard about MNIST dataset, or played with Fashion MNIST. As a traditional Chinese user, we couldn't help but wonder: is it possible for machine learning, neural networks to recognize handwritten traditional Chinese characters? Let's challenge!

在走過資料科學的路上，相信每一位學者、科學家都聽過 MNIST dataset (手寫數字資料集)，或許也玩過 Fashion MNIST；身為繁體中文使用者，難免開始好奇：手寫繁體中文是否也有機會讓機器學習、神經網路成功辨識呢？讓我們一起來挑戰！

<br>

## Description 資料集說明

Original dataset was produced based on Tegaki, an open-source package. Total 13,065 different Chinese characters, with average of 50 samples for each character.

原始資料集基於 Tegaki 開源套件下產出，總計 13,065 個不同的中文字，每一個字體平均有 50 個樣本。

<br>

## Updates 更新紀錄

 - 2021.04.17 專案衍生應用： <a href="https://traditional-chinese-handwriting.github.io/">Web-based 模型訓練、手寫辨識</a>
 - 2021.04.14 (非直接相關) 趨勢科技 T-brain 玉山人工智慧挑戰賽2021夏季賽：<a href='https://tbrain.trendmicro.com.tw/Competitions/Details/13'>繁體中文場景文字辨識競賽</a>
 - 2020.09.03 Released the whole dataset (13,065 charaters; image size: 300x300pixels; total 684,677 images)
 - 2020.04.21 提供資料集部署操作範例 (感謝<a href='https://github.com/YenLinWu'> Yen-Lin 博士 </a>熱情貢獻)
 - 2020.04.21 提供資料集部署操作範例 (感謝<a href='https://github.com/YenLinWu'> Yen-Lin 博士 </a>熱情貢獻)
 - 2020.04.20 上傳最新資料集 (4,803個常用字；圖片大小：50x50pixels；共計 250,712 個圖片檔)
 (<a href='https://language.moe.gov.tw/001/Upload/Files/site_content/download/mandr/%e6%95%99%e8%82%b2%e9%83%a84808%e5%80%8b%e5%b8%b8%e7%94%a8%e5%ad%97%e8%aa%aa%e6%98%8e.pdf'>教育部 4,808 個常用字</a>)
 - 2020.04.20 Uploaded the first dataset (4,803 charaters; image size: 50x50pixels; total 250,712 images)
<br>

## Data samples 資料樣本

 - 完整資料集 - 各樣本資料夾
![完整資料集 - 各樣本資料夾](https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset/blob/master/img/img_folder.png?raw=true)

 - 手寫"自由"範例
![手寫"自由"範例](https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset/blob/master/img/img_samples.png?raw=true)

<br>

## Usage 使用方法

### 1. 完整資料集 - whole Dataset (13,065 characters)
``` bash
git clone https://github.com/chenkenanalytic/handwritting_data_all.git

cat (file_path)/all_data.zip* > (file_path)/all_data.zip

unzip (file_path)/all_data.zip -d (output_path)
```
※ (file_path) & (output_path) 以實際檔案位置需求作修改、替換，解壓縮後資料夾名稱為 cleaned_data，共684,677個圖片。



#### 完整資料集 - 部署操作

<a href="https://colab.research.google.com/github/chenkenanalytic/handwritting_data_all/blob/master/Data_Deployment_all.ipynb">Colab操作程式碼參考</a>

<br>
 
### 2. 常用字資料集 - common words Dataset (4,803 characters)
``` bash
git clone https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset.git

```
※ 下載常用字資料集後，解壓縮 data 資料夾內的四個檔案，解壓縮後資料夾名稱為 cleaned_data(50_50)，共250,712個圖片。



#### 常用字資料集 - 部署操作 (感謝<a href='https://github.com/YenLinWu'> Yen-Lin 博士 </a>熱情貢獻)

<a href="https://colab.research.google.com/github/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset/blob/master/Data_Deployment_colab.ipynb#scrollTo=BtJidZSSed2C">Colab操作程式碼參考</a>

<a href="https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset/blob/master/Data_Deployment_local.ipynb">本地操作程式碼參考</a>

<br>
 
## Issues 問題與發現

1. 常用字資料集因壓縮至 50x50 Pixels，發現部分圖片檔筆畫不清楚、出現重疊現象。 (完整資料集較無此問題，資料為 300x300 Pixels)
2. 完整資料集佈署範例於 Colab 上解壓縮後，中文字集檔名會出現亂碼。


<br>

## Application 衍伸應用 - <a href="https://traditional-chinese-handwriting.github.io/">Web-based 模型訓練、手寫辨識</a>

The application was developed based on the <a href="https://www.coursera.org/learn/browser-based-models-tensorflow/home/week/2">week 2</a> homework of <a href="https://www.coursera.org/learn/browser-based-models-tensorflow/home/welcome">Browser-based Models with TensorFlow.js</a> in <a href="https://www.coursera.org/specializations/tensorflow-data-and-deployment">TensorFlow: Data and Deployment Specialization</a> on coursera.

此衍生應用基於 Deeplearning.ai 之 Coursera 線上課程，<a href="https://www.coursera.org/specializations/tensorflow-data-and-deployment">TensorFlow: Data and Deployment Specialization</a> 的第一堂課程：<a href="https://www.coursera.org/learn/browser-based-models-tensorflow/home/welcome">Browser-based Models with TensorFlow.js</a> 的 <a href="https://www.coursera.org/learn/browser-based-models-tensorflow/home/week/2">第二週</a>線上作業所開發。 

![繁體中文手寫辨識_智](https://raw.githubusercontent.com/chenkenanalytic/img/master/tchc-ke/%E7%B9%81%E9%AB%94%E4%B8%AD%E6%96%87%E6%89%8B%E5%AF%AB%E8%BE%A8%E8%AD%98_%E6%99%BA.gif)

若您對於此專案有興趣，歡迎參考此<a href="https://aifreeblog.herokuapp.com/posts/134/Web-based_Traditional_Chinese_Handwriting_Classifier/">文章</a>說明。


## License 授權

<a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/3.0/tw/88x31.png" /></a> (CC BY-NC-SA 4.0)<br />本資料集適用 <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/">Attribution-NonCommercial-ShareAlike 4.0 International</a> 授權。
<br />The dataset applied <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/">Attribution-NonCommercial-ShareAlike 4.0 International</a> license.

※ 使用、改作、分享請附上以下資訊：

 - 本數據集由 AI . FREE Team 改作開發自 [STUST EECS_Chinese MNIST(總集)]。如有使用、改作、分享，請註明出處及此訊息。
 
 - The dataset is AI . FREE Team development from [STUST EECS_Chinese MNIST(總集)]. If used, modified, or shared, please cite the source and the mesage.
 
 - (source: https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset )


<br>

## Citing
```
@misc{AI.FREE2020,
  author = {Po-Chuan Chen},
  title = {Traditional Chinese Handwriting Dataset},
  year = {2020},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/AI-FREE-Team/Traditional-Chinese-Handwriting-Dataset}},
}
```
 
<br> 
 
## Source 資料來源

原資料集來源：https://scidm.nchc.org.tw/dataset/stusteecs_chinese_mnist

介紹說明影片：https://www.youtube.com/watch?v=eJy1BtkqHX4

來源說明：本數據集開發修改自南臺科技大學電子系所提供之中文手寫字集。

Description: The Dataset is developed from Chinese handwriting data set, which is provided by Dept. EECS, Southern Taiwan University of Science and Technology.
