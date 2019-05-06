#### Asg用例图

------

用户交互主要包括搜索旅馆、预定旅馆、购物车操作以及支付，对于这四种交互分别进行用例的完善和关联关系的设计：

1. 搜索旅馆：
   - 输入城市
   - 入住日期
   - 离店日期
   - 搜索结果支持排序，以及如果没有搜索结果则查看推荐
2. 预定旅馆：
   - 选择旅店，选择旅店时可以搜索
   - 选择房型
   - 确定预定，确认预定时需要完善全名和地址两种客户信息
3. 购物车操作：
   - 添加，用户添加购物车时，首先需要完善个人信息
   - 移出
   - 检查
4. 支付：
   - 选择支付账户，选择支付账户可以调用外部接口
   - 填写必要信息

![1557151045341](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557151045341.png)

#### Make reservation 活动图

![2](https://wyxwyx46941930.github.io/2019/04/30/%E7%B3%BB%E7%BB%9F%E5%88%86%E6%9E%90HW7/2.jpg)

### 快递系统

------

#### 泳道图

##### 业务1

整体流程：快递员登录->存放快递->短信平台发送短信->收件人凭短信信息取件

![1557152265800](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557152265800.png)

##### 业务2

整体流程：快递员扫描二维码登录->公司认证身份->快递员扫描单号->存放快递->快递公司发送短信->收件人凭短信信息取件

![1557152811390](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557152811390.png)

##### 业务3

整体流程：快递员扫描二维码登录->公司认证身份->快递员扫描单号->存放快递->判断用户是否关注公众号->(快递公司/公众号)发送短信->收件人凭短信信息取件

![1557153775057](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557153775057.png)

#### 用例图

##### 业务1

![1557153214965](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557153214965.png)

##### 业务2

![1557153475226](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557153475226.png)

##### 业务3

![1557153541871](C:\Users\hp-pc\AppData\Roaming\Typora\typora-user-images\1557153541871.png)
