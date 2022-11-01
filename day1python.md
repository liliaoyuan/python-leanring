# day 1

### python 继承

```py
from PIL import Image

im=Image.open(path)
```

这里可以看到Im被定义幅值，之后可以继承所有属性

### PIL库用法

```python
from PIL import Image,ImageDraw,ImageFont #分别引用Image,ImageDwaw,ImageFont三个类
import os
import math

path="C:/Users/Merlinlee/Desktop/HollewayWork.jpg"#图片路径
im=Image.open(path)#读取头像图片
text='3'#未读消息的数量
w,h=im.size
print(w,h)
draw= ImageDraw.Draw(im)
myfont=ImageFont.truetype("C:/Windows/Fonts/simhei.ttf",int(w/5))#选择字体，并设置大小
draw.ellipse([0,0,20,70],fill="red")#画圆圈
draw.text((50,81),text,"white",myfont)
# im.show()
img=im.resize((128,128))
img.save("0000.jpg")
img.show()
# current_path=os.path.abspath("0000.jpg")
# print(current_path)

```

简单的画图库PIL

w,h = im,size //宽高定义成图像的像素多少

.ellipse参数中坐标的定义，很容易超出边界