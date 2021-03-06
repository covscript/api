## 分支语句

```
if 逻辑表达式

    语句块

end
```
* 逻辑表达式的值为真则执行语句块


```
if 逻辑表达式

    语句块1

else

    语句块2

end
```
* 逻辑表达式的值为真则执行语句块1
* 逻辑表达式的值为假则执行语句块2


```
switch 表达式

    case 常量标签

        语句块

    end

    default

        语句块

    end

end
```
* 执行与表达式的值相等的常量标签对应的case中的语句块
* 当无匹配的常量标签时会执行default中的语句块，如default未找到则跳出
* 常量标签的类型必须支持生成哈希值

## 循环语句

```
while 逻辑表达式

    语句块

end
```
* 当逻辑表达式的值为真时循环执行语句块


```
loop

    语句块

until 逻辑表达式
end
```
* 直到逻辑表达式的值为真时跳出循环


```
loop

    语句块

end
```
* 循环执行语句块直到用户手动跳出


```
for 变量名 = 表达式 to 表达式

    语句块

end
```
* 定义一个变量在闭区间中遍历，步长为 `1`


```
for 变量名 = 表达式 to 表达式 step 表达式

    语句块

end
```
* 定义一个变量在闭区间中遍历，步长为 `step` 后表达式的值


```
for 变量名 iterate 表达式

    语句块

end
```
* 表达式的值必须是一个支持for遍历的容器
* 定义一个变量正序遍历容器

## 控制语句
```
break
```
* 跳出循环


```
continue
```
* 进入下一轮循环


```
return
```
* 结束函数并返回null


```
return 表达式
```
* 结束函数并返回表达式的值
