# コーディングガイドライン

## 全般
### 対応ブラウザ !要確認
  - iOS safari
  - Android
  - Edge (windows10)
  - IE11
  - chrome
  - Firefox
  - safari

### インデント

スペース2個

### 文字コード 
 UTF-8

<br>

## 命名規則

### 画像名

[種別]-[名前]\_[連番].[拡張子]

例 : `btn-submit_01.svg`

### CSS class名

BEM(MindBEMding)をベースに、以下のように記述

[Block]__[Element][連番]--[Modifier]

例 : `header` <br>
例 : `header__gnav01` <br>
例 : `button--email` <br>
例 : `footer__sns--twitter` <br>

<br>

## ディレクトリ名

画像ディレクトリ : `img`<br>
CSSディレクトリ : `css`<br>
JSディレクトリ : `js`<br>

<br>

## CSS

PCファーストとして記述する。<br>
PC表示のスタイルをまず記述し、SP表示をメディアクエリで記述する

CSSのセレクタ名はclassのみ使用<br>
※idセレクタを使う場合はJS用、ページ内リンク用のみ許可

子孫セレクタ：可能

例 ： `header .header-gnav a`

### CSSプロパティ、セレクタの書き方

```
img {
  max-width: 100%;
}
```
「セレクタ名」「半角スペース」「ブレース」<br>
「インデント」「プロパティ」「コロン」「半角スペース」「値」「セミコロン」<br>
「ブレース」<br>
とする<br>
最終行のプロパティの値のうしろにもセミコロンを付与する<br>
SCSSで圧縮する場合はこの限りではない

### リセットCSS

[HTML5 Doctor Reset CSS](http://html5doctor.com/html-5-reset-stylesheet/)

<br>

## media queries !要確認

以下のブレークポイントから利用する

 - 'sm-min': 'screen and (min-width: 576px)',
 - 'sm-max': 'screen and (max-width: 575px)',
 - 'md-min': 'screen and (min-width: 768px)',
 - 'md-max': 'screen and (max-width: 767px)',
 - 'lg-min': 'screen and (min-width: 992px)',
 - 'lg-max': 'screen and (max-width: 991px)',
 - 'xl-min': 'screen and (min-width: 1131px)',
 - 'xl-max': 'screen and (max-width: 1130px)',

<br>

## SCSS

SASS構文ではなくSCSSで記述する

<br>

## JS
jQueryを利用可能
