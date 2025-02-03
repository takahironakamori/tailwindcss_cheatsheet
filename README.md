# Tailwind CSS チートシート

※未検証

## Layout

### Container

| クラス | 説明 |
|--------|------|
| `container` | レスポンシブコンテナ |

```html
<div class="container mx-auto bg-gray-100 p-4">コンテナのプレビュー</div>
```

### Display

| クラス | 説明 |
|--------|------|
| `block` `inline` `inline-block` `flex` `inline-flex` `grid` `table` `hidden` | 表示設定 |

```html
<div class="flex space-x-2">
  <div class="block bg-blue-500 text-white p-2">Block</div>
  <div class="inline-block bg-green-500 text-white p-2">Inline-block</div>
</div>
```

### Flexbox

| クラス | 説明 | `n` の値 |
|--------|------|----------|
| `flex` `inline-flex` | フレックスボックスの設定 | - |
| `flex-row` `flex-col` | フレックス方向 | - |
| `flex-wrap` `flex-nowrap` `flex-wrap-reverse` | フレックスラップ設定 | - |
| `justify-{start\|center\|end\|between\|around\|evenly}` | 横方向の配置 | - |
| `items-{start\|center\|end\|baseline\|stretch}` | 縦方向の配置 | - |
| `self-{auto\|start\|center\|end\|stretch}` | セルフアライン | - |
| `gap-{n}` | グリッド・フレックス間の間隔 | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `px` |

```html
<div class="flex justify-between bg-gray-200 p-2">
  <div class="bg-red-500 text-white p-2">Start</div>
  <div class="bg-yellow-500 text-white p-2">Center</div>
  <div class="bg-blue-500 text-white p-2">End</div>
</div>
```

---

## Spacing

| クラス | 説明 | `n` の値 |
|--------|------|----------|
| `m-{n}` | 外側の余白 (margin) | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `px`, `auto` |
| `mx-{n}` `my-{n}` | 水平方向・垂直方向の余白 | 同上 |
| `mt-{n}` `mr-{n}` `mb-{n}` `ml-{n}` | 上・右・下・左の余白 | 同上 |
| `p-{n}` | 内側の余白 (padding) | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `px` |
| `px-{n}` `py-{n}` | 水平方向・垂直方向の内側余白 | 同上 |
| `pt-{n}` `pr-{n}` `pb-{n}` `pl-{n}` | 上・右・下・左の内側余白 | 同上 |
| `gap-{n}` | グリッド・フレックス間の間隔 | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `px` |
| `space-x-{n}` `space-y-{n}` | 要素間の間隔 | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `px` |

```html
<div class="p-4 m-2 bg-gray-200">スペーシングのプレビュー</div>
```

---

## Sizing

| クラス | 説明 | `n` の値 |
|--------|------|----------|
| `w-{n}` | 幅の指定 | `0`, `1`, `2`, `4`, `8`, `16`, `32`, `64`, `1/2`, `1/3`, `1/4`, `full`, `screen`, `auto` |
| `h-{n}` | 高さの指定 | 同上 |
| `min-w-{n}` `min-h-{n}` | 最小幅・最小高さ | `0`, `full`, `screen` |
| `max-w-{n}` `max-h-{n}` | 最大幅・最大高さ | `0`, `full`, `screen` |
| `w-full` `h-full` | 親要素いっぱいの幅・高さ | - |
| `w-screen` `h-screen` | 画面いっぱいの幅・高さ | - |

```html
<div class="w-1/2 h-20 bg-blue-500">サイズのプレビュー</div>
```

## Filters

| クラス | 説明 | `n` の値 |
|--------|------|----------|
| `blur-{n}` | ぼかし | `none`, `sm`, `md`, `lg`, `xl`, `2xl`, `3xl` |
| `brightness-{n}` | 明るさ調整 | `0`, `50`, `75`, `90`, `95`, `100`, `105`, `110`, `125`, `150`, `200` |
| `contrast-{n}` | コントラスト調整 | `0`, `50`, `75`, `100`, `125`, `150`, `200` |
| `grayscale-{n}` | グレースケール | `0`, `100` |
| `hue-rotate-{n}` | 色相回転 | `0`, `15`, `30`, `60`, `90`, `180` |
| `invert-{n}` | 反転 | `0`, `100` |
| `sepia-{n}` | セピア調 | `0`, `100` |
| `saturate-{n}` | 彩度調整 | `0`, `50`, `100`, `150`, `200` |

```html
<img class="blur-md brightness-150 contrast-125" src="example.jpg" alt="フィルターのプレビュー">
```

## Typography

| クラス | 説明 |
|--------|------|
| `text-{xs\|sm\|base\|lg\|xl\|2xl\|3xl\|4xl\|5xl\|6xl\|7xl\|8xl\|9xl}` | フォントサイズ |
| `font-{sans\|serif\|mono}` | フォントファミリー |
| `font-{thin\|extralight\|light\|normal\|medium\|semibold\|bold\|extrabold\|black}` | フォントの太さ |
| `tracking-{tighter\|tight\|normal\|wide\|wider\|widest}` | 文字間隔 |
| `leading-{none\|tight\|snug\|normal\|relaxed\|loose}` | 行間設定 |
| `text-{left\|center\|right\|justify}` | テキスト配置 |
| `underline` `line-through` `no-underline` | テキストの装飾 |
| `uppercase` `lowercase` `capitalize` | 文字の変換 |
| `truncate` `overflow-ellipsis` `overflow-clip` | 文字の切り詰め |
| `whitespace-{normal\|nowrap\|pre\|pre-line\|pre-wrap}` | 空白の処理方法 |
| `break-{normal\|words\|all}` | 改行設定 |

```html
<p class="text-lg text-red-500 underline">テキストのプレビュー</p>
```

## Colors

| クラス | 説明 | 使用可能な色 |
|--------|------|--------------|
| `text-{color}` | テキストの色 | `red`, `blue`, `green`, `yellow`, `purple`, `pink`, `gray`, `black`, `white` など |
| `bg-{color}` | 背景色 | 同上 |
| `border-{color}` | ボーダーの色 | 同上 |
| `ring-{color}` | リングの色 (フォーカス時の枠線) | 同上 |
| `divide-{color}` | Flex/Grid の区切り線の色 | 同上 |
| `placeholder-{color}` | プレースホルダーの色 | 同上 |
| `shadow-{color}` | ボックスシャドウの色 | `red`, `blue`, `green` など |

### 色のバリエーション

- `{color}-{50|100|200|300|400|500|600|700|800|900}` の形式で指定可能
- 例: `bg-red-500` (中程度の赤), `text-blue-700` (濃い青)

```html
<div class="bg-blue-500 text-white p-4">色のプレビュー</div>
```

## Links

| クラス | 説明 |
|--------|------|
| `text-{color}` | リンクのテキスト色を指定 |
| `hover:text-{color}` | ホバー時のテキスト色を指定 |
| `focus:text-{color}` | フォーカス時のテキスト色を指定 |
| `underline` `no-underline` | リンクの下線を表示・非表示 |
| `hover:underline` | ホバー時に下線を表示 |
| `focus:underline` | フォーカス時に下線を表示 |
| `active:text-{color}` | アクティブ状態のテキスト色を指定 |
| `visited:text-{color}` | 訪問済みリンクの色を指定 |
| `cursor-pointer` | リンクにポインターカーソルを適用 |

- color は Colors の項目と同じ。

```html
<a href="#" class="text-blue-500 hover:text-blue-700 underline">リンクのプレビュー</a>
```

## Images

| クラス | 説明 | `n` の値 |
|--------|------|----------|
| `w-{n}` | 画像の幅を指定 | `1`, `2`, `4`, `8`, `16`, `32`, `64`, `1/2`, `1/3`, `1/4`, `full`, `screen`, `auto` |
| `h-{n}` | 画像の高さを指定 | 同上 |
| `max-w-{n}` | 最大幅を指定 | `none`, `xs`, `sm`, `md`, `lg`, `xl`, `2xl`, `3xl`, `4xl`, `5xl`, `full`, `screen` |
| `max-h-{n}` | 最大高さを指定 | `none`, `full`, `screen` |
| `rounded-{n}` | 画像の角丸の指定 | `none`, `sm`, `md`, `lg`, `xl`, `2xl`, `full` |
| `border-{n}` | 画像にボーダーを適用 | `0`, `2`, `4`, `8` |
| `border-{color}` | 画像のボーダー色を指定 | `red`, `blue`, `green`, `yellow`, `purple`, `pink`, `gray`, `black`, `white` など |
| `shadow-{n}` | 画像にシャドウを適用 | `sm`, `md`, `lg`, `xl`, `2xl` |
| `object-{n}` | 画像のオブジェクトフィットを設定 | `contain`, `cover`, `fill`, `none`, `scale-down` |
| `object-{n}` | 画像の配置を指定 | `top`, `center`, `bottom`, `left`, `right` |
| `opacity-{n}` | 画像の透明度を指定 | `0`, `25`, `50`, `75`, `100` |
| `grayscale-{n}` | グレースケール効果を適用 | `0`, `100` |
| `blur-{n}` | 画像のぼかし効果 | `none`, `sm`, `md`, `lg`, `xl`, `2xl` |

```html
<img src="example.jpg" class="w-64 h-64 rounded-lg shadow-md object-cover" alt="画像のプレビュー">
```

## Table

| クラス | 説明 |
|--------|------|
| `table` | 標準のテーブル表示 |
| `table-auto` `table-fixed` | 列幅の制御 |
| `border` `border-collapse` `border-separate` | ボーダースタイル |
| `border-{color}` | ボーダーの色 |
| `bg-{color}` | 背景色 |
| `text-{color}` | テキストの色 |

- color は Colors の項目と同じ。

```html
<table class="table-auto border-collapse border border-gray-300 w-full">
  <thead>
    <tr>
      <th class="border border-gray-300 p-2">Header 1</th>
      <th class="border border-gray-300 p-2">Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="border border-gray-300 p-2">Cell 1</td>
      <td class="border border-gray-300 p-2">Cell 2</td>
    </tr>
  </tbody>
</table>
```

## List

| クラス | 説明 |
|--------|------|
| `list-disc` `list-decimal` | 箇条書きのスタイル |
| `list-none` | 箇条書きを非表示 |
| `list-inside` `list-outside` | 箇条書きの配置 |

```html
<ul class="list-disc pl-5">
  <li>項目 1</li>
  <li>項目 2</li>
</ul>
```

## Others

### Responsive Design

| クラス | 説明 |
|--------|------|
| `sm:` `md:` `lg:` `xl:` `2xl:` | 各ブレークポイント |

```html
<div class="bg-gray-200 p-2 sm:bg-blue-500 md:bg-green-500 lg:bg-red-500 xl:bg-yellow-500">
  画面サイズによる色変化
</div>
```

### Z-Index

| クラス | 説明 |
|--------|------|
| `z-{0\|10\|20\|30\|40\|50\|auto}` | 要素の重なり順 |

### Visibility

| クラス | 説明 |
|--------|------|
| `visible` `invisible` `hidden` | 要素の表示制御 |

### Overflow

| クラス | 説明 |
|--------|------|
| `overflow-{auto\|hidden\|visible\|scroll}` | オーバーフローの制御 |

### Pointer Events

| クラス | 説明 |
|--------|------|
| `pointer-events-{none\|auto}` | ポインターイベントの制御 |

### Cursor

| クラス | 説明 |
|--------|------|
| `cursor-{pointer\|not-allowed\|wait\|default\|text}` | カーソルスタイルの変更 |

### User Select

| クラス | 説明 |
|--------|------|
| `select-{none\|text\|all\|auto}` | テキスト選択の可否 |

### Scroll Behavior

| クラス | 説明 |
|--------|------|
| `scroll-auto` `scroll-smooth` | スクロールの挙動 |

### Animation

| クラス | 説明 |
|--------|------|
| `animate-{none\|spin\|ping\|pulse\|bounce\|wiggle\|fade\|flash\|rubber-band\|shake\|swing\|tada\|wobble\|jello}` | アニメーションの適用 |
| `motion-reduce:{class}` | モーション削減設定 |
| `animate-duration-{75\|100\|150\|200\|300\|500\|700\|1000}` | アニメーションの長さ |
| `animate-delay-{75\|100\|150\|200\|300\|500\|700\|1000}` | アニメーションの遅延 |
| `animate-ease-{linear\|in\|out\|in-out}` | アニメーションのイージング |
| `animate-fill-{none\|forwards\|backwards\|both}` | フィルモード設定 |

```html
<div class="animate-bounce bg-blue-500 p-4 text-white">アニメーションのプレビュー</div>
```

## Transitions

| クラス | 説明 |
|--------|------|
| `transition` | すべてのプロパティを遷移させる |
| `transition-none` | トランジションを無効化 |
| `transition-all` | すべてのプロパティを遷移させる |
| `transition-colors` | 色の変化のみ遷移させる |
| `transition-opacity` | 透明度の変化のみ遷移させる |
| `transition-shadow` | シャドウの変化のみ遷移させる |
| `transition-transform` | 変形の変化のみ遷移させる |
| `duration-{75\|100\|150\|200\|300\|500\|700\|1000}` | 遷移時間を指定 |
| `ease-{linear\|in\|out\|in-out}` | イージング関数を適用 |
| `delay-{75\|100\|150\|200\|300\|500\|700\|1000}` | 遅延時間を指定 |

```html
<button class="transition duration-300 ease-in-out bg-blue-500 hover:bg-red-500 p-4 text-white">
  ホバーで色変化
</button>
```
