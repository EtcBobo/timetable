/*
Title: popoPicker
Description: popoPicker
*/

# 功能描述
popoPicker是一个仿iOS的3d滚轮选择器，无依赖，仅13kb

# 依赖模块
无

# 快速使用

```js
//Picker
new popoPicker('.js-picker', {
    wheels: [{
        infinite: false,
        //selected: 3,
        data: [
            { value: 0, display: '选项一' },
            { value: 1, display: '选项二' },
            { value: 2, display: '选项三' },
            { value: 3, display: '选项四' },
            { value: 4, display: '选项五' },
            { value: 5, display: '选项六' },
            { value: 6, display: '选项七' }

        ]
    }],
    background: 'dark'
});

//Date
new popoDateTime('.js-date', {
    time: false,
    background: 'light'
});

//Time
new popoDateTime('.js-time', {
    date: false,
    background: 'dark'
});

//DateTime
new popoDateTime('.js-datetime', {
    background: 'dark'
});
```

## popoPicker配置项

### wheels
* 类型：Array
* 默认值：[]
* 作用：滚轮的数据内容
* 是否必传：是
### container
* 类型：String
* 默认值：body
* 作用：选择器所在的父级
* 是否必传：否
### scrollType
* 类型：String
* 取值：2d|3d
* 默认值：3d
* 作用：滚轮的显示模式
* 是否必传：否
### background
* 类型：String
* 取值：light|dark
* 默认值：light
* 作用：主题背景颜色
* 是否必传：否
### display
* 类型：String
* 默认值：bottom
* 作用：滚轮显示位置
* 是否必传：否
### headTitle
* 类型：String
* 默认值：无
* 作用：滚轮顶部标题
* 是否必传：否
### init
* 类型：Function
* 作用：初始加载完成后执行
* 是否必传：否
### getResult
* 类型：Function
* 作用：返回滚动时的结果
* 是否必传：否
### save
* 类型：Function
* 作用：点击确定
* 是否必传：否
### cancel
* 类型：Function
* 作用：点击取消
* 是否必传：否

## popoDateTime配置项

### container
* 类型：String
* 默认值：body
* 作用：选择器所在的父级
* 是否必传：否
### scrollType
* 类型：String
* 取值：2d|3d
* 默认值：3d
* 作用：滚轮的显示模式
* 是否必传：否
### background
* 类型：String
* 取值：light|dark
* 默认值：light
* 作用：主题背景颜色
* 是否必传：否
### display
* 类型：String
* 默认值：bottom
* 作用：滚轮显示位置
* 是否必传：否
### date
* 类型：Boolean
* 默认值：true
* 作用：是否显示日期
* 是否必传：否
### time
* 类型：Boolean
* 默认值：true
* 作用：是否显示时间
* 是否必传：否
### save
* 类型：Function
* 作用：点击确定
* 是否必传：否
### cancel
* 类型：Function
* 作用：点击取消
* 是否必传：否

# 特别说明
更多配置和用法，请参考[popoPicker](https://github.com/po-po/popoPicker)