# -
优化
# -
1.要什么查什么，避免select*；<br/>
2.不要 ORDER BY RAND()随机取一条数据<br/>
3.一张表设置一个主键，int型，避免使用外键联合做主键<br/>
4.尽可能使用Not Null<br/>
5.查询条件尽量避免模糊查询<br/>
6.使用 TIMESTAMP(4 个字节) 或 DATETIME 类型 (8 个字节) 存储时间；使用String存储占用空间大，不好用时间函数进行比较<br/>
7.避免使用 ENUM 类型； ENUM 类型的 ORDER BY 操作效率低，需要额外操作<br/>
8.禁止使用不含字段列表的 INSERT 语句<br/>
9.拆分复杂的大 SQL 为多个小 SQL<br/>
10.WHERE 从句中禁止对列进行函数转换和计算<br/>
11.在明显不会有重复值时使用 UNION ALL 而不是 UNION<br/>
