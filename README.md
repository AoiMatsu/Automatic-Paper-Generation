# 自动组卷系统

 
  本人非CS专业，项目为大三选修的python课的期末设计，是一个小白第一个正式的项目。(虽然是东拼西凑)
  
  本程序使用pycharm集成开发环境，采用 Qt designer + PyQt5 设计界面，代码使用的核心库是PyQt5以及docx，由于PyQt5与docx存在某种不兼容问题，以至于我试过很多方法仍然无法封装，问题截图如下：
  
[![1.md.jpg](https://img.xhacgn.com/images/2023/01/06/1.md.jpg)](https://img.xhacgn.com/image/Z577n)

[![R2J4AJ07LEFUVKHGP_T.md.png](https://img.xhacgn.com/images/2023/01/06/R2J4AJ07LEFUVKHGP_T.md.png)](https://img.xhacgn.com/image/Z5wzT)

pyinstaller -F -w ALL.py --hidden-import PySide2.QtXml  

* * *

所以，具体使用方法如下：

①将文件夹(AutomaticPaperGeneration)整体导入pycharm，打开ALL.py

[![2NXU7KPPJ9L40Q.md.png](https://img.xhacgn.com/images/2023/01/06/2NXU7KPPJ9L40Q.md.png)](https://img.xhacgn.com/image/Z59Pw)

②终端中安装PyQt5与docx库
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple pyqt5
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple docx

③运行ALL.py代码，进入登录界面

[![JBDYXYUNO1NGC92BG6.md.png](https://img.xhacgn.com/images/2023/01/06/JBDYXYUNO1NGC92BG6.md.png)](https://img.xhacgn.com/image/Z5E4G)

目前教师端阅卷功能尚未实现，选择学生端，用户名输入：Admin 密码输入：111111
然后根据提示进入答题界面——

[![L8LGTC8R7O43C2ZB.md.png](https://img.xhacgn.com/images/2023/01/06/L8LGTC8R7O43C2ZB.md.png)](https://img.xhacgn.com/image/Z5Fv3)

④(学生)进入答题界面后，点击右方答题卡题号进行作答。

[![O6W6FV3NDUWFEVUBJYY.md.png](https://img.xhacgn.com/images/2023/01/06/O6W6FV3NDUWFEVUBJYY.md.png)](https://img.xhacgn.com/image/Z5H1Y)

(1)目前题库比较小，1~3题是选择题，4~6题是填空题，7~9题是判断题

(2)目前填空题暂时无法机器阅卷

(3)每次进入答题界面，题目都不同，题目是随机从题库提取并排序的。目前每种题型题库10道题，每种题型随机抽取3道。

(4)目前分数系统还存在bug，导致最终总分计算出错


* * *

附录：
①Qt designer部分
界面ui设计——

[![5_JVEFWI5C7PRUGY.md.png](https://img.xhacgn.com/images/2023/01/06/5_JVEFWI5C7PRUGY.md.png)](https://img.xhacgn.com/image/Z5dmP)

[![UUU9FIPFE_G7X7A9.md.png](https://img.xhacgn.com/images/2023/01/06/UUU9FIPFE_G7X7A9.md.png)](https://img.xhacgn.com/image/Z5rHB)
