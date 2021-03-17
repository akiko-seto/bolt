# Bolt
## 修正内容

  ## header
  1.<header class="inner inner_header">を二つに分ける
  - divを追加して<header>を単体にしました。

  ## Bolt
  1..main「title_Bolt_Theme」 の閉じタグが足りない
  - 閉じタグ追加しました。

  2.<div class="Words_title_Bolt_Theme">はいらないinnerにつける
  - <div class="Words_title_Bolt_Theme">についていたプロパティをinner_title_Bolt_Themeに移動しました。

  3.height: 640px;はいらない
  - 消しました

  ## OUR LATEST WORK

  1.<article> にclass="title_our_latest_work">
  - クラスを指定し、子要素にありましたdivをひとつずつ削除しました。<section>も同様に行っています
  
  2.Sub_contents、親要素でpaddingをとる
  - テキスト（子要素）をmarginで上下の余白をとっていたため、親要素で隙間をとりpaddingに変更しました。
  横の隙間は兄弟要素の隙間になるのでmarginのままです。

  ## sns

  1.要素内の隙間はpadding
  - marginからpaddingに変更しました。

  2.親要素のheightはいらない
  - 消しました。

  3.liの改行(見やすくするため)
  - <li></li>の間で改行して見やすくしました。


  ##　全体にかかわること
  1.セクションごとの footerを参考に、高さ(padding)をinnerで統一する
  - padding、背景色を各見出しにありますinner～のクラスに統一しました。
　　title～には幅を指定しています。
　　それに伴い、90行目<div class="sns_wrapper">、33行目　　<section>タグにクラスを追加し、一部divを削除してます。



2. 修正指示を記載します(メンター)
  - 修正内容を記載してください(研修生)