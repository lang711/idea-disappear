## 初衷

想做也只是想，不保留就容易忘却，空留遗憾，所以每当有什么想法就赶紧写下来，即使天马行空，即使乱七八糟，这就是种子，即便在这一刻它没有生根发芽，也许这一辈子也不会，那也没什么，因为这就是希望。


### 水平居中
实则上，对于行内元素用`text-align:center`就可以解决**99%**种情况，而块级元素，如果只是单一块级元素那么用`margin:auto`足以解决，
但很多时候肯定不止，那么将父元素设置`display:flex`，`justify-content:center`，不仅可以轻松解决，而且还能消除行内元素之间由于编辑器的原因产生的间隙问题。
当然，也可以设置`margin-left:50%`或者`left:50%`,接着用`transform:translateX(-50%)`拉回来。


### 垂直居中
很容易就想到，用`line-height`就可以轻松解决行内元素垂直居中，但同时应该给块级元素设置`height`，毕竟`line-height`并不是实际高度，而对于其他行内块或者块级元素，也同样可以使用`display:flex`,`align-items:center`来实现，也可以使用`margin-top`或者`top`，再用`transform：translateY(-50%)`,总之，所谓的居中也并不一定是居中，而是要根据设计图去调整，吹毛求疵总是会很累。
