---
marp: true
theme: default
paginate: true
backgroundImage: #FFCE00
header: " "
footer: ©2023 株式会社Utill 髙橋俊介
style: |
    header {
        background-image: url("images/logo.svg");
        background-size: contain;
        background-repeat: no-repeat;
        padding: 1rem 2rem;
    }
    footer {
        text-align:right;
        right:2rem
    }
    .mermaid{
        width:100%;
    }
---
# Marpで資料を作ってLTへの参加ハードルを下げる
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# 自己紹介
## 髙橋俊介
- 新卒で小売業界でSV(スーパーバイザー)として働く
- 2019年よりWebエンジニアとして働き始める
- 今年の2月から株式会社UtillでWebエンジニアとして働いている

![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# 本日のお題
- そもそもLTについてどういう認識？
- MarpでLT資料を作ろう
- まとめ
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# そもそもLTについてどういう認識？
![opacity:0.03 bg 70%  grayscale](images/logo.svg)


---
<style scoped>
    footer {
        display:none;
    }

</style>


### 題材と資料に関して<br>調べる人が多い
### LTを始めてやる人が<br>調べていそうな<br>ワードたち
![bg 90% right:65%](images/image1.png)

---
# そもそもLTについてどういう認識？
## 題材系
### →人によるので一律に解決策が出しづらいこと

## 資料系
### →ある程度、技術的に解決出来ること
![opacity:0.03 bg 70%  grayscale](images/logo.svg)


---
# そもそもLTについてどういう認識？
## 参加へのハードルを下げれそうな点
## →LT資料を作ることが楽になればいい
![opacity:0.03 bg 70%  grayscale](images/logo.svg)


---
# そもそもLTについてどういう認識？

## 何を使ってLT資料を作る？
### ツール
- PPT、Google スライド
- Keynote
- Canva 
- etc...
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# そもそもLTについてどういう認識？
## もっと楽に資料作りたい
- 資料作成に時間かけたくない
- 書き慣れてるMarkDownで書きたい
- 履歴管理したい
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# MarpでLT資料を作ろう
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

---
# MarpでLT資料を作ろう
![opacity:0.03 bg 70%  grayscale](images/logo.svg)
## 用意するもの
- Visual Studio Code (必須)
- Marp for VS Code (必須)
- Markdown Preview Mermaid（任意）

---
# MarpでLT資料を作ろう
![opacity:0.03 bg 70%  grayscale](images/logo.svg)
## 基本的にMD記法なら何でも書ける
<style scoped>
  table { table-layout: fixed; width: 100%; display:table; font-size: 24px; }
</style>
【表サンプル】
| 額(円) | 平均(個)| 最大値(個) | 最小値(個) |
| --- | --- | --- | --- |
| 10,000 | 12.949 | 179 | 5 | 
| 5,000  | 6.814 | 180 | 5 |
| 1,000  | 8.589 | 181 | 5 |

---

<style scoped>
    .mermaid{
        padding-left:2rem;
    }
    footer{display:none}
</style>

# MarpでLT資料を作ろう
## Mermaidも使える
![bg 90% right:50%](images/image4.png)
※事前にVSCodeの設定で`markdown.marp.enableHtml`で検索して、checkを入れておきましょう。

---

<style scoped>
    .mermaid{
        padding-left:2rem;
    }
    footer{display:none}
</style>

# MarpでLT資料を作ろう
## Mermaidも使える
![bg 90% right:50%](images/image3.png)

<div class="mermaid">
sequenceDiagram
    participant cook as 料理人
    participant tool as フライパン
    cook ->>+ tool: お肉を焼く
    Note over tool: 火が通るまで待つ
    tool -->>- cook: 焼き上がり
</div>

---

# MarpでLT資料を作ろう
## 特定のページだけスタイル変更したい
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

```
<style scoped>
    要素{
        セレクタ:プロパティ;
    }
</style>
```
でscopedでCSSも割り当てられる。


---
<style scoped>
    footer{
        display:none
    }
</style>

# MarpでLT資料を作ろう
## Marpを出力①
単純にPDFとして出力するだけであればVSCode上で出力可能
![bg 95% right:50%](images/image2.png)

---
<style scoped>
    footer{
        display:none
    }
</style>

# MarpでLT資料を作ろう
## Marpを出力②
GitHub Actionで[@marp-team/marp-cli](https://github.com/marp-team/marp-cli) を使ってHTML/CSSやPDF、PowerPoint ドキュメントとして出力

---

# MarpでLT資料を作ろう
## 公開まで自動化したい


---
![opacity:0.03 bg 70%  grayscale](images/logo.svg)
# まとめ
- LTはMarpを使って資料作成に時間を掛け過ぎない
    - 使うことで1ページのボリュームを盛り過ぎずに済む
- 社内でLT会をやる時などMarpで
    - GitHubなどで管理しておくと楽
    - テーマ用CSSを作って使いまわせるようにしておくことで更に効率化

---
![opacity:0.03 bg 70%  grayscale](images/logo.svg)

<style scoped>
    h1{
        text-align:center
    }
</style>

# ご清聴ありがとうございました。
