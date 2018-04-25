## 命名规范

* 命名使用英文单词，不允许使用拼音，要见名知意，不常见的词要添加中文注释。

* 当表示数组列表等可数名词要加 `s` 后缀，js 里由于没有类型，不知道是否是数组，推荐不可数名词也加上 `s` 以示区别，ts 在有类型声明的情况下可以不用加。

* 函数方法名中动词使用一般现在时，`getXXX()，fetchData()`...

* 表生命周期的方法可以加时态，例如 react 式的 didMount, vue 式的  mounted

* 布尔值加上 `is` 前缀，`isOK`, 表状态时加上时态，`isLoading，isLoaded`

* 原则上任何命名不允许缩写

* 单个单词坚决不允许缩写，例如 `password => pwd`, 但一些常见的除外，例如 `Accessibility => a11y, internationalization => i18n`

* 拼接词长度超过 20 个可以使用缩写

  - 缩写时采用常见的缩写方式（以能猜出单词意思或音译出为佳）例如: `button => btn`

  - 其余缩写方式以缩写单词前面字母为主，例如 `parameters => params`

  - 如果单词实在过长或单词过多，采用缩写首字母方式， 例如 `Hypertext Markup Language => HTML`，表明变量或方法的主要单词尽量不要缩写。

  - 缩写词必须添加完整的单词注释，不常见的词要添加中文注释。

* react 组件内处理DOM事件的方法名统一以 `handle` 开头，当组件内部只有一个 click 事件时，可以使用 handleClick , 但不推荐，如果事件较多时，坚决不允许 handleClick1, handleClick2.

* react 组件向外部暴露的 DOM 事件类型的 props 以 `on` 开头，例如 `onClick={xxx}`，不是 dom 事件的普通函数 props 坚决不要添加 on 前缀。

