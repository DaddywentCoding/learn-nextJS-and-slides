SwiperのSlideを利用してカレンダ形式で表示させた。


Deploy後Slidesが動作しない。
原因はGitHub Pagesはjekyllというもので生成されるが、
こいつが_nextのようなフォルダを無視する特徴がある。

なので_next 配下の CSS や JS の static ファイルが 404 になってしまう。
.nojekyll ファイルを生成してjekyllを無効にできる。
.nojekyll ファイルは中身はなし。
