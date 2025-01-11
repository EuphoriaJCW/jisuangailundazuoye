# jisuangailundazuoye
学习方法：
  苯人在计概这方面确实是零基础，所以可能一开始一两个月都在系统性地学习语法，尤其是对于列表，字典的一些内置函数的学习，主要方法是哔哩哔哩和一些python的书籍，到了后期开始逐渐接触贪心，dp，dfs和bfs，感觉难度提升很大，个人做的就是把每周的作业看懂，然后去leetcode和晴问上刷一些题，争取做到dp的题尽可能有思路，dfs和bfs的题尽可能少debug（因为是长代码）。
做的题目：
1.判断闰年（http://cs101.openjudge.cn/practice/02733/）
a=int(input())
if a%4!=0:
    print('N')
elif a%3200==0:
    print('N')
elif a%100==0 and a%400!=0:
    print('N')
else:
    print('Y')
2.鸡兔同笼（http://cs101.openjudge.cn/practice/02750/）
a=int(input())
if a%2!=0:
    print('0 0')
elif a%2==0 and a%4!=0:
    b=(a+2)/4
    c=a/2
    print(int(b),int(c))
else:
    b=a/4
    c=a/2
    print(int(b),int(c))
3.Domino piling（http://codeforces.com/problemset/problem/50/A）
M,N=list(map(int,input().split()))
s=M*N//2
print(s)
4.Theatre square（https://codeforces.com/problemset/problem/1/A）
n,m,a=list(map(int,input().split()))
x=(n+a-1)//a
y=(m+a-1)//a
s=x*y
print(s)
5.Petya and strings（http://codeforces.com/problemset/problem/112/A）
string1=input()
string2=input()
string1_=string1.lower()
string2_=string2.lower()
if string1_<string2_:
    print('-1')
elif string1_==string2_:
    print('0')
else:
    print('1')
6.Team（http://codeforces.com/problemset/problem/231/A）
n=int(input())
ls=[]
m=0
for i in range(n):
    ls.append(list(map(int,input().split())))
for each in ls:
    if each[0]+each[1]+each[2]>=2:
        m+=1
    else:
        m+=0
print(m)
7.
