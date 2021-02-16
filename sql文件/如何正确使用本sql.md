- 本sql公开在：https://github.com/FermHan/gulimall
- 参考了视频评论区 特立独行ベ猫 大神的sql：https://github.com/1046762075/mall

个人笔记地址：https://blog.csdn.net/hancoder/article/details/106922139


本sql在其他大神sql的基础上，修正了一些内容。
如前面添加了数据库信息，防止数据库混乱。
还有B站id特立独行的猫 大神里的sql，不过我看他admin库没有弄好(表名大小写有问题)，主要是表名和教程里的发生了冲突，可能他有他自己的使用规则，但是还是用了renren-fast里的。https://github.com/1046762075/mall
另外他里面的库是mall_admin这种形式的，稍加注意即可。还有admin库里他的表名很奇怪，应该是自己改过，我这里上传了renren-fast里的，本人测试可以使用

如何使用:
sql里的数据库都是`mall_admin、mall_ops、...`形式的，而db表都基本没什么区别。
你使用时仅需将你java IDEA里每个项目的application.yml了的库信息改了即可，db表名一般无需改动

另注：

在数据库的 pms_attr 表加上value_type字段，类型为tinyint就行；
在代码中，AttyEntity.java、AttrVo.java中各添加：private Integer valueType，
在AttrDao.xml中添加：《result property="valueType" column="value_type"/》  （把尖括号换成英文的）

