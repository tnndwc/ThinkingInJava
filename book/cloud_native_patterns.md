# Cloud Native Patterns

> https://book.douban.com/subject/35169075


+ 云原生是高度的分布式和高度的变化（不确定）
+ 面向失败去设计软件
+ 正确处理失败请求的方式：先重试，每次重试之间要保证有时间间隔，同时限定有限的重试次数。重试仍然失败，考虑使用前一次成功的结果缓存返回（当然要考虑场景是否合适这样做），而不是直接返回错误。