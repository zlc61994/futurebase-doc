## 华为云项目管理指引：
 1. 项目创建类型：新建项目类型为“看板”； --项目经理
 2. 创建迭代：按照顺序：V1.0 ，V1.1，V1.2 方式创建，并标注开始和结束时间（日常项可用日期或实际项目名称）（此迭代版本号与tag分支时保持一致）；  --项目组长
 3. 创建需求： 先录入需求工作项，必须指定迭代版本；  -- 产品助理
 4. 创建任务： 在建好的需求下创建子任务，必须增加任务工时，开始时间和结束时间； -- 项目组成员
 5. 测试任务： 与普通任务一样，在需求下创建子任务；  -- 项目组测试人员
 6. 任务开始执行： 更新状态为“执行中”； --项目组开发人员
 7. 任务执行完成： 此时开发人员合并代码到sit，并更新状态为“已解决”，测试人员和产品助理开始介入；--项目组开发人员
 8. 测试任务执行： 更新任务状态“测试中”，同时更新 父需求为“测试中”；-- 项目组测试人员
 9. 测试任务完毕：此父需求下所有用例顺利执行完成，更新此需求下所有任务工作项状态为“关闭”，同时修改需求工作项状态为“测试完毕”； --项目组测试人员
 10. 需求已解决：需求状态为“测试完毕”，由项目组长更新需求项状态为“已解决”； --项目组长
 11. 产品验收：只要有需求标注为“已解决”，产品就开始单项需求验收，验收一项需求后，将需求状态变更为“关闭”；--产品助理
