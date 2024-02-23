# API-operation

# string into list

from calendar import c


my_data='this is one beautiful girl'
my_data=my_data.split()
print(my_data)
my_data.sort()  # list.sort sorts the list in place and return none
print(my_data)

# convert between types
changed_string=str(100)
print(type(changed_string))

changed_int=int('100')
print(changed_int)

changed_float=float('3.14159')
print(type(changed_float))

# count the len of name in list and consist of one list
import time

classmate_list=['nina','joey','kevin','petra','tommy']
name_len=[]
start_time=time.time()
for name in classmate_list:
    name_len.append(len(name))
end_time=time.time()    
print(name_len)
print(end_time-start_time)



# lsit comprehensive
import time

classmate_name=['nina','joey','kevin','petra','tommy']
start_time= time.time()
name_len=[len(name) for name in classmate_name]
end_time= time.time()
print(end_time-start_time)

name_len=[('length',len(name)) for name in classmate_name]
print(name_len)


classmate_name=['nina','joey','kevin','petra','tommy']
name_len=[len(name) for name in classmate_name if len(name)% 2==0]   #conditions
print(name_len)


number_list=[1,2,3,4,5,6]
','.join([str(num) for num in number_list])
print(number_list)
number_list[0]=str(number_list[0])
print(type(number_list[0]))
print(type(number_list[1]))
print(type(number_list))
print(type(str(number_list[0])))

