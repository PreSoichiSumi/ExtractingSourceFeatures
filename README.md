# ExtractingSourceFeatures
Javaソースコードをパースして，特徴量を抽出します．
特徴としては，ソースコード中のノードの数(if文，変数宣言の数)を使います．
ソースコードのパースには，[EclipseJDT](http://sdl.ist.osaka-u.ac.jp/~s-kimura/jdtdoc/jdt.html)を用いました．

## ツールの動作
1．入力として受け取ったソースコードのASTを構築
2. VisitorによりASTを辿り，特徴量を取得し，出力する
