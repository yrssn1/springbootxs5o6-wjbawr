# springboot003图书个性化推荐系统的设计与实现

## 简介

本代码仅供学习参考使用

加QQ(**3055269939**)免费获取项目和论文

## 主要内容

### 数据库表设计

将数据库概念设计的E-R图转换为关系数据库。在关系数据库中，数据关系由数据表组成，但是表的结构表现在表的字段上。

表1：tuihuantushu表

| 列名           | 数据类型 | 长度 | 约束         |
| -------------- | -------- | ---- | ------------ |
| id             | bigint   | 200  | NOT NULL     |
| addtime        | varchar  | 200  | NULL DEFAULT |
| tushubianhao   | tinyint  | 200  | NULL DEFAULT |
| tushumingcheng | varchar  | 200  | NOT NULL     |
| zuozhe         | varchar  | 200  | NOT NULL     |
| chubanshe      | varchar  | 200  | NOT NULL     |
| shuliang       | varchar  | 200  | NOT NULL     |
| xuehao         | varchar  | 200  | NOT NULL     |
| tuihuanleixing | varchar  | 200  | NOT NULL     |
| tuihuanyuanyin | varchar  | 200  | NOT NULL     |
| riqi           | varchar  | 200  | NOT NULL     |
| sfsh           | varchar  | 200  | NOT NULL     |
| shhf           | varchar  | 200  | NOT NULL     |

 

表2：tushuxinxi表

| 列名           | 数据类型 | 长度 | 约束     |
| -------------- | -------- | ---- | -------- |
| id             | int      | 200  | NOT NULL |
| addtime        | varchar  | 200  | NOT NULL |
| tushubianhao   | varchar  | 200  | NOT NULL |
| tushumingcheng | varchar  | 200  | NOT NULL |
| tushuleibie    | varchar  | 200  | NOT NULL |
| tupian         | varchar  | 200  | NOT NULL |
| zuozhe         | varchar  | 200  | NOT NULL |
| chubanshe      | varchar  | 200  | NOT NULL |
| shuliang       | varchar  | 200  | NOT NULL |
| xiangqing      | varchar  | 200  | NOT NULL |

 

表3：tushuyuyue表

| 列名             | 数据类型 | 长度 | 约束     |
| ---------------- | -------- | ---- | -------- |
| id               | varchar  | 200  | NOT NULL |
| addtime          | varchar  | 200  | NOT NULL |
| tushubianhao     | varchar  | 200  | NOT NULL |
| tushumingcheng   | varchar  | 200  | NOT NULL |
| tushuleibie      | varchar  | 200  | NOT NULL |
| zuozhe           | varchar  | 200  | NOT NULL |
| chubanshe        | varchar  | 200  | NOT NULL |
| shuliang         | varchar  | 200  | NOT NULL |
| xuehao           | varchar  | 200  | NOT NULL |
| xueshengxingming | varchar  | 200  | NOT NULL |
| lianxidianhua    | varchar  | 200  | NOT NULL |
| shenqingriqi     | varchar  | 200  | NOT NULL |
| sfsh             | varchar  | 200  | NOT NULL |
| shhf             | varchar  | 200  | NOT NULL |

 

表4：xuesheng表

| 列名             | 数据类型 | 长度 | 约束     |
| ---------------- | -------- | ---- | -------- |
| id               | varchar  | 200  | NOT NULL |
| addtime          | varchar  | 200  | NOT NULL |
| xuehao           | varchar  | 200  | NOT NULL |
| mima             | varchar  | 200  | NOT NULL |
| xueshengxingming | varchar  | 200  | NOT NULL |
| xingbie          | varchar  | 200  | NOT NULL |
| chushengriqi     | varchar  | 200  | NOT NULL |
| lianxidianhua    | varchar  | 200  | NOT NULL |
| banji            | varchar  | 200  | NOT NULL |

表5：tushufenlei表

| 列名        | 数据类型 | 长度 | 约束     |
| ----------- | -------- | ---- | -------- |
| id          | varchar  | 200  | NOT NULL |
| addtime     | varchar  | 200  | NOT NULL |
| tushuleibie | varchar  | 200  | NOT NULL |