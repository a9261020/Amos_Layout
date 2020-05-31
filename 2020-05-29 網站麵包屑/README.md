# 2020-05-29 網站麵包屑

![成品](./completed.jpg)

## 重點整理

- 加號符號(+)是會影響到後方同層級的第一個元素，第一個 li::before 之後的的 li::before 都會套用下面的 css

```css
.breadcrumb {
  + li::before {
    margin-right: 20px;
    color: #fff;
    content: ">";
  }
}
```

- 同一個群組的 CSS，可以使用%去宣告變數，用@extend 去使用。

編譯前

```scss
.txt-yellow {
  color: #ff0;
}

li {
  &:hover {
    @extend .txt-yellow;
  }
  &:last-of-type {
    @extend .txt-yellow;
  }
}
```

編譯後

```css
li:hover,
li:last-of-type {
  color: #ff0;
}
```
