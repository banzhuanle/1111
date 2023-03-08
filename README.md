该项目为《恶意挖矿流量快速检测框架的设计与实践》一文所创建收集的挖矿流量和经MMTRDF框架挖矿流量所处理后的特征数据集。
上传的mining.csv文件为经过MMTRDF框架处理后的挖矿流量特征数据集，可直接导入机器学习模型进行训练，主要是关于以太坊的挖矿流量（包括加密与IPV6），为了避免内网ip的泄露，故ip地址匿去。（挖矿连接在真实网络环境中属于老鼠流，stratum通信协议所产生的通信流量相比其他tcp长链接类型也较少，同时设置了10分钟的时间窗口进行聚合，因此导出的特征数据集也较小。）
csv文件中每行为不同连接一个时间窗口内聚合的具体数据，列为不同的特征名称，其中duration代表一个时间窗口设置为10分钟，flow代表一条连接。其余为具体的流量特征信息名称。
其余包括门罗币等其他货币类型的特征数据集和原始pcap包将于近期上传，并按名称进行具体的分类。
