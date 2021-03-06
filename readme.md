# よくある見出しを自動生成

[https://10daisuke64.github.io/heading_maker_2/](https://10daisuke64.github.io/heading_maker_2/)

## 追加機能

- 各カード内の星アイコンをクリックすると、お気に入りに登録され、ヘッダーの「お気に入り」ボタンから絞り込みができる。絞り込み機能は「Muuri.js」を使用
- 各カード内のコードアイコンをクリックすると、モーダルウィンドウが立ち上がり、該当するGoogle Fontsを読み込むlinkタグとCSSをコピーできる
- 各カード内の文言はinputタグになっており、書き換えることが可能で、全カードに反映される（ヘッダーの入力欄は廃止）
- 需要は多分ないけどレスポンシブ対応

## 必要な改善点

- Safariでレイアウトがガン崩れする

## プロダクトの紹介

- 普段WEBデザインの仕事をしていて、欧文＋日本語（Google Fonts縛り）を組み合わせた見出しデザインを作ることが頻繁にある
- そのパターンがマンネリ化してきたので、新しい組み合わせを発見するため、見出しを自動生成するツールを作った
- 自分の使いたいfont-familyとfont-weightをGoogle Fontsで検索し、JavaScript内の配列に格納
- フォントを読み込むlinkタグが自動生成され、ブラウザ上には60個の組み合わせサンプルが自動生成される

## 工夫した点，こだわった点

- サンプルをクリックするとCSSが出てくるのでコピー可能
- ヘッダー右の入力欄からサンプルに表示させる文言を変更可能、また、更新ボタンも実装

## 苦戦した点，共有したいハマりポイントなど

- 変数に格納したテキストと文字列を連結させまくることで、linkタグやCSSを生成しているので、記号の記述ミスなどで詰まることがあった
- 良いと思ったサンプルをお気に入り登録できたり、お気に入りをソートしたり、italicに対応したり、拡張の余地はまだまだあるなと思う
