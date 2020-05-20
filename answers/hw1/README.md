# FE210-hw1

A Pen created on CodePen.io. Original URL: [https://codepen.io/laiyenju/pen/dyYQLjY](https://codepen.io/laiyenju/pen/dyYQLjY).

## HW1: 終於了解 css position 在幹嘛，以及讓人愛不釋手的 css flexbox

從 codeing 火球術之後換購了這門課程，帶著成為前端工程師的決心，直到昨天才開始看，完成第一份作業。
雖然我對 HTML、CSS 有基本概念，也有架設個人部落格網站的經驗，但總是改用其他人開源的模板，或者偷懶套用 Bootstrap，對只用 CSS 設置 layout 完全沒信心，因為根本不了解 CSS position 的原理。

第一次作業收穫最大就是 CSS 的 position 與 flexbox，在前者釐清 `position: relative` 與 `position: absolute` 的差別，後者則是新學到的技巧。

- `position: relative` 能讓被設定的物件，將父層物件作為定位基準點，也可以指定 z-index。
- `position: absolute` 則會讓被設定的物件，去尋找最接近的、position 設定為 relative 或 absolute 的物件作為定為基準點。
- CSS flexbox 比 `display: inline-block` 有更多設定空間，用來水平對齊、按順序排列物件、平均分佈物件，使用方式是 `display: flex` 搭配 
  - justify-cnotent: `[flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe]`
  - flex-direction: `[row | row-reverse | column | column-reverse]`
  - align-items: `[stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe]`
  - align-content: `[flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe]`
  - flex-wrap: `[nowrap | wrap | wrap-reverse]` 選擇換行方式
  - flex-flow: `column wrap`

以前看到有人在推特分享 flexbox 好用的心得，都無法理解好用的點在哪，但這次入坑後，真的就如 Huli 所說的回不去了。
未來遇到會不斷增生的物件，可以使用 flexbox 模式安排，創造類似 RWD 的樣式。
