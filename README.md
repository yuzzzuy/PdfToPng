
## 主要简介
 - 项目名：PDF转IMG
 - 主要技术：Java(项目为Java普通项目）  
 - 主要功能：  
    - 把PDF格式文件转化为多个单img图片并存放到同级目录新建的同名文件夹中
    - 把PDF格式文件转化为单个img图片（长图）并存放到自定义的路径下
 - 使用说明：引入依赖包直接调用工具类即可  
## 内部方法
#### pdfToImagePath（String filePath）
- 参数：
-- filePath:pdf的绝对路径
- 功能
-- 将PDF按页数每页转换成一个jpg图片
### pdfmultiImage(String filePath, String outPath)
- 参数 
-- filePath:pdf的绝对路径
-- outPath：输出图片的绝对路径
- 功能
-- 将PDF中的每一页当成一个图片存放到数组中
### PicFixY(List<BufferedImage> piclist, String outPath)
- 参数
-- piclist：图片数组
-- outPath：输出图片的绝对路径
- 功能
-- 将图片数组中的图片按照下标拼接成一个从上自下的长图
## 使用的依赖包  
 - fontbox-2.0.15  
 - pdfbox-2.0.15  
 - commons-logging-1.2