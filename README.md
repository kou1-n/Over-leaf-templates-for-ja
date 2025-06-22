# LaTeX Template for Japanese Documents

このリポジトリは日本語文書作成のためのLaTeXテンプレートです。

## 構成

- `main.tex` - メインのLaTeXファイル
- `content/` - 文書の内容を格納するディレクトリ
  - `profile.tex` - **プロフィール情報設定ファイル**（新機能）
  - `abstract.tex` - アブストラクト
  - `body.tex` - 本文
  - `appendix.tex` - 付録
- `bib/` - 参考文献ファイル
  - `references.bib` - BibTeXファイル
- `latexmkrc` - latexmkの設定ファイル

## プロフィール情報の設定

### 1. 基本設定
`content/profile.tex`ファイルを編集して、あなたの情報を設定してください：

```latex
% 基本情報
\newcommand{\profileName}{あなたの名前}
\newcommand{\profileStudentID}{学籍番号}
\newcommand{\profileLaboratory}{研究室名}
\newcommand{\profileProgram}{プログラム名}
\newcommand{\profileSchool}{研究科名}
\newcommand{\profileUniversity}{大学名}

% 報告書タイトル
\newcommand{\reportTitle}{報告書のタイトル}
```

### 2. オプション設定
必要に応じて、以下の情報も設定できます：

```latex
% 連絡先情報
\newcommand{\profileEmail}{your.email@example.com}
\newcommand{\profilePhone}{+81-45-xxx-xxxx}

% 研究分野・専門
\newcommand{\profileResearchArea}{研究分野}
\newcommand{\profileKeywords}{キーワード1, キーワード2, キーワード3}
```

### 3. 詳細プロフィールの表示
本文に詳細なプロフィール情報を表示したい場合は、`content/body.tex`の最初の部分で以下の行のコメントアウトを外してください：

```latex
\showFullProfile
\newpage
```

## 使用方法

1. 必要なLaTeX環境をインストールしてください
2. `content/profile.tex`でプロフィール情報を設定
3. `main.tex`を編集して文書を作成
4. 以下のコマンドでPDFを生成：

```bash
latexmk -pdf main.tex
```

## 必要なパッケージ

- latexmk
- 日本語LaTeX環境（pLaTeX等）

## ライセンス

このテンプレートは自由に使用・改変できます。 