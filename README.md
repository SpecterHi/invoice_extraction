# PDF电子发票信息提取
## 1. 字段说明
PDF电子发票信息提取，从电子发票左上角的二维码中识别以下信息：  
 - 发票代码
 - 发票号码
 - 开票日期
 - 校验码
 - 价税合计（小写）
网上我也看过其他的通过提取PDF内容获取字段的解决方案。虽然有可能可以获取更多字段信息，但非常不稳定。因为电子发票虽然看起来一样，但背后的PDF格式千差万别。
## 2. 安装说明
本程序仅在`MacOS`搭配`python3`上测试过。
程序依赖包括`zbarlight`和`PyMuPDF`，然而这两个无法简单地通过`pip`安装。具体安装方法参见：
 - `zbarlight`：[https://pypi.org/project/zbarlight/](https://pypi.org/project/zbarlight/)
 - `PyMuPDF`：[https://pypi.org/project/PyMuPDF/](https://pypi.org/project/PyMuPDF/)
其他依赖通过`pip`安装即可：
```
pip install pillow pandas
```