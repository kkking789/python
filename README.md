# BingSpyderDataSetCreater
python相关库
这是一个用来爬bing图片做分类数据集的简易爬虫

可以自定义爬的图片的数量，以及爬的种类
每次下载图片的time.sleep最好不要低于0.3，不然有被封IP的风险，可以把等待时间调小点，这样下的快
headers可以在浏览器的开发者模式下找到，具体从网上查怎么找
另外引入了一个额外的库PIL，下载方式直接命令窗输入 pip install Pillow 即可

这份爬虫对下载的图片的宽长积存在一定限制，这样防止下载到奇奇怪怪的图标，来污染数据集

想要自定义一些参量的话可以直接改default的值，也可以在命令窗输入

python main.py --你想要修改的参量1=你想要把它改成的值1 --你想要修改的参量2=你想要把它改成的值2
并运行

另外，为什么整个世界上有FPGA这么恶心的东西啊，服了

Version: 1.1:

添加了自动创建数据集的文件夹
在下载图片时随机抽取10张图片，5张放进测试集，5张放入验证集，其余放入训练集

Author: kkking789
Date: 23.11.28
Version: 1.1
