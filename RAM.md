* 物理内存（RAM）

  * 使用中（In Use）

    * 压缩（Compreesed）
    * 已修改（Modified）

    > modified写入磁盘后会转换为standby

  * 可用（Available）

    * 空闲（Free）
    * 待机（Standby）（本质就是缓存cache）

  * 硬件保留（Hardware Reserved）

* 分页内存/虚拟内村（ROM-硬盘中的一部分划分为RAM使用）

> 已提交内存(Committed):所有已申请内存的总量, 申请并使用后才会划分到 In Use中
>
> 分页缓冲池\非分页缓冲池

  