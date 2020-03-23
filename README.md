# AR.jsでImage Trackingが可能になったのでテスト

参考にしたのは以下のサイト。

## Introducing AR.js 3
https://medium.com/chialab-open-source/introducing-ar-js-3-bb27ffa1b59c

## AR.js Documentation
https://ar-js-org.github.io/AR.js-Docs/

## AR.js ではじめる Image Tracking
https://qiita.com/ikkou/items/d4711eb74afa000ea481

### 以上のサイトで触れられてはいながはまった点

- NFT Marker Creator (https://carnaux.github.io/NFT-Marker-Creator/) で、Image Descriptorを作成する際、「Generate」ボタンを押しても、私の環境のChrome（最新版）では、.fset3しかダウンロードできず失敗した。Firefoxでは３ファイル生成された。
- HTMLに記述するのはこれら３ファイル拡張子の前（共通）だが、サイトには３ファイルともアップロードしないといけない(はず？）。最初Chromeで１ファイルしかできないのでそれのみでやってみたが当然のことながら失敗した。
- サンプルをそのまま載せてみても恐竜が現れない。もしかしてGithubだとうまくいかない？ raw.githack.comなど試してみたが動かない。
- よく考えれば、対象コンテンツがサンプルは３D。そこにそのまま動画を入れようとしてた。それでは当然だめ。
- サンプルに、nft-videoというディレクトリがあり、そこに動画を再生するサンプルがあった。Ver. 3の公開前にTwitterでチラ見せしていたやつだった。
- そこで本家をfolkして（EasternCloud/AR.js）、動画部分だけをYouTubeにしてみたが動かず。重すぎるからかと少し待ってみたが、Loadingが終わっても黒い画面のままだった。
- 仕方なく動画を同一フォルダに入れてみたら、やっと動いた。
