# 代码质量竞赛

为了提高大家的编码水平,代码质量,从而提高产品的质量,交付优质的产品。决定以后每周五举行一次code review.
以积分制形式进行.每个月计算一次总分.

## 1、奖惩制度
最高得分者会有奖励(带薪假期1天),最低得分者也有惩罚(乐捐100团建费)。
在新公司成立时,连续积分在倒数前2的,下份合同签署的时候不涨薪。外包不续签.

## 2、积分说明

每次review积分总分为一百分,有不符合要求的进行扣分.扣分标准如下:

#### 2.1、后端

1. 日志不规范的扣5分(如直接e.printStackTrace()/捕获后不做任何操作/无意义的日志输出等)[java规范-3.日志打印](java/规范/java规范.md)
1. 循环调用接口的扣5分
1. 后台因为报错而将敏感信息传递到前端的扣4分.
1. maven依赖不规范的扣3分
1. 在api模块使用entity,依赖了devtools的扣2两分
1. 使用map或entity接收返回参数的扣2分
1. 应通过线程池进行线程操作，禁止在代码中直接new一个线程操作，否则扣2分 [java规范-5.多线程](java/规范/java规范.md)
1. 出现硬编码的扣1分[java规范-6.常量定义](java/规范/java规范.md)
1. 规范中其他明确禁止的扣2分
1. 不允许使用restTemplate之外的工具请求中台服务.也不允许自己new.否则扣1分(因为base提供的restTemplate做了埋点)

#### 2.2、前端

1. 代码需要完全符合eslint规范，包括但不仅限于缩进、引号等，不应出现eslint error级别提示。否则扣4分。
1. 项目图片需要压缩处理，否则扣3分。
1. 文件名大小写不规范，扣2分。 

> 目前列出的都是非常紧要的问题,随着review的进行后面会陆续增加扣分标准,前后端分开计分

## 3、review范围

1. review的代码为新版本的代码,以前的老代码允许有1个季度的时间来重构(一个季度后会review).
2. 每次review进行两小时,分别对聚合服务,中台服务(前端的单独进行)代码进行review.

## 4、积分记录及异议处理

1. 每次review结束后会当场公布积分,有异议可以当场提出,提出的异议在场的人超过50%同意的可以更改.结束后原则上不接受任何异议。
2. 积分会在结束后统一记录在华为云viki上.地址到时会公布在群里
  ​                                                                                                                      