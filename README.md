# sns-media-live

Meta APIが取得するSNS mediaの公開専用repositoryです。

- mediaの長期保存正本はDellです。
- 投稿コード、Access Token、Secret、package、runtime DBは置きません。
- 公開mediaは`media-live` orphan branchで管理します。
- 既存予約の旧Raw URLは変更しません。
- snapshot更新時は全accountの保持対象を含め、SHA-256検証後に`media-live`だけを`--force-with-lease`で更新します。

`media-live`の配置規則:

```text
<account_id>/<platform>/<package_id>/<filename>
```

