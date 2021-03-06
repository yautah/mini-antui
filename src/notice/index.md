## Notice
| 属性 | 说明 | 类型 | 默认值 |
|----|----|----|----|
|mode| 提示类型,link,closable,'' | String|''|
|action| 提示显示文本| String|''|
|show| 是否显示通告栏| boolean|true|
|onClick| 点击按钮回调 | (): void| - |

### using

```json
// page.json
{
  "defaultTitle": "小程序AntUI组件库",
  "usingComponents":{
    "notice":"mini-antui/es/notice/index"
  }
}
```

### examples

```xml
// page.axml
<view class="demo-title">NoticeBar 通告栏</view>
<view class="demo-item">
    <notice>因全国公民身份系统升级，添加银行卡银行卡银行卡银行卡</notice>
</view>
<view class="demo-item">
    <notice mode="link" onClick="linkClick">因全国公民身份系统升级，添加银行卡银行卡银行卡银行卡</notice>
</view>
<view class="demo-item">
    <notice mode="closable" onClick="closableClick" show="{{closeShow}}">因全国公民身份系统升级，添加银行卡银行卡银行卡银行卡</notice>
</view>
<view class="demo-item">
    <notice mode="link" action="去看看" onClick="linkActionClick">因全国公民身份系统升级，添加银行卡银行卡银行卡银行卡</notice>
</view>
<view class="demo-item">
    <notice mode="closable" action="不再提示" onClick="closableActionClick" show="{{closeActionShow}}">因全国公民身份系统升级，添加银行卡银行卡银行卡银行卡</notice>
</view>

```
