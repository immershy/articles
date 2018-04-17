

一、 Hbase 和 Cassandra技术选型
    1、 一致性：Hbase注重CP,Cassandra注重AP，Hbase强一致性，Cassandra可调节的一致性
    2、 部署运维： Hbase依赖Zookeeper,Hdfs等组件，Cassandra只有一个tar包
    3、 架构： Hbase通过Master节点读取和写入，Cassandra各个节点对等通过gossip协议交换集群信息
    4、 Hash策略： Cassandra一致性hash(MurmurHash,OrderHash,RandomHash)，对Scan的支持不如Hbase
    5、 易用性： Cassandra 类sql语法，cqlsh
