[![Work in Repl.it](https://classroom.github.com/assets/work-in-replit-14baed9a392b3a25080506f3b7b6d57f295ec2978f6f33ec97e36a161684cbe9.svg)](https://classroom.github.com/online_ide?assignment_repo_id=3626355&assignment_repo_type=AssignmentRepo)
# 房價預測
## 1.房價預測使用工具：
### 使用的程式軟體：
Google Colaboratory  
### 使用的測試檔案：
  train-data.csv - 訓練的資料合集  
  valid-data.csv - 驗證的資料合集  
  test-data.csv - 測試的資料合集  
  metaData.csv - 介紹資料的 
## 2.程式方塊圖及作法：
  ![image](data/processchart.png)

## 3.畫圖及結果分析：
  ![image](data/picture/house_price_plt.png)  ![image](data/picture/house_price_plt2.png)  ![image](data/picture/house_price_plt3.png)  ![image](data/picture/house_price_plt4.png) ![image](data/picture/house_price_plt5.png)  ![image](data/picture/house_price_plt6.png) ![image](data/picture/house_price_plt7.png) ![image](data/picture/house_price_accuracy.png)

## 4.討論預測值誤差很大的狀況：
  一開始是以為model的隱藏層數不夠，後來發現這跟我們挑選訓練的data很有相關，
  在訓練時需要考慮到我們所訓練的data和我們所想要得到的目標關聯性產生良好的影響，
  並去斟酌選取必要的data作為訓練模型的資料基礎，再做模型的訓練，結果會比之前的預測誤差的狀況要好的多。
  
  在調整模型方面，除了在調整神經元參數、層數以外，還有額外加入earlystop的指令，
  可以防止模型在訓練時產生overfiting，進而讓模型產生更好的結果。
  
## 5.修正方案：
### (1).選取需要的data參數
  ![image](data/picture/house_price_selectdata.png)
  ![image](data/picture/house_price_selectdata2.png)
### (2).改良訓練模型的參數、層數、優化器
  ![image](data/picture/house_price_model_fix.png)
### (3).加入earlystop的指令防止overfiting
  ![image](data/picture/house_price_earlystop.png)
