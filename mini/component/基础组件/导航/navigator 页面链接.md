
# 简介
页面链接。导航栏相关设置请参见 [my.setNavigationBar](https://opendocs.alipay.com/mini/api/xwq8e6)。

## 使用限制
navigator 组件不支持 onTap 事件。

## 扫码体验
![|127x157](https://gw.alipayobjects.com/zos/skylark/f5c228d3-46e1-42d2-bc00-bfb4f48b726c/2018/jpeg/b69413a4-6c07-40df-bf34-be32a4987946.jpeg#align=left&display=inline&height=1906&margin=%5Bobject%20Object%5D&originHeight=1906&originWidth=1540&status=done&style=none&width=127)

# 使用

## Herbox
[小程序在线](https://herbox-embed.alipay.com/s/doc-navigator?theme=light&previewZoom=75&chInfo=openhome-doc) 

## 示例代码

### .axml 示例代码
```html
<!-- API-DEMO page/component/navigator/navigator.axml -->
<view class="page">
  <view class="page-description">导航栏</view>
  <navigator open-type="navigate" url="./navigate" hover-class="navigator-hover">跳转到新页面</navigator>
  <navigator open-type="redirect" url="./redirect" hover-class="navigator-hover">在当前页打开</navigator>
  <navigator open-type="switchTab" url="/page/API/index/index" hover-class="navigator-hover">跳转到另外一个 Tab - API</navigator>
  <navigator open-type="reLaunch" url="/page/component/index" hover-class="navigator-hover">重新打开</navigator>
  <navigator open-type="navigateBack" hover-class="navigator-hover">返回上一页面</navigator>
</view>
```

### .js 示例代码
```javascript
// API-DEMO page/component/navigator/navigator.js
Page({});
```

### .acss 示例代码
```css
/* API-DEMO page/component/navigator/navigator.acss */
navigator {
  background-color: lightcoral;
  color: #fff;
  margin-bottom: 10rpx;
  padding: 20rpx;
  text-align: center;
}
.navigator-hover {
  background-color: lightskyblue;
  color: #fff;
}
```

## 属性说明
| **属性** | **类型** | **描述** |
| --- | --- | --- |
| open-type | String | 跳转方式。<br />**默认值：** navigate |
| hover-class | String | 点击后的样式类。<br />**默认值：** none |
| hover-start-time | Number | 按住后多少时间后出现点击状态，单位 ms。 |
| hover-stay-time | Number | 手指松开后点击状态保留时间，单位 ms。 |
| url | String | 当前小程序内的跳转链接。 |


###  open-type 有效值
| **属性** | **描述** |
| --- | --- |
| navigate | 对应 [my.navigateTo](/mini/api/zwi8gx) 的功能。 |
| redirect | 对应 [my.redirectTo](/mini/api/fh18ky) 的功能。 |
| switchTab | 对应 [my.switchTab](/mini/api/ui-tabbar) 的功能。 |
| navigateBack | 对应 [my.navigateBack](/mini/api/kc5zbx) 的功能。 |
| reLaunch | 对应 [my.reLaunch](/mini/api/hmn54z) 的功能。 |


# 相关文档

- [my.navigateTo](https://opendocs.alipay.com/mini/api/zwi8gx)
- [my.navigateBack](https://opendocs.alipay.com/mini/api/kc5zbx)
