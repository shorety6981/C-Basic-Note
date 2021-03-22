# array

**动态数组初始化** 	

一维：int* array = new int[n];       
二维：int* array = new int[m][n];       
n:行 m:列       
在[n]后加（）表示默认初始化，即n个元素都为0    
ps:虽然我们分配了一个动态数组，其实返回的是一个T类型的指针，指针指向的是数组的第一个元素     

**释放动态数组** 	

释放动态数组时，使用delete[ ] arr_name；即在数组名前加上一个中括弧      
delete释放数组是逆序进行的，最后一个元素被最先释放，第一个元素最后一个被释放     
申请了内存却没释放，当函数不断地被调用，这些申请过的内存会一直堆积     
```
void delete_fun()
{
	int *arr_test = new int[10];
 
	cout << arr_test << endl;
 
	delete[] arr_test;
}
```

**二维数组的行数与列数表示**	
	
行：  `matrix.size();`			
列:   `matrix[0].size();`		
