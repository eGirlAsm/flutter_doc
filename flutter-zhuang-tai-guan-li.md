# flutter 状态管理

虽然之前曾经小小入门过react,但实际上仍然是不知所云。

比如说这个状态\(stateFulWidget\)概念来自react。

不说别的直接把官网的核心内容复制过来。

```
重点：

要创建一个自定义有状态widget，需创建两个类：StatefulWidget和State
状态对象包含widget的状态和build() 方法。
当widget的状态改变时，状态对象调用setState()，告诉框架重绘widget
```

我最喜欢菜单栏就用菜单栏把，很多官方案例都是按钮，实在没意思。

我自己也是边学边写文，瞎整了一个出来，还是很满意的，除了变量内容有点多余之外。

```
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(home: ZhuangTai()));
}

class ZhuangTai extends StatefulWidget{
  @override
  _ZhuangtaiState createState()=> new _ZhuangtaiState();
}


class _ZhuangtaiState extends State<ZhuangTai>{
  String _shenme = "qunima";

  void _setZhuangTai(int nIndex){
    setState((){
      if(_shenme == "qunima" && nIndex == 1){
        _shenme = "nimabi";
      }else{
        _shenme = "qunima";
      }
    });
  }

  @override
  Widget build(BuildContext context){
    return new Scaffold(
      body: Center(
        child: Text(_shenme,textDirection:TextDirection.ltr),
      ),
      bottomNavigationBar:BottomNavigationBar(
        items: <BottomNavigationBarItem>[
          BottomNavigationBarItem(icon: Icon(Icons.home),title: Text('qunima')),
          BottomNavigationBarItem(icon: Icon(Icons.home),title: Text("nimabi")),
        ],
        onTap: _setZhuangTai,
      ),
    );
  }
}
```



