# Selectsort快速排序
def Selectsort(alist):
    for i in range(len(alist)-1):
        min=i
        for j in range(i+1,len(alist)):
            if alist[j]<alist[min]:
                min=j
        temp=alist[i]
        alist[i]=alist[min]
        alist[min]=temp
    return alist
     
alist=[3,6,8,9,5,4,0,1,2]
print(Selectsort(alist))
        
            
    

