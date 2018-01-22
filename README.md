# CIFAR-10 チュートリアル [非公式]

## はじめに
このノートでは、私がRWTH Aachen University (アーヘン工科大学) の夏学期の講義「Deep Learning in Physics Research」で学んだ[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)の分類問題について説明しています。コード自体が長いため、インタラクティブ形式にまとめていますが、最後に全体のコードを一括に書いています。

## <u> 予備知識&想定読者 </u>

<u>予備知識&想定読者</u>
- 深くは理解できていないが、Tensorflowで[MNIST for beginners](https://www.tensorflow.org/get_started/mnist/beginners)はやってみた。が、その後が続かない。
- 機械学習の背景については一通り勉強してみた（「ゼロから作るDeep Learning」)
- Kerasを使ってCNNをやってみたい。

※いくつか勉強不足の点があるので、間違いを見つけられた場合はご指摘いただけると嬉しいです。issueページにて受け付けております。

## 更新履歴
- 2018/01/22: `dlipr`を新たに`dlt`とリネームし、PyPIへ登録しました。これについては[dltのリポジトリ](https://github.com/hiroyuki827/deep_learning_tools)からどうぞ。
- 2018/01/18: dliprパッケージで使われている`np.histogram2d`にてエラーが発生しているため、confusion matrixに関する記述を削除しました。

## <u>動作環境</u>

- Python 3.0以上
- GTX 1080 GPU with 8GB memory (パワーがあればそれでいい)
- Keras
- Tensorflow 1.4.1以上
- dlt

**準備**
`pip install dlt`でダウンロードできます。

## <u>参考文献</u>:
- 「ゼロから作るDeep Learning」(斎藤 康毅著）
- [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
- [DeepLearning系ライブラリ、Kerasがあまりにも便利だったので使い方メモ](http://www.procrasist.com/entry/2017/01/07/154441#modelを作る)
- 講義のレジュメ・スライド ([こちら](https://github.com/hiroyuki827/deep_learning_in_physics_research_SS17)の各講義回ディレクトリよりダウンロード可)