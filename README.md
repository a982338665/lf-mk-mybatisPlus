# lf-mk-mybatisPlus
Mybatis-Plus（MP）在 MyBatis 的基础上只做增强不做改变，简化开发、提高效率  
介绍MyBatis-Plus的高级功能，包括逻辑删除、自动填充、乐观锁、性能分析、多租户实现、动态表和SQL注入器等内容
>课程地址：https://www.imooc.com/learn/1130
>官方地址：mybatis.plus

## 1.课程介绍及快速入门
### 1.1 课程介绍及学前须知

1.前置技术：
    
    ·lambda表达式
    ·springboot，maven
    ·mybatis    
  
### 1.2 mybatis与JPA对比

1.mybatis与jpa对比：
    
    ·mybatis：
        ·优势：
            -sql语句能自由控制，更灵活，性能较高
            -sql与代码分离，易于阅读维护
            -提供xml标签，支持编写动态sql【if-else等】
        ·劣势：
            -简单的crud操作仍需要写sql
            -xml要维护大量sql
            -mybatis自身功能有限，但支持Plugin
    ·jpa
        ·优势：
            -jpa移植性较好，hql语句，Jpql语句，只需更换数据库驱动便可更换数据库类型
            -提供很多CRUD方法开发效率高，不用写sql
            -面向对象操作，对象化程度更高
            
### 1.3 MP简介-mybatis-plus

1.简介：
    
    ·MP是mybatis的一个增强工具，只做增强，不做改变
    ·2018开源软件排名top10：MP第五【vue，echarts，dubbo，layui，mp，Deepin，Druid，fastjson，RocketMq，ThinkPHP】
    ·CRUD操作在容器启动时注入
    
2.特性：
    
    ·无侵入，损耗小，强大的CRUD操作
    ·支持lambda形式调用，支持多种数据库
    ·支持主键自动生成，支持多种生成策略，支持ActiveRecord模式
    ·支持自定义全局通用操作，支持关键词自动转义
    ·内置代码生成器，内置分页插件，内置性能分析插件
    ·内置全局拦截插件，内置SQl注入剥离器，有效防止sql注入攻击    
    
### 1.4 lombok安装
### 1.5 快速入门
## 2.基本使用
### 2.1 通用传统模式简介 及通用mapper 新增方法
1.ssm传统编程模式：
    
    ·接口中写抽象方法
    ·XML或注解写SQL
    ·Service中调用接口
    ·Controller中调用
      
### 2.2 常用注解

    ·@TableId
    ·@TableFiled
    ·@TableName
    ·@TableField(exist = false)

    
### 2.3 排除非表字段的三种方式
    
    ·transient
    ·static
    ·@TableField(exist = false)
       
## 3.mybatisPlus查询方法
### 3.1 普通查询
### 3.2 条件构造器查询1
    
    ·AbstractWrapper - 条件构造器的类
    
### 3.3 条件构造器查询2
### 3.4 条件构造器查询3
### 3.5 条件构造器查询4
### 3.6 select不列出全部字段
### 3.7 condition作用

    ·用来做模糊查询的判断：
    
### 3.8 实体作为条件构造器构造方法的参数
### 3.9 AllEq用法
### 3.10 其他使用条件构造器的方法
### 3.11 lambda条件构造器
## 4.自定义sql及分页查询

1.自定义sql：

    ·要求版本大于：3.0.7

2.分页：

    ·物理分页插件:
    ·自定义分页
    
## 5.更新及删除

1.更新：

    ·根据id更新
    ·以条件构造器作为参数更新方法
    ·条件构造器中set的使用
    
2.删除：

## 6.AR模式，主键策略和基本配置
### 6.1 AR模式

    ·通过实体类对象直接操作表的增删改查：ActiveRecord
    ·1.实体类实现Model
    ·2.接口集成BaseMapper

### 6.2 主键策略
### 6.3 基本配置
## 7.通用service


