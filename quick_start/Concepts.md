# DorisDB基本概念

* FE：FrontEnd DorisDB的前端节点，负责管理元数据，管理客户端连接，进行查询规划，查询调度等工作。
* BE：BackEnd DorisDB的后端节点，负责数据存储，计算执行，以及compaction，副本管理等工作。
* Broker：DorisDB中和外部HDFS/对象存储等外部数据对接的中转服务，辅助提供导入导出功能。
* DorisManager：DorisDB 管理工具，提供DorisDB集群管理、在线查询、故障查询、监控报警的可视化工具。
* Tablet：DorisDB 表的逻辑分片，也是DorisDB中副本管理的基本单位，每个表根据分区和分桶机制被划分成多个Tablet存储在不同BE节点上。
