# G5/G9 产品修改记录

- 产品编号：$(@{number=38; product_id=JLZ-EDU-SK-032; chinese_name=错因分析; english_name=Error Cause Analyzer; repository_name=edu-error-cause-analyzer; repository_url=https://github.com/jinlize-tech/edu-error-cause-analyzer; product_type=Skill; category_code=03; category=03 教学教研中心; description=学生错题原因分析。; target_users=System.Object[]; core_input=题目、学生答案、正确答案、步骤、知识点和教师补充观察; main_output=错因分类、错误步骤、知识/方法缺口、验证问题和建议练习; product_risk=把单一错误推断为能力缺陷; dedup_label=存在部分功能交叉; dedup_note=与学情分析区别：聚焦单题/题组错因，不做长期趋势报告。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：错因分析
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：学生错题原因分析。
- 主要风险：把单一错误推断为能力缺陷
- 去重边界：与学情分析区别：聚焦单题/题组错因，不做长期趋势报告。

- 先核对学段、学科、教材版本、课程标准和既有教学资料，防止版本错配。
- 把学习目标、活动、练习、评价和作业建立可追踪对应关系。
- 区分知识、能力、过程方法和素养目标，并按认知层级与难度检查覆盖。
- 对题目、答案、评分标准和教学结论标注来源及人工复核要求。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
