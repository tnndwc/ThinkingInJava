# 虚拟内存

> 一种内存管理技术

> 内核才会真正的操作物理内存

### 为什么需要虚拟内存

+ 使得应用程序拥有连续对地址空间（⚠️ `连续的`地址空间）

+ 可以借助磁盘来扩展应用程序的“内存容量”，比如，可以把某些不活跃程序的虚拟地址空间的内存换入到磁盘上存储