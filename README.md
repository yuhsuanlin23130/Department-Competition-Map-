### 說明
把104到108年個人申請考生的選擇集合做成一個T(系所數)×N(學生數)的矩陣，每一行表示某所科系有哪些學生填，透過t-Distributed Stochastic Neighbor Embedding (t-SNE) 降維並把矩陣投射到二維空間，則相似的選擇集合會聚到一起。由於投影之下科系彼此間有所重疊，透過 Hierarchical Clustering 對重疊科系做位置上的些微調整。

### 執行環境
Python3.7 + Jupyter Notebook

### 目錄結構說明
* ds資料夾內為104到108年個人申請之科系資訊與考生科系錄取資料。資料來源為<a href="https://www.com.tw/cross/?__cf_chl_jschl_tk__=06be384d9d4f5ac282bdb530b9a8a89ac6e588b8-1590161150-0-AWsb-xTrWdfw_cLTPEvZX2yMPSKIrFiEuhA_AG45dsGC0HQmn3xBwJUGT5hF_rPTSCDRxGeARPs82AWyG0eSuIPJTHk9KUMFhJGefReUCHVIkx9FP0o4kUkKubGIM76RE-xUX6nbXBCqf_FkfiyoTJkRpt2oBtrZ5XTXJKjSaO4sgQPQugKuC8y-Mz7sWgp01dp1mJCybuTqXYV4TZKQlOh5_mDJxCws9FTumOqdJKGhgakcDKXYpj71p4W-DkwblIFjITKgR1TnJGzb0Skp1_bf8OErkYoGWhSTjlByqNf3">交叉查榜網站</a>。
* 10* - tSNE_jaccard.ipynb 為各年度資料前處理、 t-Distributed Stochastic Neighbor Embedding (t-SNE) 投影實作，以及二維平面上避免科系重疊所做之調整。
* legend.png 為科系所屬領域之圖示。領域根據<a href="https://stats.moe.gov.tw/bcode/">大專校院學科標準分類</a>。
* 10*.png 為最終投影圖片檔。

