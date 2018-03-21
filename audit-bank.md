## 网银查询问题:

### 1. 网银信息表中bank_type=[99,98,97]
查询条件: select distinct recv_type from list_bank_acct t where t.recv_acct = '收款账号'
99: 在list_bank_acct 表中找不到记录
98: 在list_bank_acct 表中找到多条记录
97: 其他错误

### 2. 网银信息导入方式:

每个导入操作都会有一个相同的导入批次ID: result_id

#### 2.1 webservice导入
select * from bank_model t where t.origin = '1';


#### 2.2 Excel导入
select * from bank_model t where t.origin = '2';




## 客户名称

1. 马超
2. 杨智慧
3. 何鹏
4. 付仁敬
5.

马超(客户)、杨智慧(客户)、何鹏(客户)、付仁敬(客户)、王宗杰(亚信)、吴海波(亚信)、梅世友(亚信)、田明强(亚信)、叶英生(亚信)、牛刚(亚信)




1. 按时按量完成工作，不拖延工作进度
2. 主动解决客户反馈的问题，修复和开发新功能，并且输出完善的开发文档，保持良好的代码可读性和可扩展性
3. 熟悉经分相关业务知识，并且对现有的系统做优化。
4. 配合项目经理完成项目上线



1. 工作中，能够独立完成上级分配的任务，如果遇到无法解决的问题及时向上反馈，提高了工作效率
2. 业务功能开发时，引导客户达到客户公司双赢的目的
3. 积极完成上级分配的任务，能够主动承担项目组中的重难点任务，并且很到的完成分配的任务
4. 每天严格按照公司的工作时间上下班，项目关键时期，加班通宵，上班时间没有做与工作不相干的时期
5. 主动与上级领导，客户，同事之间沟通，提高工作效率，减少不必要的损失



1. 修复和开发的功能，无故障并且主动协助同事排查解决问题


1. 暂时没有得到客户表扬，接触不到客户。
2. 很少有机会接触客户
3. 遵守需求开发流程、上线流程、维护流程，代码有详细注释，并且提供高可用，高可扩展性。


1. 服从领导工作安排
2. 主动承担责任，不推脱责任
3. 不怕困难，在工作中主动承担重难点任务
4. 务实，不吹嘘弄假
5. 遵守公司的规章制度


2017-11

linux之shell脚本

学习在linux系统下如何编写安全高效的shell脚本，shell脚本在工作中处处可见，简单的几行代码可以帮助我们解决很复杂的问题。





## 问题1

1、尾款预警，营业厅编码在区域选择为全部时不可选填
2、尾款预警，仍选不到和平河西-南京路营业厅（QDA00001）

select DEPART_FRAME, DEPART_CODE, depart_id
  from (select b.depart_code DEPART_FRAME,
               a.depart_code DEPART_CODE,
               B.depart_id
          from td_m_depart a, td_m_depart b
         where a.depart_kind_code in ('100')
           and a.validflag = '0'
           and substr(a.depart_frame, 6, 5) = b.depart_id) t
 where DEPART_FRAME = 'CCB00000';
SELECT * FROM td_m_depart T WHERE T.DEPART_ID = '30191';
SELECT * FROM td_m_depart T WHERE T.DEPART_CODE = 'QDA00001';
SELECT * FROM td_m_depart T WHERE T.DEPART_CODE = 'CCBA0163';














