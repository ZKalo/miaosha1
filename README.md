# miaosha1
初级秒杀项目，秒杀项目的基本构建，还没有处理高并发和优化性能


技术：Springboot + JPA + MySQL + Mybatis + bootstrap + JQuery

项目大致分三部分：
  【1】用户注册与登录
  【2】商品显示与详情
  【3】秒杀活动与下单
  
项目注意点：
  1）Springboot JPA的使用，最注意的一点是更新操作要使用@Query注解
  2）返回用户信息使用JWT的token技术
  3）商品分有秒杀活动和没有秒杀活动的商品，注意两者下单时的价格不一样
  4）商品的秒杀活动是否有效和个数问题，目前版本只取有效中的第一个
  
项目缺点：
  ①、没有考虑高并发和性能优化问题，也就是没有使用redis，消息队列等
  ②、整个流程没有太严谨，也就是没有太多的验证操作
