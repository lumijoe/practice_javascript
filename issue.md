先にリンクさせたいファイル名を記述して、ファイルが存在していなければ自動で作成してくれる機能を使用する
　 - ファイル名を保ヴァーして com+クリックすると作成するか問われるので yes で実行するとディレクトリ構造も構築してくれる

**参考コード**

if (scroll < posTop - windowHeight + windowHeight / 2 + 100 || scroll > posTop + windowHeight / 2 - 100) { // // 下へ画面 1/2 || 上へ画面 1/2 スクロールした時消える処理
// section の見出しアニメーション
$('section').each(function() {
var posTop = $(this).offset().top; // 各 section の上部座標
var posHeight = $(this).outerHeight(); // 各 section の高さ
var windowHeight = $(window).height(); // ウィンドウの高さ

      console.log(Math.floor(scroll));

      if (scroll < posTop - windowHeight + windowHeight / 2 + 100 || scroll > posTop + windowHeight / 2 - 100) { //   // 下へ画面1/2 || 上へ画面1/2 スクロールした時消える処理
        $('.section_header', this).slideUp();
      } else { // 現れる処理
        $('.section_header', this).slideDown(500);
      }
