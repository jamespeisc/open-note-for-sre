# Kafka

## 深入解析Kafka的offset管理

 https://blog.csdn.net/zjjcchina/article/details/122425951  

## kakfa 控制器节点的作用

https://developer.aliyun.com/article/941171

## kafka 看这一篇就够了

https://zhuanlan.zhihu.com/p/447597155

## 一些note

zk 保存kafka的元数据信息 kafka保存集群偏移量

Kafka 并不支持主写从读

Kafka是通过使用epoch number（纪元编号，也称为隔离令牌）来完成的。epoch number只是单调递增的数字，第一次选出Controller时，epoch number值为1，如果再次选出新的Controller，则epoch number将为2，依次单调递增。
Controller与Zookeeper1，进行交互，获取与更新集群中的元数据信息。主题管理，分区重新分配，leader选举，成员管理
