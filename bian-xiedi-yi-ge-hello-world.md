# 编写第一个 Hello world

```
import 'package:flutter/material.dart';

void main(){

runApp(
  Center( 
    child:Text('hello world',textDirection: TextDirection.ltr,)
  )
);

}
```

这应该是史上最简单的flutter 入门了。

我试了把 textDirection属性去掉结果报错。

TextDirection 应该是文章左对齐 右对齐 。

#### 试试更改

试着把Center改成了 Container 按SHIFT + F5 停止调试,然后再Command + SHIFT + F5 重新调试。

结果文字跑左上角去了。

```
import 'package:flutter/material.dart';

void main(){

runApp(
  Container( 
    child:Text('hello world',textDirection: TextDirection.ltr,)
  )
);

}
```

查了文档 发现container是这样一个东西

![](/assets/container.png)

还可以用其他widget组件 

```
import 'package:flutter/material.dart';

void main(){

runApp(
  Padding(
    padding: EdgeInsets.all(90.0),
    child: Text('hello world',textDirection: TextDirection.ltr,),
  )
);

}
```



