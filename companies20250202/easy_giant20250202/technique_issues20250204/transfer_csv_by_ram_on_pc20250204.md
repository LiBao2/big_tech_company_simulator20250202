
copy file from office365/excel/google sheets/wps office/lark/feishu/dingtalk/wework/tencent docs


```python
import pyperclip
import pandas as pd
import io

data=pyperclip.paste()
data=io.StringIO(data)
data=pd.read_csv(data)


```
