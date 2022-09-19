# 手順(工事中)


## 1.map対象論文の選定  

### 1.1ソースのデータセット
[COCI January 2022 Dump](https://doi.org/10.6084/m9.figshare.6741422.v13)を利用した。
- 論文数:71,337,645  
- 引用数:1,271,360,867  

### 1.2近年の引用情報のみを抽出
おおむね2019年以降の高被引用論文を対象にするため、以下の条件で引用をフィルタ
- creation >= 2019/1/1  
- creationの年部分 - timespanの年部分 >= 2019    
その結果、以下に絞られた。
- 引用数:7,450,676 
- 論文数:46,563,981  
 
### 1.3分野ごとのトップ論文の計算
おおむね5% 以下となるようにする。被引用数21以上のみを対象にした。  
メタデータ取得対象:390,587論文  
分野ごとに1/5にて78,026  

## 2.クラスタリング

### 2.1クラスタリング方法

共引用度とクラスタ数の比較  
<iframe width="1000" height="700" frameborder="0" scrolling="no" src="clustering_stats_std.html"></iframe>  

共引用度とクラスタ数の比較(logスケール)  
<iframe width="1000" height="700" frameborder="0" scrolling="no" src="clustering_stats_log.html"></iframe> 

### 2.2クラスタリングの分野推定
