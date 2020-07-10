# 파일에 읽고 쓰는 법

## 텍스트 파일 

- 코드에 있는 텍스트 내용을 파일에 기록하고 파일에서 텍스트를 읽어오는 방법

```python
with open('file.txt', 'r') as file:
    file.read()

with open('file.txt', 'w') as file:
    file.write("sth")
```



## 바이너리 파일

- 리스트나 데이터를 파일을 바이너리로 저장 혹은 불러오기

```python
import pickle
with open('data.p', 'rb') as file:
    pickle.load(file)
    
with open('data.p', 'wb') as file:
    pickle.dump("what", file)
```



## CSV 파일

```python
import pandas as pd
import csv
pd.read_csv('file.csv')
data.to_csv("file.csv", encoding = 'utf-8-sig')

```

