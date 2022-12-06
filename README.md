# reposiotory 
math
from datetime import *
name=input('enter your name: ')
def bill_cal():
a=True
total_price=0
list_item_price=[]
while a:
print('''
1.list of item
2.choose item
3.exit
''')
choice=int(input('enter your choice:'))
choices=[1,2,3]
if choice in choices:
d={'dal':65,'oil':70,'mirchi':45,'paste':20,'shampoo':50,'milk':25,'chocolate':20,'water
bottle':20,'juice':40,'cake':70,'fruits':50,'biscuits':78,}
if choice in choices:
c=1
for i,j in d.items():
print('\t',c,'.',i,',$',j)
c+=1
if choice ==2:
q=True
while q:
print("press 'q' to see main menu.")
item=input('enter item:')
if item in d.keys():
qnt = input('enter quantity:')
if qnt.isdigit():
qnt=int(qnt)
price=float(d[item]*qnt)
list_item_price.append((item,qnt,price))
total_price+=price
else:
print('invalid input quantity..')
elif item =='q':
q=False
else:
print('item not present.')
if choice == 3:
a=False
