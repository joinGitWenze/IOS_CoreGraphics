# IOS_CoreGraphics
     CoreGraphics是提供2D绘图的框架,使用C结构和C函数模拟了一套面向对象的变成机制,没有OC/Swift对象方法机制;2D绘图并不能操作单独的像素;所以绘制机制都是在context上下文进行的.数据结构和函数可以通过CG来识别.
    
     CoreGraphics的优点:
     
     1 快速,高效绘图,可以减少文件大小
     
     2 可以自由使用动态的,搞质量的图像
     
     3 可以创建直线,路径,渐变,文字与图像等内容,并可以做变现处理
     
     CGContextRef:获取上下文画布:CGContextRef ctx =  UIGraphicsGetCurrentContext();
     CGContextAddRect:绘制闭合曲
     CGContextSetFillColorWithColor:设置填充颜色
     CGContextFillPath:填充路径
     (1) 绘制一个矩形 
     CGContextRef ctx =  UIGraphicsGetCurrentContext();
     CGContextAddRect(ctx, rect);
     CGContextSetFillColorWithColor(ctx, [UIColor greenColor].CGColor);
     CGContextFillPath(ctx);

     
   
