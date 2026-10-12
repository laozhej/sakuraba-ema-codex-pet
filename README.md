# Sakuraba Ema · Codex Pet
Petdex link: https://petdex.dev/pets/sakuraba-ema

[English](#english) · [简体中文](#简体中文) · [日本語](#日本語)

<p align="center">
  <img src="previews/waving.gif" alt="Ema waving" width="192" height="208">
  <img src="previews/running.gif" alt="Ema thinking quietly" width="192" height="208">
  <img src="previews/look-directions.gif" alt="Ema looking around" width="192" height="208">
</p>

## English

A fan-made chibi **Sakuraba Ema (桜羽エマ)** from *Magical Girl Witch Trials*, ready to keep you company in Codex. Her human appearance follows the supplied character illustrations: silver-white hair with pink tips, pink eyes, a sakura-adorned black beret, and a layered black-and-white floral outfit.

### Features

- **9 animations:** idle, moving right, moving left, waving, jumping, disappointment, waiting for input, thinking/working, and review.
- **16 gaze directions** for following your pointer.
- A calm thinking loop with gentle glances, a blink, and a small nod; her hands stay below the collar.
- Transparent **v2 WebP** sprite sheet: **1536 × 2288**, arranged as **8 × 11** cells of **192 × 208**.
- An offline interactive preview and individual animation GIFs.

### Install

1. Download **sakuraba-ema.zip** from the [latest release](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest) and extract it.
2. Copy the extracted **sakuraba-ema** folder into your local pet directory:
   - **Windows:** `%USERPROFILE%\.codex\pets\`
   - **macOS / Linux:** `~/.codex/pets/`
   - If you use a custom `CODEX_HOME`, use `$CODEX_HOME/pets/` instead.
3. Check that `sakuraba-ema/pet.json` and `sakuraba-ema/spritesheet.webp` are directly inside that folder, without an extra nested folder.
4. In a compatible desktop app, open **Settings → Pets**, refresh the list, and select **Sakuraba Ema**. Enter `/pet` to show or hide her. See the [official Pets guide](https://learn.chatgpt.com/docs/pets).

This package requires desktop support for **sprite version 2**. The [installation guide](docs/INSTALL.md) includes copy commands, troubleshooting, updates, and removal.

### Preview

Extract the release or download the repository, then open **[preview.html](preview.html)** in your browser. Select an animation or choose **Look around** and move the pointer around Ema. Keep the HTML file beside `spritesheet.webp`; GitHub displays HTML source, so download it to run the preview.

### Files and contribution

Only **[pet.json](pet.json)** and **[spritesheet.webp](spritesheet.webp)** are needed by the pet loader. **[previews/](previews/)** contains GIFs; **[docs/SPRITE_FORMAT.md](docs/SPRITE_FORMAT.md)** describes the animation layout. If Ema does not appear, check the folder nesting, preserve `spriteVersionNumber: 2`, and refresh or restart the app. To remove her, select another pet and remove only the installed `sakuraba-ema` folder.

Suggestions and fixes are welcome through GitHub issues or pull requests. Include an animation name and a screenshot or short recording when reporting a visual problem. Preserve Ema's character design and the v2 sprite layout.

### Credits

This is an **unofficial fan creation**, not an official game asset or an OpenAI product. The character and original design belong to their respective creators; see the [official game website](https://manosaba.com/). These companion sprites were created with AI assistance from supplied visual references.

---

## 简体中文

### 关于这个宠物

这是以《魔法少女的魔女审判》中的樱羽艾玛（桜羽エマ）为原型制作的同人 Codex 桌面宠物。角色采用人形 Q 版造型，保留银白渐粉的发梢、粉色眼睛、樱花装饰的黑色贝雷帽，以及黑白叠层花饰服装。

- **9 种动画**：待机、向右移动、向左移动、挥手、跳跃、失落、等待、思考／工作和审阅。
- **16 个视线方向**：预览中的 Look around 模式可让角色随鼠标位置转动视线。
- 思考动作以轻微侧瞥、眨眼和点头为主，双手保持在衣领下方。
- **v2 透明 WebP 图集**：1536 × 2288 像素，8 列 × 11 行，每格 192 × 208 像素。

### 快速安装

需要支持 **v2 宠物格式的 Codex 桌面版**。

1. 打开[最新发行版](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest)，下载附件 **`sakuraba-ema.zip`**。
2. 解压后，将整个 `sakuraba-ema` 文件夹放入 `$CODEX_HOME/pets`；未自定义 `CODEX_HOME` 时，默认位置是 `~/.codex/pets`，Windows 为 `%USERPROFILE%\.codex\pets`。
3. 确认目录结构为 `pets/sakuraba-ema/pet.json` 和 `pets/sakuraba-ema/spritesheet.webp`。两个文件必须位于同一层，不要多套一层文件夹。
4. 在应用中打开 **Settings → Pets → Refresh**，选择 **Sakuraba Ema**。使用 `/pet` 显示或隐藏宠物。

完整说明见[完整安装指南](docs/INSTALL.md#简体中文)；应用操作也可参考[官方 Pets 文档](https://learn.chatgpt.com/docs/pets)。

### 预览与排查

如需离线预览，可下载并解压[仓库 ZIP](https://github.com/laozhej/sakuraba-ema-codex-pet/archive/refs/heads/main.zip)，打开 `preview.html`，切换动画或使用 **Look around** 模式。`preview.html` 和 `previews/*.gif` 是可选预览文件，安装只需 `pet.json` 与 `spritesheet.webp`。

宠物未出现时，请重新点击 **Refresh**，检查实际使用的 `CODEX_HOME`、文件夹层级，以及 `pet.json` 的 v2 元数据与应用版本是否兼容。此包面向 Codex 桌面宠物，不是通用网页宠物上传包。卸载时，只删除 `pets/sakuraba-ema` 文件夹。

### 致谢

角色来自[原作《魔法少女的魔女审判》](https://manosaba.com/)。本项目为同人制作，与 OpenAI 及原作创作者无隶属或合作关系。图像基于提供的参考资料，借助 AI 制作，并非官方游戏精灵图。

## 日本語

### このペットについて

『魔法少女ノ魔女裁判』の桜羽エマをモチーフにした、ファン制作の Codex デスクトップペットです。人型のちびキャラクターとして、毛先がピンクの銀白色の髪、ピンクの瞳、桜を飾った黒いベレー帽、花飾りのある黒と白の重ね着衣装を再現しています。

- **9 種類のアニメーション**：待機、右移動、左移動、手振り、ジャンプ、落胆、入力待ち、思考／作業、レビュー。
- **16 方向の視線**：プレビューの Look around モードでは、マウスポインターに合わせて視線が動きます。
- 思考中は、控えめな横目、まばたき、うなずきで表現し、両手は襟より下に保ちます。
- **v2 形式の透過 WebP スプライトシート**：1536 × 2288 ピクセル、8 列 × 11 行、1 コマ 192 × 208 ピクセル。

### インストール

**v2 ペット形式に対応した Codex デスクトップ版**が必要です。

1. [最新リリース](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest)から **`sakuraba-ema.zip`** をダウンロードします。
2. 展開した `sakuraba-ema` フォルダーごと `$CODEX_HOME/pets` にコピーします。`CODEX_HOME` を変更していなければ、既定の場所は `~/.codex/pets`、Windows では `%USERPROFILE%\.codex\pets` です。
3. `pets/sakuraba-ema/pet.json` と `pets/sakuraba-ema/spritesheet.webp` が存在することを確認します。両ファイルは同じ階層に置き、フォルダーを二重にしないでください。
4. アプリで **Settings → Pets → Refresh** を開き、**Sakuraba Ema** を選びます。`/pet` で表示と非表示を切り替えられます。

詳しくは[詳しいインストールガイド](docs/INSTALL.md#日本語)と[公式 Pets ドキュメント](https://learn.chatgpt.com/docs/pets)をご覧ください。

### プレビューとトラブルシューティング

オフラインで確認するには、[リポジトリの ZIP](https://github.com/laozhej/sakuraba-ema-codex-pet/archive/refs/heads/main.zip)をダウンロードして展開し、`preview.html` を開きます。アニメーションの切り替えや **Look around** モードを試せます。`preview.html` と `previews/*.gif` は任意のプレビュー用ファイルです。インストールに必要なのは `pet.json` と `spritesheet.webp` の 2 ファイルです。

一覧に表示されない場合は **Refresh** を押し、使用中の `CODEX_HOME`、フォルダーの階層、`pet.json` の v2 メタデータとアプリの対応状況を確認してください。このパッケージは Codex のデスクトップペット用です。一般的な Web ペットのアップローダー向けではありません。アンインストールする場合は、`pets/sakuraba-ema` フォルダーだけを削除してください。

### クレジット

キャラクターの原作は[『魔法少女ノ魔女裁判』](https://manosaba.com/)です。本プロジェクトはファンによる非公式の制作物で、OpenAI および原作の制作者とは関係ありません。画像は提供された参考資料をもとに AI の支援で制作したもので、公式ゲームのスプライトではありません。
