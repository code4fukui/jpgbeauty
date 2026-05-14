# jpgbeauty

Web向けにサイズの大きいJPGおよびPNGファイルをリサイズ・圧縮するクライアントサイドツールです。すべての処理はブラウザ内で完結し、サーバーへのファイルアップロードは行われません。

## デモ

**https://github.com/code4fukui/jpgbeauty

## 機能

-   **ブラウザ内処理:** サーバーへアップロードすることなく、ローカル環境で安全に画像を最適化します。
-   **一括変換:** 複数のファイルをドラッグ＆ドロップして、一度に処理できます。
-   **スマートリサイズ:** 画像の寸法を、指定した最大幅または最大高さに縮小します。
-   **PNGからJPEGへの変換:** サイズや寸法の制限を超えたPNGファイルを自動的にJPEGへ変換します。
-   **品質コントロール:** JPEGの圧縮品質を調整できます（0.0〜1.0）。
-   **色空間の管理:** Webでの互換性を高めるため、オプションでsRGB色空間へ強制変換できます。
-   **ファイルサイズ制限:** 指定したキロバイト数のしきい値を超える画像に対して変換を実行します。
-   **自動ダウンロード:** 最適化された単一の画像を直接ダウンロードするか、複数の画像をZIPアーカイブにまとめてダウンロードします。

## 使い方

1.  ページ上のドロップゾーンに1つ以上のJPGまたはPNGファイルをドラッグ＆ドロップします。
2.  必要に応じて設定を調整します:
    -   **最大幅/高さ (px):** 出力画像の幅または高さの最大ピクセル数。
    -   **品質 (0-1.0):** 変換後の画像のJPEG品質。`1.0`が最高品質です。
    -   **sRGBを強制:** 出力画像にsRGB色空間を適用する場合はチェックを入れます。
    -   **最大サイズ (kbyte):** このサイズを超える画像は再圧縮されます。
3.  処理されたファイルは自動的にダウンロードされます。複数のファイルをドロップした場合は、1つの `jpgs.zip` ファイルとして保存されます。

## 依存関係

このアプリケーションは、以下のオープンソースライブラリを使用して構築されています:

-   [ImageUtil.js](https://github.com/code4fukui/ImageUtil) - コアとなる画像操作ユーティリティ。
-   [exif-js](https://github.com/taisukef/exif-js) - 画像からEXIFメタデータを読み取るためのライブラリ。
-   [downloadZip.js](https://github.com/code4sabae/js/blob/master/downloadZip.js) - ZIPアーカイブの作成とダウンロード用。
-   [waitDropFiles.js](https://github.com/code4sabae/js/blob/master/waitDropFiles.js) - ファイルのドラッグ＆ドロップイベントの処理用。
-   [downloadFile.js](https://github.com/code4sabae/js/blob/master/downloadFile.js) - 単一ファイルのダウンロード実行用。
-   [readAsArrayBufferAsync.js](https://github.com/code4sabae/js/blob/master/readAsArrayBufferAsync.js) - ローカルファイルの非同期読み込み用。
-   [Bootstrap](https://getbootstrap.com/) - UIのスタイリング用。

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) を参照してください。
