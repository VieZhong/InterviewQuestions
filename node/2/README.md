# 请介绍一下 require 的模块加载机制

1. 计算模块绝对路径；
2. 如果缓存中有该模块，则从缓存中取出该模块；
3. 按优先级依次寻找并编译执行模块，将模块推入缓存（require.cache）中；
4. 输出模块的 `exports` 属性；