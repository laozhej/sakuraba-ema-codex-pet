# Installation / 安装说明 / インストール

[English](#english) · [简体中文](#简体中文) · [日本語](#日本語)

## English

Use a desktop app that supports the local Codex **v2 pet format**. This package was validated and installed on Windows. The POSIX copy commands below describe the same file layout; they have not been tested on every desktop platform.

### Download and place the files

1. Open the [latest release](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest), download `sakuraba-ema.zip`, and extract it.
2. Copy its `sakuraba-ema` folder into your pets directory. The default is `%USERPROFILE%\.codex\pets` on Windows or `~/.codex/pets` on macOS/Linux. A custom `CODEX_HOME` uses the `pets` directory inside that location.
3. The resulting layout must be:

```text
<CODEX_HOME or ~/.codex>/
└── pets/
    └── sakuraba-ema/
        ├── pet.json
        └── spritesheet.webp
```

Documentation, previews, and GIFs can stay with these files, but the app only needs those two files. A repository ZIP may extract into `sakuraba-ema-codex-pet-main`; rename that folder to `sakuraba-ema` before copying it, or copy the two files into a new folder with that name.

### Optional copy commands

Open a terminal in the extracted folder containing `pet.json` and `spritesheet.webp`. These commands stop if an installation already exists, so an existing pet is not silently replaced.

**Windows PowerShell**

```powershell
$petHome = if ($env:CODEX_HOME) { $env:CODEX_HOME } else { Join-Path $env:USERPROFILE '.codex' }
$petDestination = Join-Path $petHome 'pets\sakuraba-ema'
if (Test-Path -LiteralPath $petDestination) {
    throw 'Sakuraba Ema is already installed. Back up the existing folder before updating.'
}
New-Item -ItemType Directory -Path $petDestination -Force | Out-Null
Copy-Item -LiteralPath '.\pet.json', '.\spritesheet.webp' -Destination $petDestination
```

**macOS / Linux shell**

```sh
pet_destination="${CODEX_HOME:-$HOME/.codex}/pets/sakuraba-ema"
if [ -e "$pet_destination" ]; then
  printf '%s\n' 'Sakuraba Ema is already installed. Back up the existing folder before updating.' >&2
else
  mkdir -p "$pet_destination" && cp pet.json spritesheet.webp "$pet_destination/"
fi
```

### Select and preview

Refresh **Settings → Pets**, select **Sakuraba Ema**, and use `/pet` to show or hide the desktop companion. Menu names can vary with app versions; see the [official Pets documentation](https://learn.chatgpt.com/docs/pets).

To preview without installing, open the extracted `preview.html` in a browser. Its buttons play the animations; **Look around** follows the pointer. The `previews` folder also contains standalone GIFs.

### Troubleshooting and updates

- **Not listed:** check the exact folder layout above, then refresh the pet list or restart the app. If `CODEX_HOME` is set, use that location.
- **Rejected or scrambled sprite:** keep `spriteVersionNumber` set to `2` in `pet.json`. Keep the sprite sheet at **1536 × 2288**; do not resize it or convert it to JPEG.
- **Preview is blank:** extract the ZIP first and keep `preview.html` beside `spritesheet.webp`.
- **No animation:** check the operating system's reduced-motion setting. Apps may intentionally show a still frame when reduced motion is enabled.
- **Updating:** select another pet, back up the existing `sakuraba-ema` folder outside the pets directory, and replace the two required files with the new release. Refresh the app afterward.
- **Removing:** select another pet, remove only the installed `sakuraba-ema` folder, and refresh the list.

## 简体中文

需要支持 Codex 本地 **v2 桌面宠物格式**的应用。本安装包已在 Windows 上完成验证和安装；其他桌面平台的具体支持情况取决于应用版本。

1. 从[最新发布版本](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest)下载 `sakuraba-ema.zip` 并解压。
2. 将 `sakuraba-ema` 文件夹复制到 Windows 的 `%USERPROFILE%\.codex\pets\`，或 macOS/Linux 的 `~/.codex/pets/`。如果设置了 `CODEX_HOME`，请使用该目录下的 `pets` 文件夹。
3. 确认 `pet.json` 和 `spritesheet.webp` 直接位于 `pets/sakuraba-ema/` 中，没有多套一层文件夹。
4. 在应用的 **Settings → Pets（设置 → 宠物）**中刷新列表，选择 **Sakuraba Ema**。输入 `/pet` 可显示或隐藏桌面宠物。相关界面说明见[官方文档](https://learn.chatgpt.com/docs/pets)。

也可以在包含两个必需文件的目录中运行上方对应系统的复制命令。命令检测到已有安装时会停止；更新前请先备份旧文件夹。

无需安装即可预览：用浏览器打开解压后的 `preview.html`，选择动画；**Look around** 模式会跟随鼠标。不要移动或删除旁边的 `spritesheet.webp`。

**排查与维护：**无法显示时检查目录层级和 `CODEX_HOME`，然后刷新或重启应用；保留 `spriteVersionNumber: 2` 和 **1536 × 2288** 的原始尺寸，不要转换成 JPEG。若只有静态画面，请检查系统的“减少动态效果”设置。更新时先选择其他宠物，将旧文件夹备份到宠物目录之外，再替换两个必需文件，并刷新列表。卸载时只删除已安装的 `sakuraba-ema` 文件夹并刷新列表。

## 日本語

Codex のローカル **v2 デスクトップペット形式**に対応したアプリが必要です。このパッケージは Windows で検証・インストール済みです。他のデスクトップ環境での対応状況は、アプリのバージョンによって異なります。

1. [最新リリース](https://github.com/laozhej/sakuraba-ema-codex-pet/releases/latest)から `sakuraba-ema.zip` をダウンロードして展開します。
2. `sakuraba-ema` フォルダーを、Windows では `%USERPROFILE%\.codex\pets\`、macOS/Linux では `~/.codex/pets/` にコピーします。`CODEX_HOME` を設定している場合は、その中の `pets` フォルダーを使います。
3. `pet.json` と `spritesheet.webp` が `pets/sakuraba-ema/` の直下にあることを確認します。余分なフォルダー階層を作らないでください。
4. アプリの **Settings → Pets（設定 → ペット）**で一覧を更新し、**Sakuraba Ema** を選びます。`/pet` でデスクトップペットの表示を切り替えられます。画面の操作は[公式ドキュメント](https://learn.chatgpt.com/docs/pets)も参照してください。

コマンドでコピーする場合は、上記の必須ファイルがあるフォルダーで、該当する OS のコマンドを実行してください。すでにインストールされている場合は処理が止まるので、更新前に既存のフォルダーをバックアップしてください。

インストールせずに確認するには、展開した `preview.html` をブラウザーで開きます。アニメーションを選ぶか、**Look around** を選んでポインターを動かしてください。隣の `spritesheet.webp` も必要です。

**問題が起きた場合：**フォルダー構成と `CODEX_HOME` を確認し、一覧の更新またはアプリの再起動を試してください。`spriteVersionNumber: 2` と **1536 × 2288** の画像サイズを維持し、JPEG に変換しないでください。静止画になる場合は OS のアニメーションを減らす設定を確認してください。更新時は別のペットを選び、古いフォルダーをペットの保存先以外にバックアップしてから、必須ファイルを置き換え、一覧を更新します。削除する場合は、インストール先の `sakuraba-ema` フォルダーだけを削除し、一覧を更新してください。
