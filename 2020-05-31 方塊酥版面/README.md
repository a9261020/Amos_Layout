# 2020-05-31 方塊酥版面

![成品](./completed.jpg)

## 重點整理

- CSS 中的(~)選取器會影響後方全部元素

```html
<div>
  <div>001</div>
  <div><p>002</p></div>
  <p>003</p>
  <p>004</p>
</div>
```

```css
div ~ p {
  font-size: 20px;
  color: #000;
}
```

003 004 都會變成黑色的字體
