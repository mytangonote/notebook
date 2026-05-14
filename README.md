# My Tango Note

> *A quiet corner for words worth keeping.*
> *英語の輪郭が、1単語ずつ見えてくるノート。*

AIで何でも翻訳できる時代に、能動的に英語と向き合う習慣を取り戻すための個人ノート。

A personal English vocabulary notebook for the AI era — a tool to keep your relationship with English alive, one word at a time.

---

## なぜ作ったか — Why this exists

AI翻訳が便利になりすぎて、英語を「読む」体験が静かに消えていく。仕事は回るけれど、自分が何を知っていて何を知らないかが分からなくなる。

**My Tango Note** は、気になった単語やフレーズを Claude と一緒に深く調べ、自分だけの単語帳として蓄積するための小さな道具です。

- 「単語帳」というより、**英語の私的なノート**
- 「暗記」じゃなく、**気になった言葉を腹落ちさせる**
- 「100単語覚える」じゃなく、**今週の3単語を自分のものにする**

---

## 何ができるか — What it does

英語の単語・フレーズ・熟語を入力すると、以下が **英語と日本語の両方で** 並んだリッチなエントリーが生成されます:

- **意味**（多義的なニュアンス含めて）
- **例文**（あなたが選ぶモードに合わせた文脈で）
- **Notes**（コロケーション、類義語、語源、使い分け、発音）

そして、エントリーはノート形式で蓄積され、検索・フィルタ・エクスポートできます。

### モード切替

同じ単語でも、文脈が違えば例文も変わるべき。My Tango Note は4つのモードを切り替えられます:

- 💼 **Business** — ミーティング、メール、プレゼン
- 📚 **Literature / Academic** — 本、論文、エッセイ
- ☕ **Casual** — 日常会話、友人との会話
- 📰 **News / Current Affairs** — ジャーナリズム、時事

### その他の機能

- 🔊 **音声読み上げ** — 単語と例文を発音してくれる（Web Speech API、無料）
- 🔍 **全文検索** — 意味・例文・Notes すべて横断
- 🏷️ **タイプ別フィルタ** — 名詞 / 動詞 / イディオム etc.
- 📤 **エクスポート** — CSV / JSON（Google Sheets にも取り込める）
- 🔒 **完全プライベート** — データは自分のブラウザ内のみ（サーバー送信なし）

---

## 始め方 — Getting started

### 1. このリポジトリから `index.html` をダウンロード

[Code → Download ZIP](https://github.com/mytangonote/notebook/archive/refs/heads/main.zip) でも、個別ファイル `index.html` を右クリック → 名前を付けて保存、でもOK。

### 2. Claude（Claude.ai または Claude API 経由のアプリ）に以下を投げる

```
これから私の英語の単語帳を作ります。

以降、私が英語の単語・フレーズ・熟語を投げますので、毎回以下の構造で返してください:

📘 [単語/フレーズ] /発音/ (品詞)

Meaning (EN): 英語での意味
意味 (JP): 日本語での意味とニュアンス

Example (EN): 英語例文
例文 (JP): 日本語訳

Notes: 使い分け、コロケーション、類義語、語源、発音の注意点など

モード指定がない場合はニュートラルで生成してください。
モード指定がある場合は例文と Notes をそのモードに寄せてください:
- Business モード: 仕事の文脈
- Literature / Academic モード: 文学・学術の文脈
- Casual モード: 日常会話
- News / Current Affairs モード: ジャーナリズム文脈

返ってきたエントリーは、私が手元のノート（HTMLファイル）に追記します。
```

### 3. 単語を投げて、エントリーをノートに追加

返ってきたエントリーを、ダウンロードした `index.html` の `entries` 配列に追加します。手動でコピペ、または Claude にお願いして HTML を更新してもらう、どちらでも。

### 4. ブラウザで `index.html` を開く

ローカルファイルとして、好きな場所に保存して開くだけ。サーバーは不要。

---

## ライセンス — License

[MIT License](LICENSE) — 自由に使って、改造して、共有してください。

---

## 作者 — Author

[My Tango Note](https://mytangonote.com) by [@mytangonote](https://x.com/mytangonote)
note: [note.com/mytangonote](https://note.com/mytangonote)

---

*Made with Claude. 2026.*
