# bg-fixed
ページ内の複数箇所（それぞれ別の画像）を背景固定する

## 機能
背景画像をfixedしている要素の周りをclip-pathでくり抜くとできた。  
ただこの方法では、chromeでclip-pathしている要素の上に重ねている要素が表示されないことがあった。  
重ねる要素にtransform: translateZ(0);を指定すると大丈夫になった。（原因わからず）

試したこと↓  
IntersectionObserver APIを使って、背景が切り替わる要素までスクロールしたとき、  
bodyのbeforeに敷いている背景画像を切り替えようと思ったが、iOS Safariで勢いよくスクロールしたときに、  
背景の切り替わりがラグるときがあってダメだった

## デモ
https://inaro8.github.io/bg-fixed/
