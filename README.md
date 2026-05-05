# kokusen-legal

[白線 -HAKUSEN-](https://apps.apple.com/) iOS アプリの利用規約・プライバシーポリシーを公開するためのリポジトリ。

GitHub Pages 経由で配信され、アプリ内 (`Sources/Util/LegalText.swift`) からリンクされます。

## 配信 URL

- 利用規約: <https://onigiri5373.github.io/kokusen-legal/terms/>
- プライバシーポリシー: <https://onigiri5373.github.io/kokusen-legal/privacy/>

## 構成

```
.
├── index.html         ランディング
├── terms/index.html   利用規約
├── privacy/index.html プライバシーポリシー
└── .nojekyll          Jekyll 処理を無効化(高速化 + 正確性)
```

## 編集の注意

- ToS / Privacy Policy の文言を変える場合、アプリ側の `Resources/PrivacyInfo.xcprivacy`、`Sources/Util/LegalText.swift` の `summary` と整合を保つこと。
- 重大な変更時はアプリ側の `LegalAcceptance` のキー suffix を `_v2 → _v3` のようにバンプし、既存ユーザーに再同意を促すこと。

## ライセンス

本リポジトリの内容は ONIGIRIBOYS に帰属する法的文書です。利用規約・プライバシーポリシーの転載・再利用は許可しません。
