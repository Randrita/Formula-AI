```python
import os
#import urllib.urlopen
from urllib.request import urlopen
from json import load
import json
import requests

```


```python
while True:
    IP=input("Type your target IP : ")
    url="http://ip-api.com/json/"
    response=urlopen(url+IP)
    data=response.read()
    values=json.loads(data)
    
    print(" IP: " + values['query'])
    print(" City: " + values['city'])
    print(" ISP: " + values['isp'])
    print(" Country: " + values['country'])
    print(" Region: " + values['region'])
    print(" Time zone: " + values['timezone'])
    
    break




    
```

    Type your target IP : 43.252.249.128
     IP: 43.252.249.128
     City: Kolkata
     ISP: Alliance Broadband Services
     Country: India
     Region: WB
     Time zone: Asia/Kolkata
    


```python

```
