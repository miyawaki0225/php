### 001 
```php
<?php
echo "Hello World!";
?>
```

### 003 変数宣言
```php
<?php
$txts="Hello World!";
$x=2;
$y=3;
$z=$x+$y;

echo $txts;
echo "<BR/ >";
echo $z;
?>
```

### 004 ''(シングルクォート）と""（ダブルクォート）

- シングルクォートで囲まれた文字列は常に通常の文字とみなされる
- ダブルクォートの中には変数を宣言できる。
```php
<?php
$str="Hello";
echo "$str World!\n";
echo '$str World!';
?>
```

### 005 長い文字列
```php
echo <<<EOF
asdjfl;asdkj;jl;kj
EOF;
```

### 007 浮動小数点

- float,double,real

### 008 配列
```php
$colors1 = array();
$colors1[0] = "Red";
$colors1[1] = "Green";
$colors1[2] = "Blue";
echo $colors1[0];
```

- ()の中に初期値の代入も可能。
- ()の代わりに[]も使える。

### 011 定数  
- 書式：define（定数名、値）
- defineの代わりにconstで定義もできる

```php
define("start","Hello!");
define("pi",3.14);
echo start;
echo pi;
```

### 014 文字列演算子

- 「.」で結合
- 「.=」で結合代入

### 019-21 if条件判定
- 
```
if(判断条件式){
  条件式が真のときに実行する処理
}elseif(条件式){
}else{
}
```

### 022 switch
- case値に利用できるのは`int`と`string`のみ

### 024 do-while
- 前置判定（while文）
- 後起判定（do-while文）

### 025 for文
```php
for($i=1;$i<=5;$i++){
  echo "i=".$i."\n";
}
```

### 026 function文
function 関数名（引数）｛
  実行する処理；
  return 返り値;
｝

```php
function GetName($hikisu){
  echo $hikisu."\n";
}
```

### 027 事前定義済み：マジック定数
- __FILE__　現在のソースファイル名を表示
- __LINE__　現在の行番号を表示
- __DIR__　ファイルのフルパスとファイル名を取得
- __FUNCTION__　現在実行中の関数名を取得

### 028 グローバル変数
- グローバル変数（$GLOBALS['変数名']）
- ローカル変数

### 029 出力処理
- echo 複数の引数
- print 単一の引数
- var_dump(配列) 配列の中身を確認

### 030 連想配列
- 「キー => 値」と設定する
- JavaのMap

```php
$num=array("first"=>1,"second"=>2,"third"=>3);
var_dump($num);
```


