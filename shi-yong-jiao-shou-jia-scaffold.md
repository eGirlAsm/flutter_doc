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

相当于没装修的房子和装修好了的房子。

我们这次给它盖个马桶，也就是底部的tab按钮。不然都不能说这是一个app了。

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
          bottomNavigationBar: BottomNavigationBar(
            items: <BottomNavigationBarItem>[
              BottomNavigationBarItem(icon: Icon(Icons.home),title:Text('home')),
              BottomNavigationBarItem(icon: Icon(Icons.business),title:Text('home')),
              BottomNavigationBarItem(icon: Icon(Icons.school),title:Text('home')),
            ],
          ),
        )
      );
    }
}
```

等菜单出现了。

我们再让他更接近一个app

比如给空白的内容里加点家具。

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
            child: ListView(
              padding: EdgeInsets.all(8.0),
              children: <Widget>[
                const Text('这是我2019年1月22日的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
                const Text('这是我1月30的日记'),
              ],
            )
          ),
          bottomNavigationBar: BottomNavigationBar(
            items: <BottomNavigationBarItem>[
              BottomNavigationBarItem(icon: Icon(Icons.home),title:Text('home')),
              BottomNavigationBarItem(icon: Icon(Icons.business),title:Text('home')),
              BottomNavigationBarItem(icon: Icon(Icons.school),title:Text('home')),
            ],
          ),
        )
      );
    }
}
```



