# 什么是 scaffold

网上教程很多，它就是一个脚手架,提供一些基本的东西。真正的项目应该用不上?

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



