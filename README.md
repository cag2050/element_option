* 日期范围，只可选择昨天及最近60天  
el-date-picker type="daterange"

```
pickerOptions1: {
    disabledDate (time) {
        return time.getTime() > Date.now() - 3600 * 1000 * 24 || time.getTime() < Date.now() - 3600 * 1000 * 24 * 60
    }
}
```

* 让 el-tree 出现滚动条。  
出处：https://github.com/ElemeFE/element/issues/4456  
加入样式：  
```
.el-tree-node>.el-tree-node__children {
    overflow: inherit;
    background-color: transparent;
}
```
