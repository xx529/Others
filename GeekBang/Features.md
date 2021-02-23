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
|注册资本|Numerical|float||
|实缴资本|Numerical|float||
|是否上市|Categorical|int||
|所属省|Categorical|int||
|所属省等级|Categorical|int|超一线，一线，二线...|
|所属市|Categorical|int||
|所属市类型|Categorical|int|省会城市、市级、县级...|

### 财务信息

| Name | Feature Type | Data Type | Remarks |
|--|--|--|--|
|财务公开状态|Categorical|int|
|营业收入|Numerical|float||
|净利润|Numerical|float||
|总资产|Numerical|float||
|净资产|Numerical|float||
|净利率|Numerical|float||
|毛利率|Numerical|float||

### 企业经营

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|成立日期|Numerical|timeserise||
|人员规模|Numerical|int||
|参保人数|Numerical|int||
|对外投资数量|Numerical|int|
|融资次数|Numerical|int||
|融资总金额|Numerical|float||

### 资质实力

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|竞品信息数量|Numerical|int||
|注册商标数量|Numerical|int||
|专利数量|Numerical|int||
|资质证书数量|Numerical|int||
|作品著作权数量|Numerical|int||
|软件著作权数量|Numerical|int||

### 法律风险

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|新闻舆情数量|Numerical|int||
|涉案案件总数|Numerical|int||
|原告案件数量|Numerical|int||
|原告案件涉及总金额|Numerical|int||
|原告案件涉及金额统计特征|Numerical|int|平均、最大、最小、中位、方差...|
|被告案件数量|Numerical|int||
|被告案件涉及总金额|Numerical|int||
|被告案件涉及金额统计特征|Numerical|int|平均、最大、最小、中位、方差...|

## 衍生特征

### 时间维度对比
|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|营业收入增长|Numerical|float|近1年、近3年、历史平均|
|净利润增长|Numerical|float|近1年、近3年、历史平均|
|总资产增长|Numerical|float|近1年、近3年、历史平均|
|净资产增长|Numerical|float|近1年、近3年、历史平均|
|净利率增长|Numerical|float|近1年、近3年、历史平均|
|毛利率增长|Numerical|float|近1年、近3年、历史平均|
|人员规模增长|Numerical|float|近1年、近3年、历史平均|
|参保人数增长|Numerical|float|近1年、近3年、历史平均|
|对外投资数量增长|Numerical|float|近1年、近3年、历史平均|
|融资次数增长|Numerical|float|近1年、近3年、历史平均|
|融资总金额增长|Numerical|float|近1年、近3年、历史平均|
|竞品信息数量增长|Numerical|float|近1年、近3年、历史平均|
|注册商标数量增长|Numerical|float|近1年、近3年、历史平均|
|专利数量增长|Numerical|float|近1年、近3年、历史平均|
|资质证书数量增长|Numerical|float|近1年、近3年、历史平均|
|作品著作权数量增长|Numerical|float|近1年、近3年、历史平均|
|软件著作权数量增长|Numerical|float|近1年、近3年、历史平均|
|新闻舆情数量增长|Numerical|float|近1年、近3年、历史平均|
|涉案案件总数增长|Numerical|float|近1年、近3年、历史平均|

### 横向对比特征（同规模企业）
规模假设：关于注册资本、人员数量综合指标

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|营业收入与平均对比|Numerical|float|差值、分位数|
|净利润与平均对比|Numerical|float|差值、分位数|
|总资产与平均对比|Numerical|float|差值、分位数|
|净资产与平均对比|Numerical|float|差值、分位数|
|净利率与平均对比|Numerical|float|差值、分位数|
|毛利率与平均对比|Numerical|float|差值、分位数|
|人员规模与平均对比|Numerical|int|差值、分位数|
|参保人数与平均对比|Numerical|int|差值、分位数|
|对外投资数量与平均对比|Numerical|int|差值、分位数|
|融资次数与平均对比|Numerical|int|差值、分位数|
|融资总金额与平均对比|Numerical|float|差值、分位数|
|涉案案件总数与平均对比|Numerical|int|差值、分位数|
|原告案件数量与平均对比|Numerical|int|差值、分位数|
|原告案件涉及总金额与平均对比|Numerical|int|差值、分位数|
|被告案件数量与平均对比|Numerical|int|差值、分位数|
|被告案件涉及总金额与平均对比|Numerical|int|差值、分位数|

### 纵向对比特征（同行业企业）
同行业选主要的一个，特征字段与横向保持一致

|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|营业收入与平均对比|Numerical|float|差值、分位数|
|净利润与平均对比|Numerical|float|差值、分位数|
|总资产与平均对比|Numerical|float|差值、分位数|
|净资产与平均对比|Numerical|float|差值、分位数|
|净利率与平均对比|Numerical|float|差值、分位数|
|毛利率与平均对比|Numerical|float|差值、分位数|
|人员规模与平均对比|Numerical|int|差值、分位数|
|参保人数与平均对比|Numerical|int|差值、分位数|
|对外投资数量与平均对比|Numerical|int|差值、分位数|
|融资次数与平均对比|Numerical|int|差值、分位数|
|融资总金额与平均对比|Numerical|float|差值、分位数|
|涉案案件总数与平均对比|Numerical|int|差值、分位数|
|原告案件数量与平均对比|Numerical|int|差值、分位数|
|原告案件涉及总金额与平均对比|Numerical|int|差值、分位数|
|被告案件数量与平均对比|Numerical|int|差值、分位数|
|被告案件涉及总金额与平均对比|Numerical|int|差值、分位数|

### 文本特征
|Name|Feature Type|Data Type|Remarks|
|--|--|--|--|
|积极新闻舆情案件数量|Numerical|int||
|中性新闻舆情案件数量|Numerical|int||
|消极新闻舆情案件数量|Numerical|int||
|权威媒体发布新闻舆情案件数量|Numerical|int||
|软文发布新闻舆情案件数量|Numerical|int||
|新闻舆情案件权威媒体数量|Numerical|int||
|权威媒体积极新闻舆情案件占比|Numerical|float||
|权威媒体中性新闻舆情案件占比|Numerical|float||
|权威媒体消极新闻舆情案件占比|Numerical|float||
