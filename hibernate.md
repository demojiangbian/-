# -
引入jar开发包
配置相关的XML文件
熟悉API
# -
https://www.cnblogs.com/mq0036/p/8522150.html<br/>
什么是Hibernate框架？<br/>
hibernate是一个ORM（对象关系映射）框架，建立java对象与关系数据库的映射关系，实现java对象的直接存取；<br/>
ORM关注点：对象与数据库列的关系。<br/>
# -
Hibernate对象映射->hbm.xml;hibernate-mapping节点下class节点 类名name与表名table对应；id节点 主键映射 name、column；
property节点 name、column、length、type。<br/>
主配置文件:hibernate.cfg.xml; 配置数据库的信息property，其他参数，加载映射文件 mapping属性resource<br/>
# -
为什么要使用Hibernate？<br/>
# -
hibernate对数据操作 https://www.cnblogs.com/biehongli/p/6528001.html
hibernate增加save(),修改update(),saveOrUpdate();主键查询session.get(User.class, 1)/session.load(User.class, 1);get()与load()的区别？<br/>
HQL查询createQuery，HQL查询与SQL查询的区别？Criteria查询createCriteria();本地查询createSQLQuery()。
