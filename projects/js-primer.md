# JavaScriptの入門書
> https://github.com/asciidwango/js-primer

js-primerは、JavaScriptの入門書です。
この書籍は、これからJavaScriptを始める人がECMAScript 2015以降をベースにして学べることを目的にして現在進行系で書かれています。
JavaScriptは変化を取り入れている言語であるため、JavaScriptの変化に対して対応できる基礎をつけることが目的です。

この書籍の特徴として、書いている最中から[GitHub](https://github.com/asciidwango/js-primer)上にオープンソースとして公開している点が挙げられます。
書籍としての出版予定はありますが、技術書においてオープンソースとして公開することが、書籍の販売にマイナスの影響を与えることは少ないと考えているためです。

また、変化が激しいウェブやJavaScriptについて扱うものが、年単位でしか更新できない媒体でのみ扱うことは適切だとはいえないためです。
そのため、GitHub上で常に最新となるように更新し、スナップショットとして書籍を出版することを目指して書かれています。

規模が大きな文書であるため、文章のメンテナンス性をするためにさまざまな仕組みを取り入れています。
textlintによる文章の自動チェックを行い、機械的にある程度の間違いを発見できる仕組みをCIで回しています。
また、技術書であるため文章中のサンプルコードの挙動は常に正しい挙動でなければいけません。
そのため、ESLintでの静的な構文チェック、コメントに書かれた値と実行結果が一致するかを比較するDocTestなどを取り入れています。
これらの文章中のコードに対してチェックする仕組みが一般にはなかったため、その仕組み自体を作成しています。

オープンソースとして公開する上で、そのプロジェクトの透明性は当事者以外にとっては大切です。
プロジェクトがどのようなフローで意思決定されているのか、何を目指しているのかが明確ではないと、
そのプロジェクトに外部の人がコントリビュートしにくいためです。

そのため、js-primerではGitHub IssueやPull Requestを積極的に利用しています。
また、コントリビュートガイドラインの整備、意思決定を行ったミーティングノートの公開などを行い透明性を確保することを意識しています。
2016年10月17日現在で、GitHub Star 438に対してWatch 184となり、Watchの比率が高く興味を持っていただけていると考えています。

このプロジェクトにおいて、JavaScript初心者にも分かりやすくなるように気をつけるとともに、正確な表現をすることを心がけています。
正確な表現をするためには、JavaScriptの仕様であるECMAScriptの仕様書を読む必要があります。
仕様書の表現そのままでは分かりやすいとはいえないため、繰り返し書き直し分かりやすくしていく必要があります。
このプロジェクトにおいて、機械的に間違いを見つけやすくする仕組みは、その繰り返し行う試行錯誤の過程を補助してくれることを学びました。