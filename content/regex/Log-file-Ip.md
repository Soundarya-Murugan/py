---
title: Log-File-Ip
date: 2024-12-04
author: Your Name
cell_count: 6
score: 5
---

```python
#Log File IP Extractor
```


```python
import re
```


```python
import sys

```


```python
def extract_ips(log_data):
    ip_pattern = r'\b(?:\d{1,3}\.){3}\d{1,3}\b'
    ips = re.findall(ip_pattern, log_data)
    if ips:
        print("IP addresses found:")
        for ip in ips:
            print(ip)
    else:
        print("No IP addresses found.")

```


```python
if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: python script.py 'log data'")
    else:
        log_data = sys.argv[1]
        extract_ips(log_data)
```

    Usage: python script.py 'log data'



```python

```


---
**Score: 5**
