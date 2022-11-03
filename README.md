# PHPとデータベース

## PHPとデータベースを接続
connect.php
PDOクラス
  PDOのインスタンス化は引数に直接情報を記載しても良いが冗長となり可読性低下を招く。
  したがって、connect.phpで記載しているように、それぞれ変数に代入した上で引数に渡す。

try-catch文
```
try {
  // 失敗する可能性があるコード

  // 失敗したらthrow文で例外を投げる
  throw new 例外クラス名()
} catch (例外クラス名 例外クラスのオブジェクトを代入する変数名) {
  // 失敗したとき行う処理
}
```

## PHPでテーブルを作成
create-table.php
query()メソッド
  実行したいSQL文が決まっている場合に使用
prepare()メソッド
  実行するSQL文が動的に変わる場合に使用
  bindvalue()
    プレースホルダ
      :(コロン)で始まる文字列で指定

## PHPでデータを取得(SELECT)
select.php
SELECT文
query()メソッド
fetchAll()メソッド

## PHPでデータを挿入(INSERT)
insert.php
prepare()メソッド
INSERT文
bindvalue
  プレースホルダ
  :(コロン)で始まる文字列で指定
isset関数
  変数に値がセットされているか調べる関数。
  値がセットされていれば"TRUE"を、そうでなければ"FALSE"を返す。
header関数
  ブラウザに対して様々な指示を出せる関数。
  header('Location: リダイレクト先のパス')にすれば、別のページにリダイレクトさせられる。