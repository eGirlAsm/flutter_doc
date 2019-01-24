# 使用脚手架 scaffold

直接看示例代码

```
import 'package:flutter/material.dart';

void main(){

runApp(
  new MyApp()
);

}

class MyApp extends StatelessWidget{
  @override
  Widget build(BuildContext context) {
      // TODO: implement build
      return MaterialApp(
        title: 'first app',
        home:Scaffold(
          appBar:AppBar(
            title: Text('top bar title'),
          ),
          body: Center(
            child: Text('hellasldjfl')
          ),
        )
      );
    }
}
```

原先只是hello world的时候 一片黑暗,只有文字。

而这次有头有背景。这就是别人为我们搭建好了架子,直接写进去内容就行了。

