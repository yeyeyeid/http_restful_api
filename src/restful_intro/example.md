# RESTful API常见形式举例

下面找些常见的RESTful的API供参考和有个直观的概念：

## RESTful的订单的API

```
==========  =====================  ==================================
HTTP 方法    行为                   示例
==========  =====================  ==================================
GET         获取资源的信息           http://example.com/api/orders
GET         获取某个特定资源的信息    http://example.com/api/orders/123
POST        创建新资源              http://example.com/api/orders
PUT         更新资源                http://example.com/api/orders/123
DELETE      删除资源                http://example.com/api/orders/123
==========  ====================== ==================================
```

## RESTful的客户的API

```
POST http://www.example.com/customers
POST http://www.example.com/customers/12345/orders

GET http://www.example.com/customers/12345
GET http://www.example.com/customers/12345/orders
GET http://www.example.com/buckets/sample

PUT http://www.example.com/customers/12345
PUT http://www.example.com/customers/12345/orders/98765
PUT http://www.example.com/buckets/secret_stuff

DELETE http://www.example.com/customers/12345
DELETE http://www.example.com/customers/12345/orders
DELETE http://www.example.com/bucket/sample
```

## RESTful的待办事项TodoList的API

```
==========  ===============================================  =============
HTTP 方法   URL                                              动作
==========  ===============================================  =============
GET         http://[hostname]/todo/api/v1.0/tasks            检索任务列表
GET         http://[hostname]/todo/api/v1.0/tasks/[task_id]  检索某个任务
POST        http://[hostname]/todo/api/v1.0/tasks            创建新任务
PUT         http://[hostname]/todo/api/v1.0/tasks/[task_id]  更新任务
DELETE      http://[hostname]/todo/api/v1.0/tasks/[task_id]  删除任务
==========  ================================================ =============
```

更多细节详见：**【整理】TodoList待办事项：常被用于解释一个概念和框架如何应用）**


