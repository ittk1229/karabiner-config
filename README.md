# Karabiner config

JIS 配列の MacBook 用の Karabiner-Elements Complex Modifications

## Features

- JIS 配列の MacBook で US 配列のような入力が可能
- 日本語環境における vim をより便利に
- ホームポジションを崩さない入力をサポート
- 小指より親指を多用

## Rules

### us-like symbols

- JIS 配列の記号を対応する位置の US 配列の記号に変換
- JIS 配列における <kbd>]</kbd> は <kbd>↩︎</kbd>, <kbd>\_</kbd> は <kbd>\\</kbd>, <kbd>⇧\_</kbd> は <kbd>|</kbd> になっている点に注意

---

### space as right control

- <kbd>␣</kbd> を他のキーと組み合わせて入力する場合 <kbd>右 ⌃</kbd> に変換
  - 本来左手小指で入力する必要がある <kbd>⌃</kbd> を親指で入力可能に
  - <kbd>⌃</kbd> と干渉しない独自のキーバインドを設定可能

### vim-like arrows

space as right control と組み合わせて使用

- <kbd>右 ⌃h</kbd>, <kbd>右 ⌃j</kbd>, <kbd>右 ⌃k</kbd>, <kbd>右 ⌃l</kbd> をそれぞれ <kbd>←</kbd>, <kbd>↓</kbd>, <kbd>↑</kbd>, <kbd>→</kbd> に変換
  - ホームポジションを崩さず矢印キーが使用可能に
  - 標準の <kbd>⌃h</kbd> による削除は <kbd>左 ⌃h</kbd> で利用可能

---

### corne-like keys

使用感を自作キーボード [corne](https://github.com/ittk1229/qmk_firmware/tree/ittk1229/keyboards/crkbd/keymaps/ittk1229) に近づける

- <kbd>⇥</kbd> を <kbd>esc</kbd>, <kbd>英数</kbd> の連続入力に変換
  - <kbd>esc</kbd> をより近い位置に
  - vim で日本語入力をする際、ノーマルモードに戻るたびに <kbd>英数</kbd> を入力する手間を省く
- <kbd>⌃</kbd> の単押しを <kbd>⇥</kbd> に変換
  - <kbd>⇥</kbd> を <kbd>esc</kbd> に割り当てたため、ここで整合性をとる
  - 他のキーと組み合わせて入力した場合は <kbd>⌃</kbd> が入力される
- <kbd>かな</kbd> を <kbd>↩︎</kbd> に変換
  - 親指で <kbd>↩︎</kbd> を入力可能に
- <kbd>英数</kbd> を他のキーと組み合わせて入力する場合 <kbd>⌘</kbd> に変換
  - 親指のより近い位置で <kbd>⌘</kbd> を入力可能に
- <kbd>右 ⌘</kbd> の単押しを <kbd>かな</kbd> に、他のキーと組み合わせての入力を <kbd>⇧</kbd> に変換
  - <kbd>かな</kbd> を <kbd>↩︎</kbd> に割り当てたため、ここで整合性をとる
  - 親指で <kbd>⇧</kbd> を入力可能に
- <kbd>右 ⇧</kbd> を <kbd>⌦</kbd> (windows の <kbd>Del</kbd> に相当) に変換
  - <kbd>⌦</kbd> を単体で入力可能に
- <kbd>⇪</kbd> を 絵文字キーボードのショートカット(<kbd>⌃⌘␣</kbd>) に変換
  - 絵文字キーボードを 1 キーで呼び出し可能に
  - <kbd>⇪</kbd> は不要と判断し、他のキーに割り当てていない

---

### esc to screenshot

- <kbd>esc</kbd> を <kbd>⇧⌘5</kbd> に変換
  - <kbd>⇥</kbd> を <kbd>esc</kbd> に割り当てたため、空いた <kbd>esc</kbd> を有効活用
  - スクリーンショットツールが 1 キーで呼び出し可能に
