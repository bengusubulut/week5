A = [[{'name':'amnah','old':20},
      {'name':'amina','old':18},
      {'name':'mihail','old':21}],[ 
      {'name':'hira','old':19},
      {'name':'kubra','old':21},
      {'name':'emran','old':22}]
     ,[{'name':'zeynep','old':17},{'name':'ege','old':23}]]

for table in A:
    for student in table:
        if student['name'].startswith('a'):
            pass
        else:
            print(student)

with open("class.txt", "a") as f:
    for i in range(5):
        f.write('ind:'+str(i)+'\n')

f = open("class.txt", 'r', encoding='utf-8')
B = f.read()

print(type(B))
print(B)

x = B.split(':')
print(type(x))
print(x)

for element in x:
    print(element)
    print('---------')
    sep = element.split('{')
    for s in sep:
        print(s)
        print('==========')