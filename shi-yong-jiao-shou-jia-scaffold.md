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

我不知道大家喜不喜欢看小说，我以前看很多。其中我最喜欢的app就是追书神器了。

我们编译完上面的代码之后发现列表根本不像列表，反而像是一行行文字。

那我们就给他们加点图片，让app看起来像个小说app。

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
                Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
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

最后我们还是给他们加个耳朵（左右上角图标）吧，送佛送到西嘛。

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
            leading: Icon(Icons.verified_user),
            actions: <Widget>[
              IconButton(icon: Icon(Icons.search),tooltip: 'alsdkjfla',),
              IconButton(icon: Icon(Icons.settings),)
            ],
          ),
          body: Center(
            child: ListView(
              padding: EdgeInsets.all(8.0),
              children: <Widget>[
                Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
                        Row(children: <Widget>[
                  Expanded(child: Icon(Icons.screen_lock_landscape),),
                  Expanded(child: Text('小说标题'),)
                ],),
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

这里把官网的图片复制过来。

![](/assets/header.png)



最后效果预览图

![](/assets/screen.png)

