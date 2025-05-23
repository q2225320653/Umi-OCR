<p align="left">
    <a href="README.md">
        中文
    </a>
    <span> • </span>
    <a href="README_en.md">
        English
    </a>
    <span> • </span>
    <span>
        <b>日本語</b>
    </span>
</p>

<p align="center">
  <a href="https://github.com/hiroi-sora/Umi-OCR">
    <img width="200" height="128" src="https://tupian.li/images/2022/10/27/icon---256.png" alt="Umi-OCR">
  </a>
</p>

<h1 align="center">Umi-OCR</h1>

<p align="center">
  <a href="https://github.com/hiroi-sora/Umi-OCR/releases/latest">
    <img src="https://img.shields.io/github/v/release/hiroi-sora/Umi-OCR?style=flat-square" alt="Umi-OCR">
  </a>
  <a href="https://github.com/hiroi-sora/Umi-OCR/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/hiroi-sora/Umi-OCR?style=flat-square" alt="LICENSE">
  </a>
  <a href="#ダウンロード">
    <img src="https://img.shields.io/github/downloads/hiroi-sora/Umi-OCR/total?style=flat-square" alt="ダウンロード">
  </a>
  <a href="https://star-history.com/#hiroi-sora/Umi-OCR">
    <img src="https://img.shields.io/github/stars/hiroi-sora/Umi-OCR?style=flat-square" alt="スター">
  </a>
  <a href="https://github.com/hiroi-sora/Umi-OCR/forks">
    <img src="https://img.shields.io/github/forks/hiroi-sora/Umi-OCR?style=flat-square" alt="フォーク">
  </a>
  <a href="https://hosted.weblate.org/engage/umi-ocr/">
    <img src="https://hosted.weblate.org/widget/umi-ocr/svg-badge.svg" alt="翻译状态">
  </a>
</p>

<div align="center">
  <strong>無料、オープンソース、大量文字が一括認識できるのソフトウェア</strong><br>
  <sub>Windows7 x64以上と互換性があります</sub>
</div><br>

- **無料**: このプロジェクトのすべてのコードはオープンソースで完全に無料です。
- **便利**: 解凍して使用し、オフラインで実行し、ネットワークは必要ありません。
- **効率的**: 高効率のオフライン OCR エンジンが付属しています。コンピュータのパフォーマンスが十分であれば、オンライン OCR サービスよりも速くなることがあります。
- **柔軟**: カスタマイズ可能なインターフェースをサポートし、コマンドラインや HTTP API など、複数の呼び出し方法をサポートします。

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ec301b55.png" alt="1-タイトル-1.png" style="width: 80%;"></p>

![1-タイトル-2.png](https://tupian.li/images/2023/11/19/6559909fdeeba.png)

## ソースコードの使用:

開発者は続ける前に、[プロジェクトのビルド](#プロジェクトのビルド)を読んでください

## リリースのダウンロード:

- **GitHub** https://github.com/hiroi-sora/Umi-OCR/releases/latest
- **Source Forge** https://sourceforge.net/projects/umi-ocr
- **Lanzou (蓝奏云)** https://hiroi-sora.lanzoul.com/s/umi-ocr

<details>
<summary><b>• Scoop インストーラー</b></summary>

[Scoop](https://scoop.sh/) はWindowsで動作するコマンドラインインストーラーで、複数のアプリケーションを簡単に管理できます。まず Scoop をインストールし、次に以下のコマンドを使用して `Umi-OCR` をインストールしてください：

- `extras` バケットを追加：
```
scoop bucket add extras
```

- （オプション1）Umi-OCR をインストール（ `Rapid-OCR` エンジン付属、互換性が高い）：
```
scoop install extras/umi-ocr
```

- （オプション2）Umi-OCR をインストール（ `Paddle-OCR` エンジン付属、やや高速）：
```
scoop install extras/umi-ocr-paddle
```

- 両方を同時にインストールしないでください。ショートカットが上書きされる可能性があります。しかし、[プラグイン](https://github.com/hiroi-sora/Umi-OCR_plugins) を追加することで、異なるOCRエンジンをいつでも切り替えることができます。

</details>

## はじめに

ソフトウェアリリースパッケージは、`.7z`圧縮形式または自己解凍`.7z.exe`パッケージで利用可能です。自己解凍パッケージは、圧縮ソフトウェアがインストールされていないコンピューターでファイルを抽出するために使用できます。

このソフトウェアはインストールを必要としません。抽出後、`Umi-OCR.exe`をクリックしてプログラムを開始します。

問題が発生した場合は、[Issue](https://github.com/hiroi-sora/Umi-OCR/issues)を提出してください。最善を尽くしてサポートします。

## インターフェース言語

Umi-OCR は、インターフェースの複数の言語をサポートしています。ソフトウェアを初めて開くと、コンピューターのシステム設定に基づいて自動的に言語が切り替わります。

言語を手動で切り替える必要がある場合は、以下の図を参照してください。`全局设置`→`语言/Language`。

<p align="center"><img src="https://tupian.li/images/2023/11/19/65599c3f9e600.png" alt="1-タイトル-1.png" style="width: 80%;"></p>

## タブインターフェース

Umi-OCR v2 は、一連の柔軟で使いやすい**タブインターフェース**で構成されています。好みに応じて必要なタブインターフェースを開くことができます。

タブバーの左上隅を使用して**ウィンドウ常に最前面**を切り替えることができます。右上隅は、日常使用中の偶発的な閉鎖を防ぐために**タブインターフェースをロック**するために使用できます。

### スクリーンショット OCR

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecb4dfb4.png" alt="2-スクリーンショット-1.png" style="width: 80%;"></p>

**スクリーンショット OCR**: このページを開いた後、キーボードショートカットを使用してスクリーンショットをキャプチャし、画像内のテキストを認識することができます。

- 左側の画像プレビューパネルを使用して、マウスでテキストを選択してコピーすることができます。
- 右側の認識レコードパネルを使用して、テキストを編集し、複数のレコードを選択してコピーすることができます。
- 他の場所から画像をコピーして Umi-OCR に貼り付け、認識することもサポートしています。

#### 段落マージ

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecc62ac9.png" alt="2-スクリーンショット-2.png" style="width: 80%;"></p>

**OCR テキスト後処理 - 段落マージ**について: この機能は、OCR 結果のレイアウトと順序を整理し、テキストを読みやすく使用しやすくすることができます。プリセットスキームは以下の通りです。

- **単一行**: 同じ行上のテキストをマージします。ほとんどのシナリオに適しています。
- **複数行 - 自然な段落**: 同じ段落に属するテキストを知的に認識してマージします。ほとんどのシナリオに適しており、上記の図に示されています。
- **複数行 - コードブロック**: テキストの元のインデントとスペーシングを復元しようとします。コードスニペットやスペースを保持する必要があるシーンを認識するのに適しています。
- **縦書きレイアウト**: 縦書きレイアウトに適しています。縦書き認識もサポートするモデルライブラリと併用する必要があります。

---

### バッチ OCR

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecdc5197.png" alt="3-バッチ-1.png" style="width: 80%;"></p>

**バッチ OCR**: このページでは、ローカル画像をバッチでインポートして認識することがサポートされています。

- 認識されたコンテンツは、txt/jsonl/md/csv(Excel)などのさまざまな形式で保存できます。
- `テキスト後処理`技術をサポートし、同じ自然な段落に属するテキストを認識してマージすることができます。また、コードブロックや縦書きテキストなど、複数の処理スキームもサポートしています。
- 一度に処理できる画像の数に制限はなく、タスクを完了した後、ソフトウェアは自動的にシャットダウンまたはスリープすることができます。

#### 無視域

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecbc0021.png" alt="3-バッチ-2.png" style="width: 80%;"></p>

**OCR テキスト後処理 - 無視域**について: これは、バッチ OCR の特別な機能で、画像内の望ましくないテキストを除外するために使用されます。

- 無視領域エディタは、バッチ認識ページ設定の右側の列でアクセスできます。
- 上記の例のように、画像の上部と右下隅に複数の透かし/LOGO があります。これらの画像がバッチで認識される場合、透かしは認識結果に干渉します。
- 右マウスボタンを押し続けて、複数の長方形ボックスを描画します。これらのエリア内のテキストは、タスク中に無視されます。
- 長方形ボックスをできるだけ大きく描画し、透かしのすべての可能な位置を完全に包むようにしてください。

---

### 大量文章のｏｃｒ

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ecc8bfd4.png" alt="" style="width: 80%;"></p>

---

### QR コード

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed01f5b2.png" alt="4-QRコード-1.png" style="width: 80%;"></p>

**スキャンコード**:

- スクリーンショットをキャプチャしたり、貼り付けたり、ローカル画像をドラッグして、QR コードやバーコードを読み取ることができます。
- 1 つの画像で複数のコードをサポートします。
- 以下の 19 のプロトコルをサポートします:

`Aztec`,`Codabar`,`Code128`,`Code39`,`Code93`,`DataBar`,`DataBarExpanded`,`DataMatrix`,`EAN13`,`EAN8`,`ITF`,`LinearCodes`,`MatrixCodes`,`MaxiCode`,`MicroQRCode`,`PDF417`,`QRCode`,`UPCA`,`UPCE`,

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed001437.png" alt="4-QRコード-2.png" style="width: 80%;"></p>

**コード生成**:

- テキストを入力して QR コード画像を生成します。
- **誤り訂正レベル**などのパラメータを含む 19 のプロトコルをサポートします。

---

### グローバル設定

<p align="center"><img src="https://tupian.li/images/2024/03/27/66040ed16f4e0.png" alt="5-グローバル設定-1.png" style="width: 80%;"></p>

**グローバル設定**: ここでは、ソフトウェアのグローバルパラメータを調整できます。一般的な機能には、以下が含まれます:

- ショートカットを一度に追加するか、自動起動を設定します。
- インターフェースの**言語**を変更します。Umi は繁体字中国語、英語、日本語などの言語をサポートしています。
- インターフェースの**テーマ**を切り替えます。Umi には複数のライト/ダークテーマがあります。
- インターフェーステキストの**フォントサイズ**と**フォント**を調整します。
- OCR プラグインを切り替えます。
- **レンダラー**: ソフトウェアインターフェースは、デフォルトで GPU 加速レンダリングをサポートしています。画面のちらつきや UI の位置ずれが発生する場合は、`インターフェースと外観` → `レンダラー`に移動して、異なるレンダリングスキームに切り替えるか、ハードウェアアクセラレーションをオフにしてみてください。

---

## API の使用:

- [コマンドラインマニュアル](docs/README_CLI.md)
- [HTTP API マニュアル](docs/http/README.md)

## プロジェクト構造について

### リポジトリ:

- [Main Repository](https://github.com/hiroi-sora/Umi-OCR) 👈
- [Plugin Repository](https://github.com/hiroi-sora/Umi-OCR_plugins)
- [Windows Runtime Library](https://github.com/hiroi-sora/Umi-OCR_runtime_windows)
- [Linux Runtime Library](https://github.com/hiroi-sora/Umi-OCR_runtime_linux)

## プロジェクトのビルド

- [Windows](https://github.com/hiroi-sora/Umi-OCR_runtime_windows)
- [Linux](https://github.com/hiroi-sora/Umi-OCR_runtime_linux)

---

## ソフトウェアのローカライゼーション:

本プロジェクトはUIのローカライズ作業にWeblateプラットフォームを利用しています。翻訳者による協力を歓迎します。[Weblate: Umi-OCR](https://hosted.weblate.org/engage/umi-ocr/) にアクセスし、既存言語の校正・補完や新規言語の追加が可能です。

以下に、Umi-OCRのローカライゼーションに貢献いただいた翻訳者の皆様を感謝とともに掲載します:

| 翻訳者                                                                               | 対応言語                  |
| ------------------------------------------------------------------------------------ | ------------------------- |
| [bob](https://hosted.weblate.org/user/q021)                                          | English, 繁體中文, 日本語 |
| [Qingzheng Gao](https://github.com/QZGao)                                            | English, 繁體中文         |
| [Weng, Chia-Ling](https://hosted.weblate.org/user/ChiaLingWeng)                      | English, 繁體中文         |
| [linzow](https://hosted.weblate.org/user/linzow)                                     | English, 繁體中文         |
| [Marcos i](https://hosted.weblate.org/user/ultramarkorj9)                            | English, Português        |
| [Eric Guo](https://hosted.weblate.org/user/qwedc001)                                 | English                   |
| [steven0081](https://hosted.weblate.org/user/steven0081)                             | English                   |
| [Brandon Cagle](https://hosted.weblate.org/user/random4t4x14)                        | English                   |
| [plum7x](https://hosted.weblate.org/user/plum7x)                                     | 繁體中文                  |
| [hugoalh](https://hosted.weblate.org/user/hugoalh)                                   | 繁體中文                  |
| [Anarkiisto](https://hosted.weblate.org/user/Anarkiisto)                             | 繁體中文                  |
| [ドコモ光](https://hosted.weblate.org/user/umren190402)                              | 日本語                    |
| [杨鹏](https://hosted.weblate.org/user/ypf)                                          | Português                 |
| [Вячеслав Анатольевич Малышев](https://hosted.weblate.org/user/1969)                 | Русский                   |
| [Muhammadyusuf Kurbonov](https://hosted.weblate.org/user/muhammadyusuf.kurbonov2002) | Русский                   |
| [தமிழ்நேரம்](https://hosted.weblate.org/user/TamilNeram/)                                | தமிழ்                       |

情報の誤りや記載漏れがありましたら、[こちらのディスカッション](https://github.com/hiroi-sora/Umi-OCR/discussions/449) までご連絡ください。

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hiroi-sora/Umi-OCR&type=Date)](https://star-history.com/#hiroi-sora/Umi-OCR&Date)

## [変更ログ](CHANGE_LOG.md)
