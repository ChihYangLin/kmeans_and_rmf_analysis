## K-means 集群分析
#### 使用非監督式模型K-means，將電商的顧客交易資料做分群貼標，供後續做商業分析參考。

## 實作步驟
* 1 整理要放進Kmeans的特徵欄位
  * 非數值型態 --> 數值型態 --> one hot encoding
  * 如下圖所示 : 特徵欄位加入R(最近的購買日), F(購買頻率), M(總消費金額), 購買種類次數, 地區, 性別
  * ![image](https://github.com/ChihYangLin/kmeans_and_rmf_analysis/blob/master/demo_photos/kmeans.png)
* 2 用1~20群做Kmeans，把誤差做成圖，觀察最適合的分群數目
 * ![image](https://github.com/ChihYangLin/kmeans_and_rmf_analysis/blob/master/demo_photos/cluster_error.png)
* 3 給予每個顧客群標籤，並秀出每一群的特徵數值，以供後續視覺化或分析
 * ![image](https://github.com/ChihYangLin/kmeans_and_rmf_analysis/blob/master/demo_photos/results.png)
* 4 視覺化(以第0群的消費種類為例)
 * ![image](https://github.com/ChihYangLin/kmeans_and_rmf_analysis/blob/master/demo_photos/category.png)
