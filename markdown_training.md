GitHub Markdown 構文 練習用

# A first-level heading 見出し1
## A second-level heading 2
### A third-level heading 3
#### 4
##### 5
###### 6
見出しは6まで。

####### 7

**太字** _斜体_ ~~取り消し線~~ **太字および _太字中にある斜体_ の例** ***全体が太字かつ斜体*** <sub>下付き</sub> <ins>underlined下線付き</ins>
> 引用

コードの引用 `git status`

コードの引用ブロック
```
git status
git add
git commit
```


リンク
[GitHub Pages](https://pages.github.com/)

2 行の間に空白行を残すと、issue、pull request、ディスカッションの .md ファイルと Markdown の両方で、空白行で区切られた 2 行がレンダリングされます。

行の間に空白行がないと、
改行されない。

- George Washington 順序なしリスト
* John Adams
+ Thomas Jefferson

1. James Madison 順序ありリスト
2. James Monroe
3. John Quincy Adams

- 入れ子になったリストを作成するには、
   - 入れ子になったリスト項目の前に、リスト マーカー文字 (- または *) が、その上の項目のテキストの最初の文字の真下にくるまで
     - スペース文字を入力します。

- [ ] タスク リストを作成するには、リスト アイテムの前に空白、ハイフン、[ ] を付けます。
- [x] 完了したタスクをマークするには、[x] を使います。

脚注

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: 脚注は 脚注の参照の直後に書いてもよいが、表示される場所は 下部になる。
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.

脚注は Wiki ではサポートされていません。

<!-- HTML コメント内に配置することで、レンダリングされた Markdown からコンテンツを非表示にすることができます。This content will not appear in the rendered Markdown -->

テーブルの作成[^3]
[^3]: 出典 https://docs.github.com/ja/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables


パイプ (|) とハイフン (-) を使用してテーブルを作成できます。 ハイフンは各列のヘッダーの作成に使用され、パイプは各列の区切りに使用されます。 正しく表示されるように、表の前には空白行を 1 行追加してください。


| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

セルの幅は変わるので、列がぴったり一致する必要はありません。 各列のヘッダ行には、ハイフンを 3 つ以上使用してください。

| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |

ヘッダー行でハイフンの左、右、両側にコロン (:) を使うと、列でテキストを左寄せ、右寄せ、センタリングすることができます。

| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |

折りたたみセクションの作成[^4]
[^4]: 出典 https://docs.github.com/ja/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-collapsed-sections

details ブロック内のすべての Markdown は、閲覧者がクリックして詳細を展開するまで折りたたまれたままです。

<details>

<summary>折りたたまれた内容の要約をここに書く Tips for collapsed sections</summary>

### You can add a header

summary ラベル内の Markdown は、既定で折りたたまれます。

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>

<details open>

セクションを既定で開いているように表示するには、open 属性を details タグに追加します:

</details>

GitHub のすべてのコメント フィールドで固定幅フォントを有効にすることができます。

- GitHub で、任意のページの右上隅にある自分のプロフィール写真をクリックしてから、 [設定] をクリック
- 左側のサイドバーで、[ 外観] をクリック
- [Markdown editor font preference](Markdown エディターのフォント設定) で [Use a fixed-width (monospace) font when editing Markdown](Markdown の編集時に固定幅 (等幅) フォントを使用する) を選びます。 
- <details>https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github#enabling-fixed-width-fonts-in-the-editor</details>

プレビューは メモ帳でも可能。

出典
https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

