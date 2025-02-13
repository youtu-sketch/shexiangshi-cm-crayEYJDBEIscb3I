[合集 \- 深度学习\&机器学习 操作tips(9\)](https://github.com)[1\.BiLSTM算法（一）2024\-04\-09](https://github.com/jzzg/p/18125147)[2\.BiLSTM算法（二）2024\-04\-10](https://github.com/jzzg/p/18125219)[3\.ResNet50算法2024\-04\-16](https://github.com/jzzg/p/18138375)[4\.《PyTorch深度学习实战》（一）2024\-12\-21](https://github.com/jzzg/p/18621159)[5\.《PyTorch深度学习实战》（二）2024\-12\-26](https://github.com/jzzg/p/18631705)[6\.Python学习（一）——配套《PyTorch深度学习实战》01\-04](https://github.com/jzzg/p/18652015)[7\.Python学习（二）——配套《PyTorch深度学习实战》01\-04](https://github.com/jzzg/p/18652361)[8\.Python学习（三）——配套《PyTorch深度学习实战》01\-05](https://github.com/jzzg/p/18652897)9\.Python学习（四）——配套《PyTorch深度学习实战》01\-05收起
## 1\. Python中字符串的相加和相乘


在Python中，字符串可以通过加号（`+`）进行相加（连接），也可以通过乘号（`*`）进行相乘（重复）。以下是这两种操作的详细说明和示例：


### 字符串的相加（连接）


字符串的相加是通过使用加号（`+`）运算符来实现的。它将两个或多个字符串连接成一个单一的字符串。



```
str1 = "Hello"
str2 = "World"
result = str1 + " " + str2
print(result)  # 输出 "Hello World"

```

在连接多个字符串时，可以连续使用加号：



```
str1 = "Hello"
str2 = "World"
str3 = "Python"
result = str1 + " " + str2 + " " + str3
print(result)  # 输出 "Hello World Python"

```

### 字符串的相乘（重复）


字符串的相乘是通过使用乘号（`*`）运算符来实现的。它将一个字符串重复指定的次数。



```
str1 = "Hello"
result = str1 * 3
print(result)  # 输出 "HelloHelloHello"

```

如果乘以0，结果将是一个空字符串：



```
str1 = "Hello"
result = str1 * 0
print(result)  # 输出 ""

```

### 组合使用


你也可以将字符串的相加和相乘组合使用：



```
str1 = "Hello"
str2 = "World"
result = (str1 + " ") * 2 + str2
print(result)  # 输出 "Hello Hello World"

```

### 注意事项


* 字符串的相加和相乘操作是不可逆的，即结果仍然是一个字符串，而不是一个列表或其他数据结构。
* 在连接大量字符串时，使用`join()`方法通常更高效，因为它避免了创建多个中间字符串对象。
* 字符串的相乘操作要求乘数是一个整数，否则会引发`TypeError`。


通过这些操作，你可以灵活地处理字符串数据，满足不同的编程需求。




---


## 2\. Python中元祖的相加和相乘


在Python中，元组（tuple）也可以通过加号（`+`）进行相加（连接），以及通过乘号（`*`）进行相乘（重复）。以下是对这两种操作的详细说明和示例：


### 元组的相加（连接）


元组的相加是通过使用加号（`+`）运算符来实现的。它将两个或多个元组连接成一个单一的元组。



```
tuple1 = (1, 2, 3)
tuple2 = (4, 5, 6)
result = tuple1 + tuple2
print(result)  # 输出 (1, 2, 3, 4, 5, 6)

```

在连接多个元组时，可以连续使用加号：



```
tuple1 = (1, 2)
tuple2 = (3, 4)
tuple3 = (5, 6)
result = tuple1 + tuple2 + tuple3
print(result)  # 输出 (1, 2, 3, 4, 5, 6)

```

### 元组的相乘（重复）


元组的相乘是通过使用乘号（`*`）运算符来实现的。它将一个元组重复指定的次数。



```
tuple1 = (1, 2, 3)
result = tuple1 * 3
print(result)  # 输出 (1, 2, 3, 1, 2, 3, 1, 2, 3)

```

如果乘以0，结果将是一个空元组：



```
tuple1 = (1, 2, 3)
result = tuple1 * 0
print(result)  # 输出 ()

```

### 组合使用


你也可以将元组的相加和相乘组合使用：



```
tuple1 = (1, 2)
tuple2 = (3, 4)
result = (tuple1 + tuple2) * 2
print(result)  # 输出 (1, 2, 3, 4, 1, 2, 3, 4)

```

### 注意事项


* 元组的相加和相乘操作是不可逆的，即结果仍然是一个元组，而不是其他数据结构。
* 元组的相乘操作要求乘数是一个整数，否则会引发`TypeError`。
* 元组是不可变的，因此相加和相乘操作不会改变原始元组，而是创建一个新的元组。


通过这些操作，你可以灵活地处理元组数据，满足不同的编程需求。




---


## 3\. Python中列表的相加和相乘


是的，Python中的列表（list）也可以通过加号（`+`）进行相加（连接），以及通过乘号（`*`）进行相乘（重复）。以下是对这两种操作的详细说明和示例：


### 列表的相加（连接）


列表的相加是通过使用加号（`+`）运算符来实现的。它将两个或多个列表连接成一个单一的列表。



```
list1 = [1, 2, 3]
list2 = [4, 5, 6]
result = list1 + list2
print(result)  # 输出 [1, 2, 3, 4, 5, 6]

```

在连接多个列表时，可以连续使用加号：



```
list1 = [1, 2]
list2 = [3, 4]
list3 = [5, 6]
result = list1 + list2 + list3
print(result)  # 输出 [1, 2, 3, 4, 5, 6]

```

### 列表的相乘（重复）


列表的相乘是通过使用乘号（`*`）运算符来实现的。它将一个列表重复指定的次数。



```
list1 = [1, 2, 3]
result = list1 * 3
print(result)  # 输出 [1, 2, 3, 1, 2, 3, 1, 2, 3]

```

如果乘以0，结果将是一个空列表：



```
list1 = [1, 2, 3]
result = list1 * 0
print(result)  # 输出 []

```

### 组合使用


你也可以将列表的相加和相乘组合使用：



```
list1 = [1, 2]
list2 = [3, 4]
result = (list1 + list2) * 2
print(result)  # 输出 [1, 2, 3, 4, 1, 2, 3, 4]

```

### 注意事项


* 列表的相加和相乘操作是不可逆的，即结果仍然是一个列表，而不是其他数据结构。
* 列表的相乘操作要求乘数是一个整数，否则会引发`TypeError`。
* 列表是可变的，因此相加和相乘操作不会改变原始列表，而是创建一个新的列表。


通过这些操作，你可以灵活地处理列表数据，满足不同的编程需求。




---


## 4\. Python中的与或非


在Python中，与（AND）、或（OR）和非（NOT）是逻辑运算符，用于组合或修改布尔值（`True`或`False`）。以下是对这些逻辑运算符的详细说明和示例：


### 与（AND）


* **功能**：`and`运算符用于逻辑与运算。当两个操作数都为`True`时，结果为`True`，否则为`False`。
* **示例**：
```
result = True and True  # True
result = True and False  # False
result = False and True  # False
result = False and False  # False

```


### 或（OR）


* **功能**：`or`运算符用于逻辑或运算。当两个操作数中至少有一个为`True`时，结果为`True`，否则为`False`。
* **示例**：
```
result = True or True  # True
result = True or False  # True
result = False or True  # True
result = False or False  # False

```


### 非（NOT）


* **功能**：`not`运算符用于逻辑非运算。它将布尔值取反，即`True`变为`False`，`False`变为`True`。
* **示例**：
```
result = not True  # False
result = not False  # True

```


### 短路求值


Python的逻辑运算符具有短路求值的特性：


* **AND短路**：如果第一个操作数为`False`，则整个表达式的结果必定为`False`，因此不会评估第二个操作数。



```
result = False and some_function()  # 不会调用some_function()

```
* **OR短路**：如果第一个操作数为`True`，则整个表达式的结果必定为`True`，因此不会评估第二个操作数。



```
result = True or some_function()  # 不会调用some_function()

```


### 实际应用


这些逻辑运算符可以用于复杂的条件判断，例如：



```
age = 25
is_student = True

# 判断是否为成年学生
if age >= 18 and is_student:
    print("You are an adult student.")

# 判断是否为未成年或非学生
if age < 18 or not is_student:
    print("You are either a minor or not a student.")

```

通过这些逻辑运算符，你可以构建复杂的逻辑条件来控制程序的流程。




---


## 5\. Python的赋值机制


![赋值机制](https://img2024.cnblogs.com/blog/2760960/202501/2760960-20250105102141999-1993176197.png)
这张图片描述了Python中基本类型（如整数）的赋值机制。在Python中，基本类型是不可变的，这意味着一旦创建，它们的值就不能被改变。图片中的三行代码展示了变量赋值和内存地址的变化过程：


### Step 1


* `a = 100`：创建了一个变量`a`，并将其与值`100`关联。在内存中，`100`被存储在一个位置，我们称之为`pos1(100)`。
* `b = a`：创建了另一个变量`b`，并将`a`的值赋给它。在Python中，这意味着`b`也指向内存中的同一个位置`pos1(100)`。


### Step 2


* `a = 200`：将新的值`200`赋给变量`a`。由于基本类型是不可变的，所以不会修改内存中`pos1(100)`的位置。相反，`a`现在指向内存中的另一个位置`pos2(200)`。而`b`仍然指向原来的`pos1(100)`，因为`b`的值没有被重新赋值。


### Step 3


* 这个步骤强调了可以使用`id()`函数来验证变量的内存地址。`id()`函数返回对象的内存地址，可以用来检查两个变量是否指向同一个对象。


这个过程说明了Python中变量赋值的机制，即变量实际上是对对象的引用。当一个变量被赋值给另一个变量时，它们都指向内存中的同一个对象。如果原始变量被赋予一个新的值，它将指向一个新的对象，而其他变量仍然指向原来的对象。


以下是这个过程的Python代码示例：



```
a = 100  # Step 1: a -> pos1(100)
print(id(a))  # 输出a的内存地址

b = a    # b也指向a的内存地址
print(id(b))  # 输出b的内存地址，应该与a相同

a = 200  # Step 2: a -> pos2(200), b仍然指向pos1(100)
print(id(a))  # 输出a的新内存地址
print(id(b))  # 输出b的内存地址，应该与最初的a相同

```

这段代码将展示`a`和`b`在内存中的地址变化，从而验证了上述的赋值机制。



> 进行联想，这样的赋值机制和在C、C\+\+、Verilog中的有什么区别？


Python的赋值机制与C、C\+\+和Verilog等语言有显著的不同，主要是因为这些语言在处理变量和内存管理方面的方式不同。以下是一些主要的区别：


### 1\. 基本类型和对象引用


* **Python**：Python中的变量总是指向对象的引用。对于基本类型（如整数、浮点数、字符串），Python使用一种称为“对象模型”的机制，其中每个值都是一个对象，变量存储的是对象的引用。这意味着即使两个变量指向同一个对象，修改其中一个变量的值不会影响另一个变量。
* **C/C\+\+**：在C和C\+\+中，基本类型（如`int`、`float`、`char`）直接存储值。变量赋值实际上是值的复制。如果一个变量被赋值给另一个变量，它们各自独立存储自己的值副本。
* **Verilog**：Verilog是一种硬件描述语言，用于设计和模拟数字系统。在Verilog中，变量的赋值可以是阻塞赋值（`=`）或非阻塞赋值（`<=`），这影响赋值的执行顺序和时序。Verilog中的赋值更接近于硬件电路的行为。


### 2\. 可变性


* **Python**：Python中的不可变类型（如整数、浮点数、字符串）一旦创建，其值就不能改变。这意味着任何赋值操作实际上都是创建一个新的对象，并让变量指向这个新对象。
* **C/C\+\+**：C和C\+\+中的变量可以直接修改其值，因为它们存储的是值本身。对于基本类型，赋值操作会直接改变变量的值。
* **Verilog**：Verilog中的变量赋值涉及到信号的更新，这些更新可能在模拟的下一个时间步发生，具体取决于赋值类型（阻塞或非阻塞）。


### 3\. 内存管理


* **Python**：Python自动管理内存，包括垃圾回收。对象的生命周期由引用计数和垃圾回收器共同管理。
* **C/C\+\+**：C和C\+\+要求程序员手动管理内存，包括分配和释放。这提供了更高的灵活性，但也增加了出错的风险。
* **Verilog**：Verilog不涉及传统的内存管理概念，因为它用于描述硬件行为，而不是软件中的内存操作。


### 4\. 赋值语句的执行


* **Python**：赋值语句创建或修改对象引用。如果一个变量被赋值给另一个变量，它们最初指向同一个对象。
* **C/C\+\+**：赋值语句复制值到新的变量。如果一个变量被赋值给另一个变量，它们各自独立存储自己的值副本。
* **Verilog**：赋值语句定义了信号之间的逻辑关系，这些关系在硬件实现中表现为电路连接。


总的来说，Python的赋值机制更侧重于对象的引用和不可变性，而C、C\+\+和Verilog则更侧重于值的直接操作和硬件行为的描述。这些差异反映了不同语言的设计哲学和应用领域。



> 如果更加形象化地解释，如下：


让我们通过一个比喻来形象化地解释Python、C/C\+\+和Verilog中的赋值机制：


### Python：图书馆的图书卡片


想象一下，Python中的变量就像是图书馆里的图书卡片。每张卡片上写着一本书的标题和它在书架上的位置（内存地址）。当你创建一个变量并赋值时，就像你从书架上取出一本书，然后写一张卡片来记录这本书的信息。


* **基本类型赋值**：假设你取出了一本名为“Python编程”的书，你写了一张卡片“a”，上面写着“Python编程”和它的位置。当你把变量`a`赋值给变量`b`时，你只是又写了一张相同的卡片“b”，两张卡片都指向同一本书。如果你在卡片“a”上写下了另一本书的名字“高级Python”，这并不会影响到卡片“b”，因为它仍然指向原来的那本书“Python编程”。在Python中，这意味着`b`的值不会随着`a`的赋值而改变。


### C/C\+\+：图书馆的复印机


在C或C\+\+中，变量就像是图书馆里的复印机。当你创建一个变量并赋值时，就像你复印了一本书的内容，并把复印件给了变量。


* **基本类型赋值**：如果你复印了“Python编程”这本书，并把复印件给了变量`a`，然后你又复印了`a`的内容给了变量`b`，那么`a`和`b`都有了“Python编程”的副本。如果你改变了`a`的副本，比如在上面写下了“高级Python”，这并不会影响到`b`的副本，因为它们是独立的。在C/C\+\+中，这意味着`b`的值不会随着`a`的赋值而改变。


### Verilog：电路板上的连线


Verilog中的赋值更像是电路板上的连线。当你在Verilog中赋值时，你定义了电路板上不同组件之间的连接。


* **赋值**：如果你定义了一个信号`a`连接到一个LED灯，然后你定义了另一个信号`b`也连接到同一个LED灯，那么`a`和`b`都会影响到LED灯的状态。如果你改变了`a`的值，这将直接影响到`b`，因为它们是同一个电路的一部分。在Verilog中，这意味着`b`的值会随着`a`的赋值而改变，这取决于你使用的是阻塞赋值还是非阻塞赋值。


通过这个比喻，我们可以看到Python中的赋值更像是创建指向同一对象的引用，而C/C\+\+中的赋值是创建值的副本，Verilog中的赋值则是定义电路组件之间的逻辑关系。这些不同的赋值机制反映了各自语言的特性和用途。



> 进一步联想，这和面向对象、面相过程的编程的区分有关系吗？


是有关系的，Python、C/C\+\+和Verilog中的赋值机制与面向对象（Object\-Oriented Programming, OOP）和面向过程（Procedure\-Oriented Programming, POP）编程范式有着紧密的联系。这些编程范式影响了语言的设计和赋值机制的实现。让我们看看它们之间的联系：


### 面向对象编程（OOP）


* **Python**：Python是一种多范式语言，支持OOP。在OOP中，数据和函数被封装在对象中，对象通过方法和属性相互交互。Python的赋值机制允许对象（包括基本类型）的引用被复制，而不是对象本身。这与OOP中对象的封装和隐藏原则相吻合，即对象的内部状态不应该被外部直接修改。


### 面向过程编程（POP）


* **C/C\+\+**：C是一种面向过程的语言，而C\+\+支持POP和OOP。在POP中，程序是由一系列操作步骤（过程或函数）组成，数据通过参数在函数间传递。C/C\+\+的赋值机制直接复制值，这与POP中函数间数据传递的方式相似，即函数调用时参数值被复制到函数内部。


### 硬件描述语言（HDL）


* **Verilog**：Verilog是一种硬件描述语言，用于设计和模拟数字电路。它不直接属于OOP或POP范式，但它的赋值机制与硬件电路的行为紧密相关。Verilog中的赋值定义了电路组件之间的连接和信号流动，这与硬件设计中电路的物理连接相似。


### 赋值机制与编程范式的关系


* **封装**：在OOP中，封装是一个核心概念，它意味着对象的内部状态应该被保护起来，不被外部直接访问。Python的赋值机制支持这一点，因为变量赋值操作不会影响到其他指向同一对象的变量，除非使用特定的方法（如修改可变对象的属性）。
* **数据流**：在POP中，数据通过函数调用在程序中流动。C/C\+\+的赋值机制反映了这种数据流，因为变量的值在函数间传递时会被复制。
* **电路行为**：Verilog的赋值机制模拟了硬件电路的行为，其中信号的赋值定义了电路组件之间的连接和数据流动。


总的来说，编程范式影响了语言的赋值机制和数据管理方式。OOP强调对象的封装和交互，POP侧重于函数和过程的调用，而硬件描述语言则模拟电路的物理行为。这些范式在不同语言中的体现，决定了它们如何处理变量赋值和数据管理。



> 更加形象地解释如下：


让我们通过比喻来形象地解释面向对象（OOP）和面向过程（POP）编程的区分，以及这两种编程范式在Python、C、C\+\+中的应用：


### 面向对象编程（OOP）：建筑团队


想象一下，你是一个建筑项目的负责人。在OOP中，每个对象就像是项目中的一个团队成员，他们各自有特定的职责和技能（属性和方法）。


* **Python**：在Python中，OOP非常自然和直观。你可以将每个团队成员（对象）视为一个独立的实体，他们可以互相交流（方法调用）和协作（继承和多态）。例如，一个`House`类可以有`build()`、`paint()`等方法，而`Apartment`类可以继承这些方法并添加特定的功能。


### 面向过程编程（POP）：食谱和烹饪步骤


面向过程编程就像是按照食谱烹饪。食谱中的每个步骤（函数）都是独立的，你需要按照一定的顺序执行这些步骤来完成菜肴。


* **C**：C语言主要是面向过程的。你可以将每个烹饪步骤（函数）视为一个独立的指令，它们按照特定的顺序执行。例如，一个程序可能首先调用`prepare_ingredients()`函数，然后是`cook_meal()`，最后是`serve_dinner()`。
* **C\+\+**：C\+\+支持面向过程和面向对象编程。你可以将C\+\+看作是食谱和建筑团队的结合。你仍然可以按照食谱（POP）的步骤来烹饪，但你也可以创建不同的食材（类）和烹饪工具（对象），它们可以有自己的特性和行为。


### Python、C、C\+\+中的OOP和POP区别


* **Python**：在Python中，OOP是核心特性之一。你可以轻松地定义类和对象，以及它们之间的关系。Python的动态类型系统使得OOP更加灵活和强大。
* **C**：C语言不支持OOP的概念。你不能定义类或对象，只能使用结构体（structs）来模拟一些OOP的特性，如封装。C语言更侧重于过程和函数的调用。
* **C\+\+**：C\+\+是支持OOP的，它引入了类（class）的概念，允许你定义对象和它们的行为。C\+\+也支持继承、多态和封装，这些都是OOP的关键特性。同时，C\+\+也保持了C语言的面向过程特性，允许你使用函数和过程来组织代码。


### 形象比喻


* **OOP**：就像是一个由多个专业团队组成的项目，每个团队（类）都有自己的专长和任务，他们可以独立工作，也可以与其他团队合作完成更大的项目。
* **POP**：就像是一个详细的食谱，每一步（函数）都是独立的，你需要按照食谱的顺序来准备和烹饪食物。


通过这些比喻，我们可以更直观地理解OOP和POP编程范式的区别，以及它们在不同编程语言中的实现和应用。



> 附上另外一个案例


![案例](https://img2024.cnblogs.com/blog/2760960/202501/2760960-20250105105939510-723924482.png)


  * [1\. Python中字符串的相加和相乘](#tid-keZ24J)
* [字符串的相加（连接）](#%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E7%9B%B8%E5%8A%A0%E8%BF%9E%E6%8E%A5)
* [字符串的相乘（重复）](#%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E7%9B%B8%E4%B9%98%E9%87%8D%E5%A4%8D)
* [组合使用](#%E7%BB%84%E5%90%88%E4%BD%BF%E7%94%A8)
* [注意事项](#%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A1%B9)
* [2\. Python中元祖的相加和相乘](#tid-8zQ6sR)
* [元组的相加（连接）](#%E5%85%83%E7%BB%84%E7%9A%84%E7%9B%B8%E5%8A%A0%E8%BF%9E%E6%8E%A5)
* [元组的相乘（重复）](#%E5%85%83%E7%BB%84%E7%9A%84%E7%9B%B8%E4%B9%98%E9%87%8D%E5%A4%8D)
* [组合使用](#%E7%BB%84%E5%90%88%E4%BD%BF%E7%94%A8-1)
* [注意事项](#%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A1%B9-1)
* [3\. Python中列表的相加和相乘](#tid-M8CMkZ)
* [列表的相加（连接）](#%E5%88%97%E8%A1%A8%E7%9A%84%E7%9B%B8%E5%8A%A0%E8%BF%9E%E6%8E%A5)
* [列表的相乘（重复）](#%E5%88%97%E8%A1%A8%E7%9A%84%E7%9B%B8%E4%B9%98%E9%87%8D%E5%A4%8D)
* [组合使用](#%E7%BB%84%E5%90%88%E4%BD%BF%E7%94%A8-2)
* [注意事项](#%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A1%B9-2)
* [4\. Python中的与或非](#tid-YHht7D)
* [与（AND）](#%E4%B8%8Eand)
* [或（OR）](#%E6%88%96or)
* [非（NOT）](#%E9%9D%9Enot):[wgetcloud全球加速服务机场](https://wa7.org)
* [短路求值](#%E7%9F%AD%E8%B7%AF%E6%B1%82%E5%80%BC)
* [实际应用](#%E5%AE%9E%E9%99%85%E5%BA%94%E7%94%A8)
* [5\. Python的赋值机制](#tid-5NGnsK)
* [Step 1](#step-1)
* [Step 2](#step-2)
* [Step 3](#step-3)
* [1\. 基本类型和对象引用](#tid-5W8QDQ)
* [2\. 可变性](#tid-JeRjKa)
* [3\. 内存管理](#tid-QNrsK6)
* [4\. 赋值语句的执行](#tid-bTWGsD)
* [Python：图书馆的图书卡片](#python%E5%9B%BE%E4%B9%A6%E9%A6%86%E7%9A%84%E5%9B%BE%E4%B9%A6%E5%8D%A1%E7%89%87)
* [C/C\+\+：图书馆的复印机](#cc%E5%9B%BE%E4%B9%A6%E9%A6%86%E7%9A%84%E5%A4%8D%E5%8D%B0%E6%9C%BA)
* [Verilog：电路板上的连线](#verilog%E7%94%B5%E8%B7%AF%E6%9D%BF%E4%B8%8A%E7%9A%84%E8%BF%9E%E7%BA%BF)
* [面向对象编程（OOP）](#%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8Boop)
* [面向过程编程（POP）](#%E9%9D%A2%E5%90%91%E8%BF%87%E7%A8%8B%E7%BC%96%E7%A8%8Bpop)
* [硬件描述语言（HDL）](#%E7%A1%AC%E4%BB%B6%E6%8F%8F%E8%BF%B0%E8%AF%AD%E8%A8%80hdl)
* [赋值机制与编程范式的关系](#%E8%B5%8B%E5%80%BC%E6%9C%BA%E5%88%B6%E4%B8%8E%E7%BC%96%E7%A8%8B%E8%8C%83%E5%BC%8F%E7%9A%84%E5%85%B3%E7%B3%BB)
* [面向对象编程（OOP）：建筑团队](#%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%BC%96%E7%A8%8Boop%E5%BB%BA%E7%AD%91%E5%9B%A2%E9%98%9F)
* [面向过程编程（POP）：食谱和烹饪步骤](#%E9%9D%A2%E5%90%91%E8%BF%87%E7%A8%8B%E7%BC%96%E7%A8%8Bpop%E9%A3%9F%E8%B0%B1%E5%92%8C%E7%83%B9%E9%A5%AA%E6%AD%A5%E9%AA%A4)
* [Python、C、C\+\+中的OOP和POP区别](#pythoncc%E4%B8%AD%E7%9A%84oop%E5%92%8Cpop%E5%8C%BA%E5%88%AB)
* [形象比喻](#%E5%BD%A2%E8%B1%A1%E6%AF%94%E5%96%BB)

   ![](https://github.com/cnblogs_com/blogs/735894/galleries/2390289/t_240408075730_155f5951f87fc6702457854e34ef270.png)    - **本文作者：** [江左子固](https://github.com)
 - **本文链接：** [https://github.com/jzzg/p/18653197](https://github.com)
 - **关于博主：** 评论和私信会在第一时间回复。或者[直接私信](https://github.com)我。
 - **版权声明：** 本博客所有文章除特别声明外，均采用 [BY\-NC\-SA](https://github.com "BY-NC-SA") 许可协议。转载请注明出处！
 - **声援博主：** 如果您觉得文章对您有帮助，可以点击文章右下角**【[推荐](javascript:void(0);)】**一下。
     
