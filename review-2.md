# Bolt
## 修正内容

  ##
  1．div Maintext～は不要
  →79行目にあった>OUR SKILLSの<Maintext～>のdivを削除しました。

  2．marginとpaddingをつける位置を直す
  →子要素でmarginをとって親要素の隙間を取っていた部分がありましたので、
  背景色を指定している要素＝親要素にpaddingを指定しました。

　3．headerのflexのいらないタグを消す
　→align-items: center;は不要であったため削除しました。

  4．73行目のEmailボタンの上をテキストと揃える
  →vertical-align: top;でテキストと一緒に上を揃えました。
  
  5．<a>タグに<a href="">をつけてcursor: pointer;を削除する
  →すべての<a>タグに<a href="">を追加しました。
  CSSでのcursor: pointer;は不要となるので削除しました。
  
  6．<h3>タグを<h2>タグに直す
  →>OUR SKILLSの部分です。<h2>に修正しました。

  7．＜p class＝"item_our_skills_Subtext">を
  　　items_our_skills　p　に変更する
  →変更しました。『class＝"item_our_skills_Subtext"』の部分は削除をしました。

  8．inner_headerのbox_sizingを消す
  →不要なプロパティでしたので削除をしました。

  9．innerとinner～は一緒のdivには入れない。
  　　また、inner～の名称はtitle～に変更をし、
　　　titile～の中身はinnerに移す。
　　　inner～は削除する。
→innerに width: 1100px;、 margin: auto;を指定して共通のクラスでコンテンツ幅、中央寄せを指定しました。
また、Giztech内にて「背景色は画面いっぱいにする」といった内容を各セクションの
title～、～wrapperに指定して、innerの上に配置しました。