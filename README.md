# smartcity-data-upload-template

Excel / CSV / GeoJSON / Shape ファイルをスマートシティ用のタイルに変換するテンプレートリポジトリです。


## 使い方

### **:black_medium_square: 初期設定**

* [[Use this template]](https://github.com/geolonia/smartcity-data-upload-template/generate) ボタンをクリックして、このテンプレートを自分のリポジトリにコピーしてください。
* [設定ファイル](https://github.com/geolonia/smartcity-data-upload-template/blob/main/.github/workflows/build.yml)にアクセスし、以下を書き換えて下さい。
  * `MUNICIPALITY_CODE`: 全国地方公共団体コード (5桁) （例: `37201`）
 
### **:black_medium_square: データを追加する**
* Excel / CSV / GeoJSON / Shape ファイルを [data](https://github.com/geolonia/smartcity-data-upload-template/tree/main/data) リポジトリにアップロードして下さい。
* ディレクトリ名、ファイル名がそのままスマートマップのサイドバーの階層になります。
  * ※ 順番を指定できないので改善する

**例**
```
都市計画情報/用途地域/
 ├ 工業地域.shp
 ├ 工業地域.dbf
 └ 工業地域.shx
環境施設.xlsx
```
![スクリーンショット 2023-12-15 14 23 47 2](https://github.com/geolonia/smartcity-data-upload-template/assets/8760841/f1302fe1-6a16-4b43-b630-e26836f4d96d)

### **:black_medium_square: 結果を地図で確認する**

「Actions」タブをクリックし最新のログをクリックして下さい。ログの中に出力されているプレビューURLをクリックすると結果が地図で確認できます。
<img width="1355" alt="スクリーンショット 2024-06-20 17 30 30" src="https://github.com/geolonia/smartcity-data-upload-template/assets/8760841/bb707698-38ac-48be-b21d-83d8e9f6c332">

### **:black_medium_square: その他**
* 生成した PMTiles を https://geolonia.github.io/smartcity-smartmap/ にドラッグ& ドロップする事で、プレビュー出来ます。
* 将来的には自動で反映する？
