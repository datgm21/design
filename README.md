# 2021年度生 ゲームデザイン実習
- [シラバス](https://drive.google.com/file/d/1dIiRItttkABdvisRGQuZwYjKLJt8mgSJ/)
- [質問](https://meet.google.com/nfe-tjom-mtb)
- [昨年度の講義資料](https://github.com/datgm20/design)
- [Slack](https://datgm21.slack.com)

# 参考URL
## 企画
- [Jesse Schell's ゲームデザインレンズデッキ](http://deck.artofgamedesign.com/#/?lang=jp)
- [マミーさん. チーム「密会取り締まり委員会」の発表](https://youtu.be/-qWwYVWgczA?t=6093)・・・ブレストの例 / チーム開発について
- [EIKIさん. ゴリラが人類を強制的にSTAY HOMEさせるゲーム](https://youtu.be/-qWwYVWgczA?t=6719)・・・アイディアの転がし方、発注、ペース、進め方
- [tnkさん. 「斬新さ」から考えるゲーム開発](https://youtu.be/-qWwYVWgczA?t=3002)・・・プランナー的視点、斬新なアイディア
- [#TokyoIndies on Twitter](https://twitter.com/hashtag/TokyoIndies?src=hashtag_click&f=live)

# 9回目
## 予定
- clusterのアップデート
  - スタートメニュー > `cluster`と入力 > clusterを起動
  - アップデートをクリック。管理者権限が必要なので教員を呼ぶ
  - ワールドを確認
- Unity2019.4.11f1 に WebGL モジュールを加える
- [よけとる](https://datgm20.github.io/OpenYoketoru2020/WebGL/index.html)のプロジェクト作成と素材集め
  - マウスで操作
  - 10秒以内にコインを全て取ればクリア
  - トゲの甲羅にぶつかるか10秒経過でゲームオーバー
- [よけとるUnityプロジェクトの作成](https://docs.google.com/document/d/1rk3klNfDD5tlQ0CpZVt34NibBh50MT6dYGDpHXmbCPw/)
- 素材はなるべくCreative Commonsなどの再配布可能なものを探す


# 8回目
## 内容
- [著作権概論](https://docs.google.com/document/d/15zRG0hcf9OU3TFoJ5vZL43AGPKCqewpD7KS_QYwntaA/edit?usp=sharing)
- 演習：素材サイトの調査
- 15:20から筆記試験

## 演習
- 利用可能なフリー素材サイトを探してSlackにURLを貼って共有しよう。また、以下について利用規約を調べてコメントする
  - 利用条件(著作者表示やURLの記載など)
  - 商用利用の可否
  - 再配布の可否

## 筆記試験
- 15:20 準備
  - PCの電源を切る
  - 座席を移動
  - スマホなどはカバンに入れて、かばんは足元
  - 机の上は筆記用具のみ
  - **問題用紙には何も書かないこと**
- 15:30 試験開始
- 15:50 試験が終わった者は、提出して退室可
- 16:10 試験終了


# 7回目
## 話題
- [日本ゲーム大賞 U18部門. 2021予選大会進出作品](https://u18.awards.cesa.or.jp/qualifying2021/)

## GitHubのPush失敗について
- GitHubはフリープランでLFSというものを使わない場合、1つのファイルのサイズが100MBまでに制限される
- うっかり100MBを越えるファイルをコミットしてしまうと、GitHub DesktopではPushもできず、取り消しもできなくなる(`git rm --cached <ファイル名>`をコマンドで実行すれば取り消せる)
- 手軽な解決策
  - 現在のプロジェクトフォルダーの名前の最後に`.bk`などを付けて名前を変える
  - プロジェクトフォルダーを開いて、容量をオーバーしているファイルと、`.git`フォルダーを削除
  - GitHub Desktopに切り替えると、リポジトリーが見つからなくなるのでエラーが表示されるので、メニューの中の Clone Again をクリックして、クローンをし直す
  - `.bk`をつけたプロジェクトフォルダーの中身をコピーして、クローンし直したプロジェクトフォルダーに上書きコピー
  - Unityでプロジェクトを開いて、問題がないことを確認

以上で問題は解決するので、コミットとプッシュをし直す。全ての作業が問題なく完了したら、`.bk`をつけた元のプロジェクトフォルダーを削除して完了。

## 内容
- [写真のデザイン](https://am1.jp/dat/design/design6-photo.pdf)
  - [図](https://am1.jp/dat/design/design6-photo-fig.pdf)

## 演習準備
### Unityのプロジェクト作成とGitHubへの登録
- プロジェクト名を`PostProcessPrac`、**3D**でUnityプロジェクトを作成
- *File*メニューから*Save Project*を選択して、プロジェクトを保存

## 演習
- コーネルボックスを作る
  - [monobook.org. コーネルボックスとは](https://monobook.org/wiki/%E3%82%B3%E3%83%BC%E3%83%8D%E3%83%AB%E3%83%9C%E3%83%83%E3%82%AF%E3%82%B9)
- [作業手順](https://docs.google.com/document/d/1PhYwUOJd5xHd2JtDEFSgeMRXTd7xlZ3Nv3ANUAR9rn0/)
  - SphereやPlane、ボックスなどを配置して着色
  - 様々なライトを試す
  - カメラの画角(Field of view = 視野角)
  - ポストプロセスによる被写界深度(ボケ)の表現、HDR(High Dynamic Range)による輝き
    - [設定手順](http://am1tanaka.hatenablog.com/entry/2018/05/19/172121)
- できたらスクリーンショットをSlackの自分のチャンネルに貼り付け

## 時間があれば...
- これまでのおさらい
- 前回の画面にさらに手を入れる

## ライティングについて参考
- [Unity公式. ライティングの手法](https://docs.unity3d.com/ja/current/Manual/BestPracticeMakingBelievableVisuals3.html)
- [テラシュールブログ. Lightmap](http://tsubakit1.hateblo.jp/archive/category/Lightmap)
- [テラシュールブログ. 画面効果](http://tsubakit1.hateblo.jp/archive/category/%E7%94%BB%E9%9D%A2%E5%8A%B9%E6%9E%9C)


# 6回目

## 内容
### フォント。UI
- [文字のデザイン](https://am1.jp/dat/design/design5-font.pdf)
  - [図](https://am1.jp/dat/design/design5-font-fig.pdf)

## 演習
- 前回の演習で作成したモック画面のオブジェクトの調整とUIを追加して画面をまとめる
- [第3回](https://docs.google.com/document/d/1U0DTbG__KQNiOBQCGeCm2Ty7IiBCMrEJgIMEMfH3MZk/)の演習で、Googleスライドで作成した企画に、現在作成しているUnityの画面を貼り付けて、タイトル、操作方法、ルールなどを記入して、企画書をバージョンアップさせる
- https://drive.google.com を開いて、Googleアカウントでログインして、3回目に作成したGoogleスライドを開いて追記する

### レイアウトのヒント
- [Anna Mészáros. デザイナーではない人がデザインする上で大切な4つの基本原則](https://gigazine.net/news/20190518-fundamental-design-principles/)
- [個人開発のUI設計術](https://crieit.net/posts/UI)
- [PHOTOSHOPVIP. 現役デザイナーが教える！完璧な書体を決める10個の黄金ルールまとめ](http://photoshopvip.net/105840?utm_content=bufferf79a8&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)
  - プロジェクトのテーマを明確化して、それに合うものを選ぶ
  - フォントのフォルム（太さ、丸み、縦横比)はある程度揃えつつ、違いがあるもの
  - 1つのプロジェクトで、タイトルと本文、あるいはタイトルとUIと本文といった、2種類以上のフォントを選ぶ

### 作業
- [作業メモ](https://docs.google.com/document/d/17JeqgPwlUDYiSMXUpmc9umw6ip8CC536H8jKA6yt5O4/)
- [coliss. 2021年用、日本語のフリーフォント477種類のまとめ -商用サイトだけでなく紙や同人誌などの利用も明記](https://coliss.com/articles/freebies/japanese-free-fonts.html)
  - タイトル用と本文用の2つのフォントを見つける。**URLをGmailの下書きやGitHubのREADME.mdに記録しておく**
- [UnityのUI基礎](https://docs.google.com/document/d/1oUDdWBGk2XUjAyt7RLHL2a1shBwrZp-ghrOb4wzGddk/)
  - [TextMeshProの使い方](https://docs.google.com/document/d/1XIBCeH27Os43a1epTxYArBBaRK8iTLLIgwG0m4FrUTA/)
  - [TextMeshPro向け　ASCIIコード＋JIS第1水準の文字](http://am1tanaka.hatenablog.com/entry/2019/10/14/183408)
- タイトル用のフォントは、使用する文字だけでフォントアセットを作成。サイズは48で、フォント画像サイズは全ての文字が収まる最小のサイズ
- スコアやメッセージ用フォントは、JIS第１水準の文字全て作成。サイズは24〜28ぐらいで2048x2048に収まるように調整

### キーワード
- 抽象化
- 記号
  - アイコン
    - 対象の形を抽象化した記号
  - インデックス
    - 対象を連想させる記号
  - シンボル
    - ！や？など、共通認識がある記号
- モノグラム
- 点、線、面
- 幾何学形態の利用
  - 図形間の距離、大きさ
  - 図形の形状、配置
  - 黄金比、白銀比
- 図と地、ゲシュタルト心理学、プレグナンツの法則
- 錯視

### 提出
- Googleスライドを共有済みなら更新したら自動的に提出になる
- 3回目にスライドを未提出の場合は、[こちら](https://docs.google.com/forms/d/e/1FAIpQLScc9scLVvYA8nCuFTSHURvQtOBTEZL2bilB6GWgb78jMYkgFA/viewform?usp=sf_link) に共有URLを登録


# 5回目(5/26)

## 話題
- [Gotanda.unity #18 sponsored by ワンダープラネット株式会社](https://meetup.unity3d.jp/jp/events/1302)

## 内容
### 前回の振り返り
- レイアウトと色
- Slackの企画を流し見

### 形を整える
- [手順](https://docs.google.com/document/d/1-stU_T0KyyxKqNC-rBmSxjMAEWN9zsHpweHtlhiI35Q/)
- [形のデザイン](https://am1.jp/dat/design/design3-shape.pdf)
- [Unityの新規プロジェクトの作成とGitHubへのパブリッシュ](https://github.com/datgm20/gp1/blob/master/github-unity.md)
  - 前回のプロジェクトを登録
  - [こちら](https://docs.google.com/forms/d/e/1FAIpQLScc9scLVvYA8nCuFTSHURvQtOBTEZL2bilB6GWgb78jMYkgFA/viewform?usp=sf_link) にリポジトリーのURLを登録
- [ProBuilderでシンプルな形を作る](https://docs.google.com/document/d/129pS_YQPJq3srmxEqCDMUX8a9aqGGnTy0OzaEPsajXU/)


# 4回目(5/19)
## 内容
- レイアウト [FOTORIA. 三分割法で写真の構図をバッチリ決定！イラストで撮影方法を解決](https://fotoria.net/ja/blog/bc/photo-shoot-techniques/sc/composition/ar/rule-of-thirds/)
- [色とUIのデザイン](https://am1.jp/dat/design/design4-color.pdf)
  - [図](https://am1.jp/dat/design/design4-color-fig.pdf)
  - [作業メモ](https://docs.google.com/document/d/1a_rWW82Q9g_PDXjtlKHyY_NooInNXocj35WYJJ-JyT4/)

## 演習　球体や立方体でハイパーカジュアルゲームなどの描きこまれていないオブジェクトで構成された画面を作る
- 先週提出された企画案をベースにすると良い
  - 先週の案が描きこまれたキャラものだったり、ない場合は、スマホやPCでPlayストアやAppストアを開いて、モデルにしたいゲームを選ぶ。その際、ゲームの提供元、タイトル、URLを調べてSlackに書き込む
  - 例
    - [Monument Valleyシリーズ](https://www.ustwogames.co.uk/)
    - [Bounce and collect](https://apps.apple.com/jp/app/bounce-and-collect/id1553875472)
- [Unityでレイアウト作成](https://docs.google.com/document/d/17WatyZDngqasXH0k6hKGg8V-_9kEqqOViAhxmiuofhI/)
  - アスペクト比を決める
  - ライト設定
  - 背景色
  - プリミティブの作成
  - マテリアルの作成
  - カメラの設定
  - 文字表示-TextMeshPro
  - 親子階層
- できたらスクリーンショットを撮影してSlackに貼り付け


# 3回目(5/12)
## 内容
- [ゲームメカニクス](https://docs.google.com/document/d/1U0DTbG__KQNiOBQCGeCm2Ty7IiBCMrEJgIMEMfH3MZk/)


# 2回目
## 話題
- [集英社ゲームクリエイターズCAMP](https://game-creators.camp/)
- [1週間ゲームジャム. テーマ「2」 5/2(日)20:00公開開始](https://unityroom.com/unity1weeks)

## 内容
- 講義：[ゲームデザインの基礎](https://docs.google.com/document/d/1ItqVAv-e-dnThzUF1o-8xucq7l95gel6FF9-96kBkpo/)
- [Jesse Schell's ゲームデザインレンズデッキ](http://deck.artofgamedesign.com/#/?lang=jp)のカードリストを眺める

## 演習２：ブレストで出た方向性を土台に以下についてまとめる
- [ブレスト結果](https://docs.google.com/spreadsheets/d/16dN31zI6sNFDMfeY0mZebofRX8BSpbv6eQbpZ7Q4Ed8/)
  - 上のリンクを右クリックして新しいタブで開く
  - ファイルメニューから、コピーを作成 を選択
  - 適当な場所を選択して保存
  - フォームの下のタブから自分のグループを選択
  - B列を選択
  - ▼アイコンをクリックして、A-Zでシートを並び替え　を選択
  - 上から3つのキーワードをテーマにして、企画書を作成する
- https://drive.google.com を開く
  - 左上の新規ボタンを押す
  - Googleスライドをクリック
  - 無題のスライド の部分をクリックして、「企画演習：氏名」と入力。氏名の部分は自分の名前
  - 先ほど選択したキーワードをスライドに貼り付ける
  - 演習にあるような項目を記載していく
  - 手書きか、図形で画面のサムネイルを作成
- ゲームデザインレンズデッキの1～5を参考に、方向を決める
- 手書き、PowerPoint、Photoshopなど何を使ってもよいので、ゲームの画面案を描く
  - 最初はそれぞれ別々に描いて、方向性が合っているかを確認してみるとよい
  - 参考： [ArtStation. Gameplay & Level Design](https://www.artstation.com/channels/gameplay_and_level_design?sort_by=trending)
- 画面案をGoogleスライドに書き込む
- 以下の項目をGoogleスライドにまとめる
  - コアステートメント
  - ゲームのコードネーム(仮のタイトル)
  - 具体的な操作方法
  - ルール(何をやるのか。あるいは、どうなったらダメなのか。など)
  - 世界観(いつ、どこ、だれ。ハイパーカジュアル系など、これがないものもあるので、ない時はなしでよい)
- 考えるヒント
  - プレイヤーが「これは面白い！」と感じる瞬間を決める
  - そのように感じる理由を考える
  - その理由を最大に強調するための操作方法、ルール、ステージ、設定などを考える
- 参考： [nekogeek. カジュアルゲームの最新ゲームを50本遊んで、企画の方向を考えよう](https://nekogeek.jp/play-casual-games-a-lot/)
  - [作例](https://docs.google.com/presentation/d/1pU7q1oWEkPfATbvy5jhatJkDWsByfO3wpBh1KIKShrk/)

## 演習１：グループでアイディアを出し
- 準備
  - [Slackに登録](https://docs.google.com/document/d/1Tu8rrbJDmAERo_ItkfcmadOinEFiTcuKmOq07ycH0G0/)
  - グループのチャンネルに参加
- ブレストの前に
  - [マミーさん. チーム「密会取り締まり委員会」の発表](https://youtu.be/-qWwYVWgczA?t=6093)・・・ブレストの例 / チーム開発について
  - [EIKIさん. ゴリラが人類を強制的にSTAY HOMEさせるゲーム](https://youtu.be/-qWwYVWgczA?t=6719)・・・アイディアの転がし方、発注、ペース、進め方
  - [tnkさん. 「斬新さ」から考えるゲーム開発](https://youtu.be/-qWwYVWgczA?t=3002)・・・プランナー的視点、斬新なアイディア
- ブレスト
  - [面白法人カヤック. 始まりも終わりもブレスト](https://www.kayac.com/vision/brainstorm)
  - テーマ「2」


# 1回目
- [ガイダンス](https://drive.google.com/file/d/1tvOISbFwll-c7fmJ7qJVIciTp3ZknSEr/)
  - [とあるツイート](https://twitter.com/toRisouP/status/1381522737265451009)
  - [Jini. 子供を地獄かもしれない世界へ誘った理由](https://note.com/j1n1/n/n8ee2242cecc3)
- [環境の準備](https://docs.google.com/document/d/16MW6maMYvt8m-60RM5wU_LzJ5r-3Hm0WTnxoBGDzxIA/)
  - Googleアカウント / Slack / Google Meet / GitHub / 作業用フォルダー
  - ツールについて
    - プログラムやアプリの使い方の管理、文章作成者が決まっているようなもの：GitHub
    - 大きな画像や動画など：Googleドライブ
    - 意見交換が主体で、将来的に消えてもよい質疑応答や進捗の共有、ブレストなど。クラス以外には非公開：Slack
    - 企画書や仕様書、確認事項など、手軽に共有したり編集できて残しておきたい文章：Googleドキュメント、ワークシート、Trelloなど
- 講義：ゲームの定義
  - [Capm Network. ゲーム理論](http://capm-network.com/?tag=%E3%82%B2%E3%83%BC%E3%83%A0%E7%90%86%E8%AB%96)
  - [スライド:ゲームの定義や要素からミニゲームを考える](https://docs.google.com/presentation/d/1_psbxg6vPk21C3nAcytyVJm8QTYr-G7AV1qAtjcRclg/)
  - [Unity Learning Material. たのしさの作り方 ](https://learning.unity3d.jp/2618/)
- 演習：ミニゲームを考えてみよう
  - Googleドキュメント、スライド、ワークシートのいずれか
  - 共有URLをSlackの自分のチャンネルに書き込む
- 演習：キータイプ練習
  - 今日の結果を[こちら](https://docs.google.com/forms/d/e/1FAIpQLSdJ-8EnCFRQN9on10anfD2I3JQi9FExL7IOQ4QuerKPKm-BIQ/viewform?usp=sf_link)へ報告
