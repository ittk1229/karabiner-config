# Karabiner config

JIS 配列の MacBook 用の Karabiner-Elements Complex Modifications

## Features

- JIS 配列の MacBook で US 配列のような入力が可能
- 日本語環境における vim をより便利に
- ホームポジションを崩さない入力をサポート

## Rules

### escape for japanese vimmer

<kbd>C-[</kbd> を <kbd>Esc</kbd>, <kbd>英数</kbd> の連続入力に変換

vim で日本語入力をする際、ノーマルモードに戻るたびに手動で <kbd>英数</kbd> を入力する手間を省略

### vim-like arrows

<kbd>C-H</kbd>, <kbd>C-J</kbd>, <kbd>C-K</kbd>, <kbd>C-L</kbd> をそれぞれ <kbd>←</kbd>, <kbd>↓</kbd>, <kbd>↑</kbd>, <kbd>→</kbd> に変換

MacBook標準の <kbd>C-H</kbd> による削除が使えなくなるので注意

### corne-like keys

<kbd>C-かな</kbd>, <kbd>C-⌘</kbd> をそれぞれ <kbd>Return</kbd>, <kbd>Delete</kbd> に変換

親指で <kbd>Return</kbd> や <kbd>Delete</kbd> の入力が可能に

### us-like symbols

JIS 配列の記号を対応する位置の US 配列の記号に変換

JIS 配列における <kbd>]</kbd>は <kbd>Return</kbd>, <kbd>\_</kbd>は<kbd>\\</kbd>, <kbd>S-\_</kbd> は <kbd>|</kbd> になっている点に注意
