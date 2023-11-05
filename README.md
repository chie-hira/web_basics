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
リクエストの構成の一部<br/>
### HTTPステータスコードとは
それぞれの意味
* 200
* 201
* 400
* 404
* 500
***

### レスポンスヘッダーとは
### レスポンスボディとは
***

### JSONとは
### JSONを使ってデータを表現
*ユーザー情報を表現
*商品情報を表現


