# 用户登陆demo

## 用户登陆流程

1. 用户填写用户名密码，提交到LoginServlet
2. 在LoginServlet中使用Mybatis查询数据库，验证用户名密码是否正确
3. 如果正确，响应“登陆成功”，如果错误，响应“登陆失败”

## 用户注册流程

1. 用户填写用户名、密码等信息，点击注册按钮，提交到RegisterServlet
2. 在RegisterServlet中使用MyBatis保存数据
3. 保存前，需要判断用户名是否已经存在：根据用户名查询数据库，如果用户名已存在，不保存；用户名不存在则保存