* 日期范围，只可选择昨天及最近60天  
el-date-picker type="daterange"

```
pickerOptions1: {
    disabledDate (time) {
        return time.getTime() > Date.now() - 3600 * 1000 * 24 || time.getTime() < Date.now() - 3600 * 1000 * 24 * 60
    }
}
```