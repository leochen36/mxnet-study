# NDArray 类


## 属性

### NDArray.shape
**描述**    返回一个数组维度的元组,如: 二维二列数组 [[1,2,3],[4,5,6]]  **返回 (2L, 3L)**
### NDArray.size
>    返回数组总长度(几维*几列), 如数组:[[1,2,3],[4,5,6]]  返回长度 6
### NDArray.context
    **返回**执行数组运算的设备容器, 如:默认是cpu第一个核心(如果没有指定context)
### NDArray.dtype
    返回数组元素的类型
### NDArray.stype
    返回存储类型(有kvstore和默认), 在采用分布式运算时,需要使用 kvstore, 否则不需要



## 方法

### NDArray.copy	Makes a copy of this NDArray, keeping the same context.

### NDArray.copyto	Copies the value of this array to another array.

### NDArray.as_in_context	Returns an array on the target device with the same value as this array.

### NDArray.asnumpy	Returns a numpy.ndarray object with value copied from this array.

### NDArray.asscalar	Returns a scalar whose value is copied from this array.

### NDArray.astype	Returns a copy of the array after casting to a specified type.

### NDArray.tostype	Return a copy of the array with chosen storage type.



