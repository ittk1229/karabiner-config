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
- JIS 配列における <kbd>]</kbd>は <kbd>↩︎</kbd>, <kbd>\_</kbd>は<kbd>\\</kbd>, <kbd>⇧\_</kbd> は <kbd>|</kbd> になっている点に注意

---

### space as control

- <kbd>␣</kbd> を他のキーと組み合わせて入力する場合 <kbd>⌃</kbd> に変換
  - 本来左手小指で入力する必要がある <kbd>⌃</kbd> を親指で入力可能に

---

### vim-like arrows

- <kbd>⌃h</kbd>, <kbd>⌃j</kbd>, <kbd>⌃k</kbd>, <kbd>⌃l</kbd> をそれぞれ <kbd>←</kbd>, <kbd>↓</kbd>, <kbd>↑</kbd>, <kbd>→</kbd> に変換
  - ホームポジションを崩さず矢印キーが使用可能に
  - 標準の<kbd>⌃h</kbd>による削除が使えなくなるので注意

---

### corne-like keys

使用感を自作キーボード [corne](https://github.com/ittk1229/qmk_firmware/tree/ittk1229/keyboards/crkbd/keymaps/ittk1229) に近づける

- <kbd>⇥</kbd> を<kbd>esc</kbd>, <kbd>英数</kbd> の連続入力に変換
  - <kbd>esc</kbd>をより近い位置に
  - vim で日本語入力をする際、ノーマルモードに戻るたびに <kbd>英数</kbd> を入力する手間を省く
- <kbd>⌃</kbd> の単押しを<kbd>⇥</kbd> に変換
  - <kbd>⇥</kbd> を<kbd>esc</kbd> に割り当てたため、ここで整合性をとる
  - 他のキーと組み合わせて入力した場合は<kbd>⌃</kbd>が入力される
- <kbd>かな</kbd>, <kbd>fn</kbd> をそれぞれ<kbd>↩︎</kbd> ,<kbd>⌫</kbd> に変換
  - 親指で <kbd>↩︎</kbd> と<kbd>⌫</kbd> の入力が可能に
- <kbd>英数</kbd> を他のキーと組み合わせて入力する場合 <kbd>⌘</kbd>に変換
  - 親指のより近い位置で<kbd>⌘</kbd>を入力可能に
- <kbd>右 ⌘</kbd>の単押しを<kbd>かな</kbd>に、他のキーと組み合わせての入力を<kbd>⇧</kbd>に変換
  - <kbd>かな</kbd>を<kbd>↩︎</kbd>に割り当てたため、ここで整合性をとる
  - 親指で<kbd>⇧</kbd>を入力可能に
