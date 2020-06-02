# FE210-hw2

A Pen created on CodePen.io. Original URL: [https://codepen.io/laiyenju/pen/eYpqbJX](https://codepen.io/laiyenju/pen/eYpqbJX).

## HW2: 如何讓網頁跑起來不卡卡的？

作業 2 的難度不高，甚至能在短時間內完成。主要學習了兩個以前沒使用過的 CSS 方法：`box-shadow` 與 `filter`。

- `box-shadow` 能直接讓物件產生陰影，可調整陰影的 x、y 軸位置外，還能調整陰影的顏色、發散程度。
- `filter` 除了能做出作業要求的物件發亮外，也有各種類似圖片濾鏡的效果可用。

```css
/* offset-x | offset-y | color */
box-shadow: 60px -16px teal;

/* offset-x | offset-y | blur-radius | color */
box-shadow: 10px 5px 5px black;

/* offset-x | offset-y | blur-radius | spread-radius | color */
box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);

/* inset | offset-x | offset-y | color */
box-shadow: inset 5em 1em gold;

/* Any number of shadows, separated by commas */
box-shadow: 3px 3px red, -1em 0 0.4em olive;
```

最後是 transition 效果，能讓動畫轉場變得更滑順。但值得注意的是， `transition: all` 的使用方法無法在每種情況一體適用，因為牽涉「效率」問題。  
最佳的寫法是 `transition: <使用 transition 的效果>`，在 transition 內寫明要使用的效果，可以減輕瀏覽器不停重繪、重排版的工作，降低瀏覽器工作量，
增加效率。

至於瀏覽器的詳細工作階段說明、優化瀏覽器效率的方式，需要看完 [Google 這篇教學](https://developers.google.com/web/fundamentals/performance/rendering/)，以及 Google 在 Udacity 開的[這門免費課程](https://www.udacity.com/course/browser-rendering-optimization--ud860)，應該會有更多收穫。
