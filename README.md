# smooth-scroll
页面内平滑滚动效果，支持滑动到指定的节点，支持调整过度的速度等。

- 设计思路 <br >
duration 做为整个平滑滚动的总时间，获取滚动区间，duration 除以 滚动区间得出滚动一个单位所需的时间，依据此时间作为定时器触发时间，实现均匀平滑滚动效果。
```
    activeTimeout = duration / (current - nextposition)
```
