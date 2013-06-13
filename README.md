# 緯度経度から行政区への変換テーブル

[国土交通省 国土数値情報](http://nlftp.mlit.go.jp/ksj/gml/datalist/KsjTmplt-N03.html)を元に、緯度経度から市区町村への変換テーブルを作りました。

現在はGeohashの4桁, 5桁を元にしたテーブルになっています。

Geohashを使うことで、緯度経度から簡単に大体の住所を導き出すことができます。

データの生成方法などについては http://qiita.com/items/21a282c7bf54fd6a4985 を参照してください。

## CSVのフォーマット

```
GeoHash, 緯度, 経度, 都道府県, 支庁, 群もしくは市, 市町村, 郵便番号
```

例:

```
xpsj,43.154296875,140.80078125,北海道,後志支庁,余市郡,余市町,01408
```

https://github.com/FrogAppsDev/jpcities
