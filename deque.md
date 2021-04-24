# deque ---double queue 双端队列

### 基本函数
1.创建队列          

deque<int> d;    
  
2.插入元素        

front()     //队首元素                      
back()      //队尾元素        
push_back()   //在队尾                                 
push_front()   //在队首                                          
insert(d.begin()+1,x);   //第一个元素之后插入x                                    
  
3.容量                                                  

size()   //双端队列的大小          
empty()   //判断是否为空        
  
4.正向，反向指针           

begin()   //队首的指针，指向队首元素        
end()   //队尾元素的下一位作为指针        

rbegin()  //以最后一个元素作为开始       
rend()   //以第一个元素的上一位作为指针      

5.删除                      

erase(deque.begin(),deque.begin()+5)   //删除某一个/段元素        
clear()   //删除所有元素        
pop_front()   //删除队首元素        
pop_back()   //删除队尾元素         

deque<int>::iterator it;   //迭代器          
deque<int>::reverse_iterator rit;   //反向迭代器             


### 正向迭代器
```
deque<int>::iterator trit;
    for(trit = deque.begin(); trit != deque.end(); trit ++)
        cout<<*trit<<" ";
    cout<<endl;
```

### 反向迭代器
```
deque<int>::reverse_iterator revit;
for(revit = d.rbegin(); revit != d.rend(); revit ++)
    cout<<*revit<<" ";
cout<<endl;
```
