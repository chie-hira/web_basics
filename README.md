# web_basics
## URLとは
ホームページの住所<br/>
Uniform Resource Locator<br/>
web上で取得したいページなどの情報源を示すための表記方法  

例)
https://www.jitec.ipa.go.jp/1_04hanni_sukiru/_index_mondai.html<br/>

| 部位 | 意味 |
| ---- | ---- |
| https:// | スキーム名 |
| www. | ホスト名 |
| jitec.ipa.go.jp | ドメイン名 |
| /1_04hanni_sukiru/ | パス名(ディレクトリ名)　 |
| _index_mondai.html　 | ファイル名 |

***

## クエリ文字列とは
クエリパラメータ<br/>
サーバーに情報を送るためにURL末尾につけ足す文字列<br/>
webのページそのものは変わらないが表示する内容を指定する<br/>
パスパラメータより階層が下のイメージ

例)<br/>
https:// query.jp/?param1=hoge1&param2=hoge2<br/>

| 部位 | 意味 |
| ---- | ---- |
| https:// query.jp | URL(クエリ文字列以外の部分) |
| ?param1=hoge1&param2=hoge2 | クエリ文字列 |

## パス変数とは
パスパラメータ<br/>
Webのページそのものを指定する<br/>
クエリパラメータより階層が上のイメージ

例)<br/>
https:// query.jp/category/{categry_id}/?param1=hoge1&param2=hoge2<br/>

| 部位 | 意味 |
| ---- | ---- |
| {categry_id} | パス変数 |
| ?param1=hoge1&param2=hoge2 | クエリ文字列 |


## クエリ文字列とパス変数の違い
* パスパラメータは表示のベースとなるWebページを指定する
* クエリパラメータはWebページのオプションを指定する(GETにあたる)

***

## HTTPメソッドとは
簡単にいうとGETとかPOSTのこと<br/>
PUT,PATCH,DELETEなど他にもある  

| メソッド名 | 意味 |
| ---- | ---- |
| GET | ページを要求 |
| POST | データを渡す |
| PUT | リソース全体をリクエスト内容で置き換える |
| PATCH |　リソースを部分的にを置き換える |
| DELETE | リソースを削除する |

***

## リクエストヘッダーとは
HTTPリクエスト(リクエストライン、ヘッダー、メッセージボディ)の構成の一部<br/>
メッセージの内容には関連しない<br/>
ブラウザからwebサーバーに伝えたい情報<br/>
フィールド名:内容で表現  

<img width="184" alt="スクリーンショット 2023-11-05 23 24 55" src="https://github.com/chie-hira/web_basics/assets/148871501/dc27512a-5be1-4bd3-8c06-4bc22d4c7532">


### HTTPステータスコードとは
HTTPリクエストの結果を示す3桁の数字　　

| コード | 意味 |
| ---- | ---- |
| 200 |　OK,成功 |
| 201 |　Created,リソースの作成成功 |
| 400 |　Bad Request,リクエストの内容が変 |
| 404 |　Not Found,リソースが見つからない |
| 500 |　Internal Server Error,サーバーエラー |

***

### レスポンスヘッダーとは
HTTPレスポンス(ステータスライン、ヘッダー、レスポンスボディ)の構成の一部<br/>
メッセージの内容には関連しない<br/>
HTTPレスポンスはHTTPリクエストに対する返事<br/>
ステータスラインに書ききれないレスポンスの情報<br/>
フィールド名:内容で表現  

<img width="180" alt="スクリーンショット 2023-11-05 23 49 15" src="https://github.com/chie-hira/web_basics/assets/148871501/a3e15d86-14d1-4853-a668-dcdbe2464d7f">


### レスポンスボディとは
HTTPレスポンス(ステータスライン、ヘッダー、レスポンスボディ)の構成の一部<br/>
メッセージの内容部分<br/>
HTML部分

***

### JSONとは
ファイル形式の1つ<br/>
JavaAcriptObjectNotation<br/>
データのやり取りをするときの書き方　　

例)<br/>
```json
{
  "bohebohe": [ 1, 2 ],
  "piyopiyo": {
  "piyota": [ "21", "lovely" ],
  "piyoko": "sama"
  }
}
```

### JSONを使ってデータを表現
例1) ユーザー情報を表現
```json
{
  "name": "中田",
  "age": 35,
  "location": "東京都",
  "hobby": "登山",
  "birthdate": "2000-09-09"
}
```

例2) 商品情報を表現
```json
{
  "productName": "Example Product",
  "price": 49.99,
  "inStock": true,
  "category": "Electronics",
  "description": "This is an example product description."
}
```

