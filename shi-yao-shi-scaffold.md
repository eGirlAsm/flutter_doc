# 什么是 scaffold

网上教程很多，它就是一个脚手架,提供一些基本的东西。真正的项目应该用不上? 因为大家都喜欢自定义嘛。

比如navigation,bottom bar,float 按钮之类的。我们还是直观的看一下 官方的文档。

```
Properties（属性）

appBar → PreferredSizeWidget （手机上面的额头部分）
An app bar to display at the top of the scaffold.
final
backgroundColor → Color
The color of the Material widget that underlies the entire Scaffold. [...]

final
body → Widget (手机内容部分)
The primary content of the scaffold. [...]

final
bottomNavigationBar → Widget (底部导航栏)
A bottom navigation bar to display at the bottom of the scaffold. [...]

final
bottomSheet → Widget
The persistent bottom sheet to display. [...]

final
drawer → Widget
A panel displayed to the side of the body, often hidden on mobile devices. Swipes in from either left-to-right (TextDirection.ltr) or right-to-left (TextDirection.rtl) [...]

final
endDrawer → Widget
A panel displayed to the side of the body, often hidden on mobile devices. Swipes in from right-to-left (TextDirection.ltr) or left-to-right (TextDirection.rtl) [...]

final
floatingActionButton → Widget
A button displayed floating above body, in the bottom right corner. [...]

final
floatingActionButtonAnimator → FloatingActionButtonAnimator
Animator to move the floatingActionButton to a new floatingActionButtonLocation. [...]

final
floatingActionButtonLocation → FloatingActionButtonLocation
Responsible for determining where the floatingActionButton should go. [...]

final
persistentFooterButtons → List<Widget>
A set of buttons that are displayed at the bottom of the scaffold. [...]

final
primary → bool
Whether this scaffold is being displayed at the top of the screen. [...]

final
resizeToAvoidBottomPadding → bool
Whether the body (and other floating widgets) should size themselves to avoid the window's bottom padding. [...]

final
hashCode → int
The hash code for this object. [...]
read-only, inherited
key → Key
Controls how one widget replaces another widget in the tree. [...]
final, inherited
runtimeType → Type
A representation of the runtime type of the object.
read-only, inherited
```

到这里大家应该是对界面有所了解了。

当学到这里，再回去看官方的教程一目了然了。我直接复制粘贴。

# Flutter教程

**Flutter 教程**教你如何使用Flutter框架构建iOS和Android移动应用程序

* [在Flutter中构建布局](https://flutterchina.club/tutorials/layout/)
  如何使用Flutter的布局机制来构建布局。学习完基本原理后，您将构建一个示例屏幕截图的布局
* [为Flutter App添加交互](https://flutterchina.club/tutorials/interactive/)
  您将扩展在“在Flutter中构建布局”中创建的简单布局应用，以使图标可点击。还讨论了管理widget状态的不同方式。
* [Flutter中的动画](https://flutterchina.club/tutorials/animation/)
  解释了Flutter动画包（控制器、动画、曲线、监听器、构建器）中的基本类，因为它会使用各种动画API来帮助您了解补间动画的过程。
* [国际化Flutter Apps](https://flutterchina.club/tutorials/internationalization/)
  了解如何国际化您的Flutter应用程序。通过widget和类的指南，使应用程序能够使用用户的语言和格式习惯显示其内容。



