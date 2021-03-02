# PrettyRuler
一个漂亮的横向刻度尺自定义控件，用CAShapeLayer实现高效GPU渲染，没有用一张图片！
控件两边添加渐变透明效果，看起来更加自然。使用方法具体看demo，简单易懂，几句代码搞定，但是该自定义控件只支持代码方式创建。

#说明
iOS7 +，刻度选择支持选择0值，为最小模式，不能选择0值时候，为正常模式，具体请看最下面效果图。

#支持pod安装
pod 'PrettyRuler', '~> 2.1.1'

#用法
1. 拖拽class文件夹到你的项目
2. 在你的控制器里导入 `TXHRrettyRuler.h` 类
3. 类似以下这段代码
	  
	  ```
	  TXHRrettyRuler *ruler = [[TXHRrettyRuler alloc] initWithFrame:CGRectMake(20, 220, [UIScreen mainScreen].bounds.size.width - 20 * 2, 140)];
	ruler.rulerDeletate = self;
	[ruler showRulerScrollViewWithCount:200 average:1 currentValue:36.5f smallMode:YES];
	[self.view addSubview:ruler];
	  ```
	
#效果图

![test](![](https://raw.githubusercontent.com/AsTryE/Images/master/Resoures/IMG_6448DF40A3D8-1.jpeg))
