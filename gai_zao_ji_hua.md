# 改造计划

对于一期改造，计划从第三方小平台入手。拟定页面包括打印发货，辅助功能和设置部分界面。
###打印发货
核心功能点：

1.用户配置缓存

2.订单缓存
  ```js
  var 订单基本信息
  var subtrades
  var printItems
  var joinedNum
  var unjoinedNum
  +getMerginTradesByOrder()
  -updateAddress()
  +merge()
  +split()   
  ```

3.快递单实体
  ```js
  +print()
  +preview()
  ```
4.发货单实体
  ```js
  +print()
  +preview()
  ```
5.快递公司实体
  ```js
 var expressCompanyMapper
 +getRegExpressionByCompanyCode()
 +getAllExpressCompanys()
 
  ```
6.发货实体
  ```js
  +consign()
  +partConsign()
  ```
###辅助功能
###设置