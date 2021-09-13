# sstream
<sstream> 定义了三个类：istringstream、ostringstream 和 stringstream，分别用来进行流的输入、输出和输入输出操作。      
<sstream> 主要用来进行数据类型转换，      
  由于 <sstream> 使用 string 对象来代替字符数组（snprintf 方式），避免了缓冲区溢出的危险；      
  而且因为传入参数和目标对象的类型会被自动推导出来，所以不存在错误的格式化符号的问题。     

### stringstream
  1.创建    
  ```stringstream ss;
     string s;
     int n;
  ```
  2.输入
  ```
  cin >> s;
  ```
  3.转换
  ```   
  sstream << s;//字符串放入流中        
  sstream >> n;//从流中抽取字符串，赋给int类型       
  ```
  4.输出
  ```
  cout << n;
  ```
  
  
### 连接字符串
```
  sstream << "sdsd" <<" " <<"df";
  sstream << "sdsjadj";
  
  cout << sstream.str();
```
结果为：sdsd df sdsjadj
