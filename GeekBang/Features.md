# 特征字段构建作业

任务假设：企业违约风险预测
参考网站：https://www.qcc.com/cbase/c70a55cb048c8e4db7bca357a2c113e0

## 基本特征

### 企业基本信息

| Name | Feature Type | Data Type | Remarks |
|--|--|--|--|
|公司名称(id)|Categorical|int|
|经营状态|Categorical|int|续存、注销、倒闭...|
|所属行业|Categorical|int|餐饮、制造、广告...|
|注册资本|numerical|float||
|实缴资本|numerical|float||
|是否上市|Categorical|int||
|所属省|Categorical|int||
|所属省等级|Categorical|int|超一线，一线，二线...|
|所属市|Categorical|int||
|所属市类型|Categorical|int|省会城市、市级、县级...|

### 财务信息

| Name | Feature Type | Data Type | Remarks |
|--|--|--|--|
|财务公开状态|Categorical|int|
|营业收入|numerical|float||
|净利润|numerical|float||
|总资产|numerical|float||
|净资产|numerical|float||
|净利率|numerical|float||
|毛利率|numerical|float||

### 企业经营

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|成立日期|numerical|timeserise||
|人员规模|numerical|int||
|参保人数|numerical|int||
|对外投资数量|numerical|int|
|融资次数|numerical|int||
|融资总金额|numerical|float||

### 资质实力

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|竞品信息数量|numerical|int||
|注册商标数量|numerical|int||
|专利数量|numerical|int||
|资质证书数量|numerical|int||
|作品著作权数量|numerical|int||
|软件著作权数量|numerical|int||

### 法律风险

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|新闻舆情数量|numerical|int||
|涉案案件总数|numerical|int||
|原告案件数量|numerical|int||
|原告案件涉及总金额|numerical|int||
|原告案件涉及金额统计特征|numerical|int|平均、最大、最小、中位、方差...|
|被告案件数量|numerical|int||
|被告案件涉及总金额|numerical|int||
|被告案件涉及金额统计特征|numerical|int|平均、最大、最小、中位、方差...|

## 衍生特征

### 时间维度特征

### 横向对比特征

### 纵向对比特征


### 文本特征

经营范围文本
