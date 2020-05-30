# 2020-05-23 人員介紹卡片

![成品](./completed.jpg)

## 重點整理

- img 會因為 baseline 的問題導致圖片下方會有點空格，使用(vertical-align)去除。

```css
img {
  vertical-align: middle;
}
```

- 想要用border去當作長寬的話，需要先把原先的width、height設定為0
