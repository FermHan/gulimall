- 本sql公开在：https://github.com/FermHan/gulimall


本sql在其他大神sql的基础上，修正了一些内容。
如前面添加了数据库信息，防止数据库混乱。
还有B站id特立独行的猫 大神里的sql，不过我看他admin库没有弄好，可能他有他自己的使用规则，但是还是用了renren-fast里的。https://github.com/1046762075/mall
另外他里面的库是mall_admin这种形式的，稍加注意即可。还有admin库里他的表名很奇怪，应该是自己改过，我这里上传了renren-fast里的，本人测试可以使用

如何使用:
sql里的数据库都是`guli_admin、guli_ops、...`形式的，而db表都基本没什么区别。
你使用时仅需将你java IDEA里每个项目的application.yml了的库信息改了即可，db表名一般无需改动

