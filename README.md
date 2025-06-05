class GameData:

#Print game information
def print_info(self):
print(f"{self.name} {self.version} {self.author} {self.description}")

#Change game name
def set_name(self, name):
self.name = name

#Change author name
def set_author(self, author):
self.author = author

#Modify version number
def set_version(self, version):
self.version = version

#Modify description information
def set_description(self, description):
self.description = description

#Retrieve game information and return a list
def get_info(self):
return [self.name, self.author, self.version, self.description]

class StorageSpace

#Add data to storage space
def add_data(self, data):
self.data.append(data)
self.Count += 1

#Get all data
def get_data(self):
return self.data

#Get the current number of data
def get_count(self):
return self.Count

#Retrieve data from the specified index location
def DataCount(self, Count):
return self.data[Count]

#Print all data (formatted as | content |)
def list(self):
for i in range(self.Count):
print("|" + self.DataCount(i), end="")
print("|")

#Delete data at the specified index location
def delete(self, Count):
self.data.pop(Count)
self.Count -= 1

#Clear all data
def delete_all(self):
self.data.clear()
self.Count = 0

#Count data items before printing
def ListUntilCount(self, Count):
for i in range(Count):
print("|" + self.DataCount(i), end="")
print("|")

#Print data items at the specified index location
def ListCount(self, Count):
print("|" + self.DataCount(Count) + "|")

Method/Function：

def square(number):
Return number * number # square operation

def cube(number):
Return number * number * number # Cube operation

def square_root(number):
Return number * * (1/2) # square root

def cube_root(number):
Return number * * (1/3) # Root opening square

def stick(number1, number2) -> int:
Return int (str (number 1)+str (number 2)) # Concatenate two numbers into an integer output

### 中文


# 定义一个用于存储游戏信息的类
class GameData:
    # 初始化方法，设置游戏的基本信息
    def __init__(self, name, author, version, description):
        self.name = name
        self.author = author
        self.version = version
        self.description = description

    # 打印游戏信息
    def print_info(self):
        print(f"{self.name} {self.version} {self.author} {self.description}")

    # 修改游戏名称
    def set_name(self, name):
        self.name = name

    # 修改作者名
    def set_author(self, author):
        self.author = author

    # 修改版本号
    def set_version(self, version):
        self.version = version

    # 修改描述信息
    def set_description(self, description):
        self.description = description

    # 获取游戏信息，返回一个列表
    def get_info(self):
        return [self.name, self.author, self.version, self.description]


# 定义一个用于管理数据存储的类
class StorageSpace:
    # 初始化为空的数据列表和计数器
    def __init__(self):
        self.Count = 0
        self.data = []

    # 添加数据到存储空间
    def add_data(self, data):
        self.data.append(data)
        self.Count += 1

    # 获取所有数据
    def get_data(self):
        return self.data

    # 获取当前数据个数
    def get_count(self):
        return self.Count

    # 获取指定索引位置的数据
    def DataCount(self, Count):
        return self.data[Count]

    # 打印所有数据（格式化为 |内容| 的形式）
    def list(self):
        for i in range(self.Count):
            print("|" + self.DataCount(i), end="")
        print("|")

    # 删除指定索引位置的数据
    def delete(self, Count):
        self.data.pop(Count)
        self.Count -= 1

    # 清空所有数据
    def delete_all(self):
        self.data.clear()
        self.Count = 0

    # 打印前 Count 个数据项
    def ListUntilCount(self, Count):
        for i in range(Count):
            print("|" + self.DataCount(i), end="")
        print("|")

    # 打印指定索引位置的数据项
    def ListCount(self, Count):
        print("|" + self.DataCount(Count) + "|")
