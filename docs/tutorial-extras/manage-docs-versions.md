---
sidebar_position: 1
---

# ドキュメントのバージョンを管理する

Docusaurusはキュメントの複数のバージョンを管理できます。

## ドキュメントバージョンを作成する

プロジェクトのバージョン1.0をリリースします。

```bash
npm run docusaurus docs:version 1.0
```

「docs」フォルダーが「versioned_docs/version-1.0」にコピーされ、「versions.json」が作成されます。

ドキュメントには2つのバージョンがあります。

- `1.0` at  `http://localhost:3000/docs/` for the version 1.0 docs
- `current` at `http://localhost:3000/docs/next/` for the **upcoming, unreleased docs**

## バージョンドロップダウンを追加

バージョン間をシームレスに移動するには、バージョンのドロップダウンを追加します。

`docusaurus.config.js` ファイルを修正する。

```js title="docusaurus.config.js"
export default {
  themeConfig: {
    navbar: {
      items: [
        // highlight-start
        {
          type: 'docsVersionDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

ドキュメント バージョンのドロップダウンがナビゲーションバーに表示されます。

![Docs Version Dropdown](./img/docsVersionDropdown.png)

## 既存のバージョンを更新する

バージョン管理されたドキュメントは、それぞれのフォルダーで編集できます。

- `versioned_docs/version-1.0/hello.md` updates `http://localhost:3000/docs/hello`
- `docs/hello.md` updates `http://localhost:3000/docs/next/hello`
