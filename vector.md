# vector 容器——#include< vector >

* 内置函数      
1.创建vector对象，vector<int> vec;         
2.尾部插入数字：vec.push_back(a);          
3.使用下标访问元素，cout<<vec[0]<<endl; 下标是从0开始          
4.使用迭代器访问元素.                  
 ```
 vector<int> it;               
    for(it=vec.begin();it!=vec.end();it++)          
        cout<<*it<<endl;   
 ```
5.插入元素, vec.insert(vec.begin()+i,a);    在第i个元素后面插入a              
6.删除元素, vec.erase(vec.begin()+2);   删除第3个元素              
           vec.erase(vec.begin()+i,vec.end()+j);    删除区间[i,j-1],区间从0开始              
7.vec.begin(),指向第一个元素              
8.vec.end(),表示末端元素的下一个            
9.向量大小:vec.size();            
10.清空:vec.clear()       
