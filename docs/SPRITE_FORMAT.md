# Sprite layout / 精灵图布局 / スプライト構成

This repository contains a **v2 desktop pet**. The asset matches the completed local pet; publishing does not alter its pixels.

| Property / 属性 / 項目 | Value / 值 / 値 |
| --- | --- |
| Pet ID | `sakuraba-ema` |
| Display name | `Sakuraba Ema` |
| Sprite version | `2` |
| File | `spritesheet.webp` |
| Pixel format | RGBA, transparent / 透明 / 透過 |
| Sheet size | 1536 × 2288 |
| Grid | 8 columns × 11 rows |
| Cell size | 192 × 208 |
| SHA-256 | `c2426b19726fa6d1e400dab58e3634acee0554e38f0c92ac2090fe4703a56dde` |

Row indices are zero-based. / 行号从 0 开始。 / 行番号は 0 から始まります。

| Row | State | Frames | English / 简体中文 / 日本語 |
| --- | --- | --- | --- |
| 0 | `idle` | 6 | Idle / 待机 / 待機 |
| 1 | `running-right` | 8 | Move right / 向右移动 / 右へ移動 |
| 2 | `running-left` | 8 | Move left / 向左移动 / 左へ移動 |
| 3 | `waving` | 4 | Wave / 挥手 / 手を振る |
| 4 | `jumping` | 5 | Jump / 跳跃 / ジャンプ |
| 5 | `failed` | 8 | Disappointed / 失落 / がっかり |
| 6 | `waiting` | 6 | Waiting for input / 等待输入 / 入力待ち |
| 7 | `running` | 6 | Thinking and working / 思考与工作 / 考え中・作業中 |
| 8 | `review` | 6 | Review / 检查 / 確認 |
| 9 | Gaze / 视线 / 視線 | 8 | 0°, 22.5°, 45°, 67.5°, 90°, 112.5°, 135°, 157.5° |
| 10 | Gaze / 视线 / 視線 | 8 | 180°, 202.5°, 225°, 247.5°, 270°, 292.5°, 315°, 337.5° |

Gaze angles advance clockwise: **0° up, 90° right, 180° down, 270° left**. The neutral gaze frame is at row 0, column 6. The state named `running` means active task work; it is a restrained thinking animation, while the two directional states provide locomotion.

视线角度按顺时针排列：**0° 向上、90° 向右、180° 向下、270° 向左**。中立视线帧位于第 0 行、第 6 列。`running` 表示任务执行状态，对应安静的思考动画；左右移动使用各自的独立动画。

視線の角度は時計回りです：**0° 上、90° 右、180° 下、270° 左**。正面の視線は 0 行目・6 列目にあります。`running` はタスク実行中の状態を表し、控えめな思考アニメーションを使用します。左右への移動には、それぞれ別のアニメーションがあります。
