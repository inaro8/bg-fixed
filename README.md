# bg-fixed
ページ内の複数箇所（それぞれ別の画像）を背景固定する

## 機能
背景画像をfixedしている要素の周りをclip-pathでくり抜くとできた。  
ただこの方法では、chromeでclip-pathしている要素の上に重ねている要素が表示されないことがあった。  
重ねる要素にtransform: translateZ(0);を指定すると大丈夫になった。

## デモ
https://inaro8.github.io/bg-fixed/
