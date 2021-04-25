基礎輸出
print('Hello, world!')
print('ábsurd')

進制改變
int('8', 16)

S = 16

print(S)

位元組 (bytes)
實際儲存的數值
mybytes = b'hello'
print(mybytes)
print(mybytes.hex())
print(bytes.fromhex('68616861'))

字串與位元組轉換
astring = "哈哈"
print(astring)
abytes = astring.encode("utf8")
print(abytes)
astring = abytes.decode("utf8")
print(astring)

列表
mylist = []

mylist.append(1)
mylist.append(2.8)
mylist.append("haha")

print(mylist[0])
print(mylist[1])
print(mylist[2])

for x in mylist:
    print(x)

字串相關函式
chr(66)
chr(114)
chr(101)

a=[66,114,101,97,107,65,76,76,67,84,70,123,65,109,118,48,117,68,121,101,114,118,80,116,109,86,114,57,83,83,83,75,125]

for i in a:
  print(chr(i),end = "")

算術運算子
number = 1 + 2 * 3 / 4.0
print(number)

remainder = 11 % 3
print(remainder)

squared = 7 ** 2
cubed = 2 ** 3
print(squared)
print(cubed)

字串運算子
ss = "hello" + " " + "world"
print(ss)

lotsofhellos = "hello" * 10
print(lotsofhellos)

列表運算子
even_numbers = [2,4,6,8]
odd_numbers = [1,3,5,7]
all_numbers = odd_numbers + even_numbers
print(all_numbers)

print([1,2,3] * 3)

字串位置
astring = "Hello world!"
print(astring.index("o"))

astring = "Hello world!"

子字串,倒敘
print(astring[3:7])
print(astring[3:7:2])
print(astring[::-1])
判斷是否對稱
qw = ("sEs")
print(qw == qw[::-1])

字串前後綴判斷
astring = "Hello world!"
print(astring.startswith("Hello"))
print(astring.endswith("asdfasdfasdf"))

字串切割
astring = "Hello world!"
q = astring.split("w")
print(q)

astring = "66 114 101 97 107 65 76 76 67 84 70 123 65 109 118 48 117 68 121 101 114 118 80 116 109 86 114 57 83 83 83 75 125!"
yu = astring.split(" ")
print(yu)

is 運算子
判斷是否為相同實例
不同源
x = [1,2,3]   
y = [1,2,3]   
print(x == y) 
print(x is y) 
同源
z = [1,2,3]   
a = z   
print(a == z) 
print(a is z)

while 迴圈
count = 0
while count < 5:
    print(count)
    count += 1  # This is the same as count = count + 1

for 迴圈
primes = [2, 3, 5, 7]
for prime in primes:
    print(prime)

for x in range(5):
    print(x)

for x in range(3, 6):
    print(x)

for x in range(3, 8, 2):
    print(x)

套件使用
import random

print(random.randint(0, 100))

異常處理
try:
    print(我抽得到Es嗎)
except:
    print("做夢")

列表操作
sentence = "the quick brown fox jumps over the lazy dog"
words = sentence.split()
word_lengths = []
for word in words:
      if word != "the":
          word_lengths.append(len(word))
print(words)
print(word_lengths)

列表生成(前者簡化版
sentence = "the quick brown fox jumps over the lazy dog"
words = sentence.split()
word_lengths = [len(word) for word in words if word != "the"]
print(words)
print(word_lengths)
