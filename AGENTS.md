# marginalgains.github.io 仕様メモ

法務ドキュメント(利用規約・プライバシーポリシー)を GitHub Pages (Jekyll, modernist テーマ) で公開するリポジトリ。

## 構成ルール

- アプリごとの利用規約: `docs/<アプリ名>/term-of-services.md`
- 英語版は `.en.md` サフィックス(例: `term-of-services.en.md`)。日英間は相対リンクで相互参照
- プライバシーポリシーは会社共通: `docs/privacy-policy.md`(日) / `docs/privacy-policy.en.md`(英)
- 規約の正文は日本語。翻訳版は参考扱い(言語条項で明記)

## Wi-Fi Connect (docs/wifi-connector/)

- ソース: `../wifi-connector-android/`(iOS版も同一規約でカバー)
- アプリ名は規約上「Wi-Fi Connect」。ストア表示名はローカライズされる(Wi-Fi接続サポート / Wi-Fi Connection Helper 等)
- 全世界配信(21言語)のため、他アプリの規約に加えて以下を含む:
  - 消費者強行法規カーブアウト(免責・準拠法・管轄)
  - App Store / Google Play 条項(Apple第三受益者、米国禁輸国表明)
  - 言語条項(日本語優先)、分離可能性
- アプリ固有の論点: Wi-Fi自体は提供しない / ポータル入力情報は提供者に直接送信 / HTTP通信を含む / VPN・プライベートDNS無効化の案内は自己責任 / 不正アクセス目的の利用禁止

## 既知の課題

- `docs/privacy-policy.md`(日本語)に広告SDK(AdMob)の外部送信記載がない。英語版には記載済みのため、日本語版の追記が望ましい(外部送信規律・Play Console データセーフティ整合)
