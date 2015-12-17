# Tabs

- category: Components
- chinese: 标签页
- type: 导航

---

选项卡切换组件。

## 何时使用

提供平级的区域将大块内容进行收纳和展现，保持界面整洁。

Ant Design 提供了三级选项卡，分别用于不同的场景。

- 卡片式的页签，用于容器顶部。
- 标准线条式页签，用于容器内部的主功能切换。
- [RadioButton](/components/radio/#demo-radiobutton) 作为更次级的页签来使用。

## API

### Tabs

| 参数             | 说明                                         | 类型     | 默认值        |
|------------------|----------------------------------------------|----------|---------------|
| activeKey        | 当前激活 tab 面板的 key                      | String   | 无            |
| defaultActiveKey | 初始化选中面板的 key，如果没有设置 activeKey | String   | 第一个面板    |
| onChange         | 切换面板的回调                               | Function | 无            |
| onTabClick       | tab 被点击的回调                             | Function | 无            |
| tabBarExtraContent | tab bar 上额外的元素                       | React Node | 无          |
| type | 页签的基本样式，可选 `line`、`card` `editable-card` 类型   | String   | 'line'      |
| tabPosition | 页签位置，可选值有 `top` `right` `bottom` `left`  | String   | 'top'      |
| onEdit | 新增和删除页签的回调，在 `type="editable-card"` 时有效 | Function(targetKey, action) | 无 |

### Tabs.TabPane

| 参数 | 说明             | 类型                    | 默认值 |
|------|------------------|-------------------------|--------|
| key  | 对应 activeKey   | String                  | 无     |
| tab  | 选项卡头显示文字 | React.Element or String | 无     |