## 按字符串值查找枚举类型

### 问题：
假设我有一个如下的枚举类型

```
public enum Blah {
    A, B, C, D
}
```

然后我想找到一个字符串所对应的枚举类型值，比如`“A”`对应`Blah.A`。怎么才能做到这一点？

我需要用到的是`Enum.valueOf()`这个方法吗？如果是，我该如何使用它？

### 回答：
是的，`Blah.valueOf("A")`会返回给你`Blah.A`。

静态方法`valueOf()`和`values()`是在编译时被创建的而并不存在在源代码里。不过它们出现在Javadoc里，比如，[`Dialog.ModalityType`](http://docs.oracle.com/javase/7/docs/api/java/awt/Dialog.ModalityType.html)



**stackoverflow链接：**
http://stackoverflow.com/questions/604424/lookup-enum-by-string-value