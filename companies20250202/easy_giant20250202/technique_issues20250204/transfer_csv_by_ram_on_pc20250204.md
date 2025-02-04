
copy file from office365/excel/google sheets/wps office/lark/feishu/dingtalk/wework/tencent docs


```python
import pyperclip
import pandas as pd
import io

data=pyperclip.paste()
data=io.StringIO(data)
data=pd.read_csv(data,sep='\t')


```

```python
#data=data.to_string(index=False)
data_out=io.StringIO()
data.to_csv(data_out,index=False)
data_out.seek(0)
print(data_out.read())
```

