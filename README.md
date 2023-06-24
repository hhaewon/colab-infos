# colab-infos
제가 코랩에서 코딩을 했을 때 유용했던 정보들을 모아 두었습니다.

## contents
- - -
### 모든 줄 `print` 없이 출력
```python
from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"
```
을 실행하면 가장 끝 줄만 `print`없이 출력되는 것이 아니라 모든 줄에서 `print`없이 예쁘게 출력되게 됩니다.  
*ex)*  
추가 ❌
```python
df = pd.DataFrame({ 'name': ['김태훈','이유정','장서희'],
                    'eng':  [90,80,70],
                    'math': [77,66,88]  })
df
df.tail()
df.head()
```
*output*
```
2
```
추가 ⭕
```python
from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"
a = 3
b = 2
a + b
a
b
```
*output*
```
2
```
