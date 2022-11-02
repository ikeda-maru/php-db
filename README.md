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