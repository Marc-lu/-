# 插入排序

## 直接插入排序  

```c++
template <class T>
void InsertionSort(T Data[], int n) {
    // 利用直接插入排序对于n个数据元素进行升序排序
    int p, i;
    for (p = 1; p < n; ++p) { //p代表插入趟数，共进行n-1趟插入
        T temp = Data[p]; //把待插入元素赋给p
        i = p-1;
        while (i >= 0 && Data[i] >= temp) { // 把比temp大的元素往后移动
            Data[i+1] = Data[i];
            i--;
        }
        Data[i+1] = temp; //i+1为temp的位置
    }
    cout<<"------直接插入排序------"<<endl;
    for (int j = 0; j < n; ++j) {
        cout << Data[j] << '\t';
    }
    cout<<endl;
}
```  

## 折半插入排序
## 希尔排序
# 交换排序
## 冒泡排序
## 快速排序
# 选择排序
## 简单选择排序
## 堆排序
# 归并排序
# 基数排序
# 各种内部排序算法的比较和选择
# 外部排序
## 置换选择排序
## 多路归并排序
