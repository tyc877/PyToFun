无聊就写写小脚本提高兴趣，继续学习python

^-^
0x01:MysqlHelper.py
用法:
  from MysqlHelper import *
  helper=MysqlHelper('localhost',3306, 'students', 'root','123456')
  ### 多查询
  sql='select name,gender from students order by id desc'
  result=helper.get_all(sql)
  print(result)
  ### 操作数据
  sql2 = "update students set name=%s where id=%s"
  params = ["yes",1]
  conn = helper.update(sql2,params)
  print(conn)
#++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
