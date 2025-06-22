# LaTeX Template for Japanese Documents

このリポジトリは日本語文書作成のためのLaTeXテンプレートです。

## 構成

- `main.tex` - メインのLaTeXファイル
- `content/` - 文書の内容を格納するディレクトリ
  - `abstract.tex` - アブストラクト
  - `body.tex` - 本文
  - `appendix.tex` - 付録
- `bib/` - 参考文献ファイル
  - `references.bib` - BibTeXファイル
- `latexmkrc` - latexmkの設定ファイル

## 使用方法

1. 必要なLaTeX環境をインストールしてください
2. `main.tex`を編集して文書を作成
3. 以下のコマンドでPDFを生成：

```bash
latexmk -pdf main.tex
```

## 必要なパッケージ

- latexmk
- 日本語LaTeX環境（pLaTeX等）

## ライセンス

このテンプレートは自由に使用・改変できます。 