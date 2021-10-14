2021最新省市区sql/json 文件

**最近更新**：增加了香港、澳门、台湾相关数据~


> 说明：
> 3级联动-包括省、市、区，数据来源[腾讯位置服务（行政区划）API](https://lbs.qq.com/service/webService/webServiceGuide/webServiceDistrict)
> 5级联动-包括省、市、区、街道、社区，数据来源于[国家统计局](http://www.stats.gov.cn/tjsj/tjbz/tjyqhdmhcxhfdm/)，数据比较old



### 目录结构描述
<pre>
├── json                        // json文件目录
│   ├── province.json           // 省
│   ├── city.json               // 市
│   ├── area.json               // 区
│   └── region.json             // 包含所有省市区数据
├── sql                         // mysql文件目录
│   ├── province.sql            // 省
│   ├── city.sql                // 市
│   ├── area.sql                // 区
│   ├── init.sql                // mysql表结构文件, 需要5张表  
│   └── region.sql              // 包含所有省市区数据,只需1张表
├── LICENSE                     // MIT
└── Readme.md                   // help
</pre>

```mysql
# 导入sql时报错时可以尝试以下方式导入
mysql -uroot -p --default-character-set=utf8 dbname < /path/community.sql
```



有问题请提issue，持续更新中.........