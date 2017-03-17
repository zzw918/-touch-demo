## 模仿移动端的下拉刷新 ##

> 使用了移动端的touch事件
### 四个touch事件
1.touchstart：只要将手指放在了屏幕上（而不管是几只）,都会触发touchstart事件。

2.touchmove: 当我们用手指在屏幕上滑动时，这个事件会被连续触发。 如果我们不希望页面随之滑动，我们可以使用event的preventDefault来阻止这个默认行为。

3.touchend: 当手指滑动后离开屏幕，这时就触发了touchend事件。

4.touchcancel: 系统停止跟踪触摸时候会触发。例如在触摸过程中突然页面alert()一个提示框，此时会触发该事件，这个事件比较少用。

### 四个touch对象 ###
1. touches，这是一个类数组对象，包含了所有的手指信息，如果只有一个手指，那么我们用touches[0]来表示。

2. targetTouches 。 手指在目标区域的手指信息。

3. changedTouches：最近一次触发该事件的手指信息。

4. touchend时，touches与targetTouches信息会被删除，changedTouches保存的最后一次的信息，最好用于计算手指信息。



> [更多示例可以看我的博客](http://www.cnblogs.com/zhuzhenwei918/p/6412138.html)

