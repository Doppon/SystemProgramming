Student Number: AL16060
          Name: Sekino Doppo

# mypower.c

- 詰まったところ / 工夫したところ
正常系の実装は比較的サクサクと進んだんですが、普段文字列をint型にするときに使うatoi関数をC言語で使うことが多かったので
double型に変換するときに上手くいかなくatof関数を使うことで解決しました。

また、異常系ではでは感覚的には
`argv[1] == NULL && argv[2] == NULL`
と言った第一引数、第二引数が何も入力されなかったときこう言うエラーが出て欲しいなとか考えていたのですが
この点、argvのポインタの仕組みを復習した際にかしこい作りになっているなと改めて思いました。



# mystrcmp.c

- 詰まったところ / 工夫したところ
最初に詰まったのはコマンドライン引数で受け取った際に文字列ポインタの理解を
全くしてなくて扱い方に困ったことです。

そこは定義にしたがって覚え直していくことですぐ解決しました。
またポインタの最後の配列に0が入るのはスンナリ進めました。

しかし、ポインタの長さが一緒だったときにに細かく差分を見るところは少し考えました。
実際には長さが一緒のときfor文で回すようにしてそれ以外は別の分岐で扱うようにして実現しました。
そして面白いのがポインタをそのまま演算できるところでした。

久しぶりにC言語書いた〜
