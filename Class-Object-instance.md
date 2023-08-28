## for Class and Instance as well as object
*Class for python is reussable function and variable*

``` python
class Human: # First letter upper is a rule
  def use_python():
    print("hello_world" + self.name) 
```
> self here refer to the variable it creastes like below
``` python
h1 = Human()
h1.name = "xioaowei"
h1.use_python

```
``` python
h2 = Human()
h2.name = "QiuBao"
h2.use_python

```
as  you can see, this is very complex and redundant since you have define every attribute(the variable) at all time

Thus Orient Object languages introduce contributor to solve this problem.
**For python**
we got this contributor
```python
 def __init__(self,name,color,weight) :
        self.name = name
        self.height = height
        self.weight = weight
```
so here IF I go
```python
h3 = Human("qiubao","black",28)
h2.use_python()
```
we get `hello_worldqiubao`

### The looking up
> let us think in a hardware way
> 1. if you have a `dot` expression in your code what will the computer do
>    1. Fisrt, the CU would depend whether the instance has the attributes
>    2. If not they will look up the class defination
Here you may have a idea about the instance, the real object created in a class like (h1 h2 h3)  as above 
