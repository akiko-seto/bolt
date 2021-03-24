
# Bolt PC
## 修正内容

## header
1. HTMLで余計なタグがありそうですね！下記のように変更しましょう！
   また、 `.header_icon` => `header_inner` にrenameしましょう！
   そして `max-width: 1100px` の指定も必要ないです！
   ```html
  <header>
    <div class="title_header">
      <div class="inner">
        <div class="header_icon">
          <i class="fas fa-bolt icon_bolt"></i>
          <a href="" class="Contact_buttom header_buttom">Contact</a>
        </div>
      </div>
    </div>
  </header>
  ↓
  <header class="title_header">
    <div class="inner header_inner">
      <i class="fas fa-bolt icon_bolt"></i>
      <a href="" class="Contact_buttom header_buttom">Contact</a>
    </div>
  </header>
  ```
  -
　 header_icon => header_innerに名前を変更しました。
　　また`our_skills_wrapper`⇒`our_skills_inner`
　　にて名称を変更しております。

   style.cssの29行目max-width: 1100px;を削除しました。

   また余計なタグに関してはfooter_textとour_skills_wrapperにございましたので、削除をしています。
​
2. `contact` ボタンに下線が出現しています...!!
   `text-decoration` で消しましょう！

   →`Contact_buttom`に`text-decoration: none;`
   　を追加して、ヘッダーのcontactボタン
   　Emailボタンの下の線を消しました。
​
​
## Bolt Theme
OK!!
​
​
## WHAT WE CAN DO?
1. `.inner` と `flex_inner` は同じdivタグに指定してOKかな！
　-`inner`と`flex_inner`を同じdivに入れて、閉じタグを一つ削除しました。
​
​
## OUR LATEST WORK
1. aタグを確認してもらうと、要素の高さが正確に取れていません！
   aタグがインライン要素なのが原因なので、 `display: inline-block` を適用しましょう。
   ```css
   a {
     display: inline-block;
   }
   ```

   -aタグの高さがつぶれていたので、上記の記載の通りに
   aタグをインラインブロック要素にしました。
   また、もともと`sns_incon_list li a `で

  width: 100%;
  height: 100%;
  display: block;

  と記述していた内容は今回追記した内容によって不要となりますので削除をしました。

​
2. `.Sub_content`の上下のpaddingは必要ないです！
   6枚画像との隙間が欲しければ`margin`でとりましょう！
  
  -`Sub_content`の上の隙間を `margin-top`で取るようにしました
  また、下側のpaddingでとっていたものは`title_our_latest_work`で取るようにするために
   `padding: 60px 0 70px 0;`に変更しました。
​
3. `Email Me` ボタンの下線消しましょう！
  -上記の"Contact_button"に"text-decoration: none;を一緒に指定して消しました。
​
​
## OUR SKILLS
1. liの子要素のpタグで指定してる`margin-bottom`は適切じゃないね！
   セクション自体の背景色を広げたいのだから、 `.title_our_skills`
   のpadding-bottomでとるべきですね！

   -`.items_our_skills p`で指定していた`margin-bottom:100px`を削除し、親要素の`title_our_skills`にて下の幅をpaddingで広げました。

   毎回修正箇所が多く申し訳ございません。
   宜しくお願い致します！