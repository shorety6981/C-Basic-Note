# vector 容器——#include< vector >

* 内置函数      
1.创建vector对象，`vector<int> vec; `   
2.创建并初始化vector对象 `vector<int> vec(n,1)`  vec数组中n个位置，每个位置数值为1                         
3.尾部插入数字：`vec.push_back(a); `         
4.使用下标访问元素，`cout<<vec[0]<<endl; `下标是从0开始          
5.使用迭代器访问元素.                  
 ```
 vector<int> it;               
    for(it=vec.begin();it!=vec.end();it++)          
        cout<<*it<<endl;   
 ```
5.插入元素, `vec.insert(vec.begin()+i,a);  `  在第i个元素后面插入a              
6.删除元素, `vec.erase(vec.begin()+2); `  删除第3个元素              
           `vec.erase(vec.begin()+i,vec.end()+j); `   删除区间[i,j-1],区间从0开始              
7.`vec.begin()`,指向第一个元素              
8.`vec.end()`,表示末端元素的下一个            
9.向量大小:`vec.size();  `          
10.清空:`vec.clear() `   

* 容器中的排序函数与其他情况不同      
`sort(vec.begin(),vec.end());`  //默认从小到大    
* 建立动态数组时，加入值要用函数   
` vec.push_back(i);`  
* 随着循环初始化的时候也刷新了，不用刻意清空    


# 细节
* vector<string> s;
s[0][0]：第一个字符串的首字母   
