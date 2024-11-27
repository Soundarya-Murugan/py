---
title: Ip-Addr-Validator
date: 2024-11-27
author: Your Name
cell_count: 8
score: 5
---

```python
#Validates if a string is a valid IPv4 address.
```


```python
import re


```


```python
def is_valid_ip(ip):
    ip_regex = r'^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$'
    return bool(re.match(ip_regex, ip))


```


```python
# Test cases

```


```python
ips = [
    "192.168.1.1",
    "255.255.255.255",
    "0.0.0.0",
    "300.168.1.1",
    "abc.def.ghi.jkl"
]

```


```python
#Print valid 
```


```python

for ip in ips:
    print(f"{ip}: {'Valid' if is_valid_ip(ip) else 'Invalid'}")
```

    192.168.1.1: Valid
    255.255.255.255: Valid
    0.0.0.0: Valid
    300.168.1.1: Invalid
    abc.def.ghi.jkl: Invalid



```python

```


---
**Score: 5**
