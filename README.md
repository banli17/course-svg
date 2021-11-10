# course-svg

## svg 常用场景

-   iconfont
-   动画

## svg viewport 和 viewBox

- viewport 是 svg 的可见区域, 即 svg 标签的 width 和 height。
- viewBox 是用于画布上绘制 svg 图形的坐标系统

相当于是首先在 viewBox 绘制，最后缩放到 viewport 大小。

- preserveAspectRatio 用于指定当 viewport 和 viewBox 长宽比不同时，在 viewport 的显示情况, 同时也可以指定在 viewport 坐标系的位置， xMinYMid meet
  - 第一个参数 xMinYMid 指定了 viewBox 在 viewport 坐标系中的位置。xMin 左边对齐 xMid 中 xMax 右边对齐   yMax 下边对齐
  - 第二个参数
      - meet 保持宽高比，并将 viewBox 缩放为 适合 viewport 的大小, 相当于 contain
      - slice 保持宽高比，并将所有不在 viewport 中的 viewBox 裁剪掉。相当于 cover
  none 不保持宽高比, 会进行拉伸铺满
这个比例会用于乘以 绘制图形的宽高 边框等。

## svg 组件

- defs
- g 将元素放到一组，但是不能指定 viewBox, 需要 use 时，在外面 svg 指定
- symbol 替换 g， 可以指定 viewBox
- use href=#
