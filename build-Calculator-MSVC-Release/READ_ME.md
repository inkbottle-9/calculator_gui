# **帮助**

---

## 程序描述
- 一个优化不太好的科学计算器.

## 当前版本
- V0.1.0(龟速更新中)

## 支持的功能
- 设置界面可以进行数学计算方面的格式设定以及单位选择.
- 自动保存所有运算记录,使用"上箭头"和"下箭头"来切换.
- 部分运算功能,选择编辑框内表达式的子集可以单独计算选中的子表达式.
- 常规数学错误以及表达式异常识别.
	

## 支持的操作符(大小写不敏感)

- 加号"**+**"
- 减号"**-**"
- 乘号"**\***"
- 除号"**/**"
- 幂"**^**"
- 阶乘"**!**"
- 取模"**%**"
- 对数"**log**"
- 正弦"**sin**"
- 余弦"**cos**"
- 正切"**tan**"
- 反正弦"**arcsin**"
- 反余弦"**arccos**"
- 反正切"**arctan**"
- 余切"**cot**",
- 排列"**ARR**"
- 组合"**COM**",
- 左括号"**(**"
- 右括号"**)**",
- 正号"**+**"
- 负号"**-**"
- 注: **优先级请结合生活实践自行脑补,不确定优先级请使用括号.**

## 两个内置常用常量(大小写敏感)

- **PI** (圆周率)
- **e** (自然对数)

## 合法表达式举例
```
((1+2)+5)/2
4*(1-3)/2
-sin(PI/6)
3!+2log16
4.7*(2+(5-3)!)
e^(sin(PI/2)*arcSIN(1))
2^(1+3!)
5ARR2+3com2
//(第一个'-'被识别为减号,其后的三个'-'被识别为负号)
1----5
+5-1/PI	
```

## 内置异常识别
- UnknownSymbol:未知符号(如试图计算表达式"Hallo+World"时抛出)
- BracketMismatching:括号不匹配(如试图计算表达式"(1+2"时抛出)
- NoOperand:无操作数(如试图计算表达式"+"时抛出)
- MathError:数学错误异常(如将0作为除数时抛出)
- ValueOverflow:数值溢出(计算表达式"1800!"时抛出)


## 注意事项
- 请不要在表达式内输入等于号;
- 表达式中的空格会被忽略;
- 不建议修改程序生成的配置文件config.conf
- 如果因为配置文件读取错误而打不开设置,(现在状态栏上面会高亮显示此类异常)  
  把config.conf文件删掉即可.

- 如果被类似于360的傻逼杀毒软件拦截,请添加信任,放心操作,
- 程序没有任何危害(360还是卸载了吧).  
  现在通过和360沟通官方已经修复了误拦截.

- 一般情况下程序会捕获计算过程中可能抛出的所有异常,不会崩;
- 如果程序崩了,请检查您的操作是否过于智障(-_-||),并且向作者汇报.
	
- 程序内部使用double作为数据存储类型,有效精度只有15位左右,  
  进行大数运算时请不要以程序显示的结果为准(只有前面15位左右是正确的数值)

## 闲话

- 不多说, 总之凑合用吧.

## 更新日志
```
    ------------------<版本 V0.1.0>------------------
    大更新! 修复了不少BUG(也许)!
    依然不收费! 瓶子良心!
    新特性:
    [1] 状态栏信息显示重写, 现在不会出现鬼畜现象
    [2] 使用全新的 QT 5.14, 支持MarkDown, 现在可以在程序里查看MD帮助文档了!
    [3] 修复了运算符结合性错误
    [4] 采用MSVC编译器! 体积更小, 速度更快!(不一定)

    已知BUG:
        暂时还没发现

```

```
	------------------<版本 V0.0.1>------------------
    第一个正式版本, 还是有很多问题
    新特性:
	[1] 加入状态栏,会显示一些实用信息(有一定BUG,我也修不好)
	[2] 更新的语法检查机制(BUG云集,有问题Call我)
	[3] 修正上个版本设置菜单单词的拼写错误
	[4] 支持使用逗号分隔符分隔数字(设置菜单的最后一条现在不再是摆设)

	已知BUG:
	[1]	运算符'*'乘号的优先级高于运算符'/'除号(结合性判断出错)
	[2]	程序开启时没有读取配置文件进行设置,而是使用了默认的设置
	以上BUG会在下一个版本修复(也许, 如果下一个版本存在的话)
```
```
	------------------<版本 V0.0.0>------------------
	最初始的测试版本, BUG云集. 能用就行, 不要在意
```


