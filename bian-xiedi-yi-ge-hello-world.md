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

TextDirection 应该是左对齐 右对齐 。

