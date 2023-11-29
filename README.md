# 稻穗影像去背模型
本模型使用U2net為主要基礎架構，旨在應用於將透過手機拍攝的影像中萃取出稻穗影像並去除背景像素，以作為可進一步分析(如穀粒含水量推估)之預處理方式，由於U2net擅長背景去除的影像語義分割之用途，因此選擇基於此架構訓練去背模型。

以下左圖為輸入之原圖範例，右圖為輸出之結果範例：
![輸入原圖範例:](https://uav-fly.nchu.edu.tw/bot/static/display/20230621175528.jpg)![輸出結果範例:](https://uav-fly.nchu.edu.tw/bot/static/display/20230621175528.png)

1.訓練模型引用[U2net架構](https://github.com/xuebinqin/U-2-Net)
```
@InProceedings{Qin_2020_PR,
title = {U2-Net: Going Deeper with Nested U-Structure for Salient Object Detection},
author = {Qin, Xuebin and Zhang, Zichen and Huang, Chenyang and Dehghan, Masood and Zaiane, Osmar and Jagersand, Martin},
journal = {Pattern Recognition},
volume = {106},
pages = {107404},
year = {2020}
}
```
2. 稻米穀粒含水量推估模型參考文獻: https://www.mdpi.com/1424-8220/21/17/5875