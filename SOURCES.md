# 来源与改写说明

“嘉伟漫剧分镜提示词”是按嘉伟的制作需求合并、重新组织的独立 Skill，不是上游的官方版本，也不依赖上游安装。

## 参考来源

1. [eternityspring/shuohao-skills](https://github.com/eternityspring/shuohao-skills)，固定版本 `c27ea0e49c009a2b3c43dec40b702597ab56e1d9`。参考 novel-storyboard 的剧情节拍、段／镜／关键帧区分、对白容量、图片与动态正文分工、参考素材职责。Apache-2.0；原通知保留在 [licenses/shuohao-NOTICE.txt](licenses/shuohao-NOTICE.txt)，许可正文在 [LICENSE](LICENSE)。
2. [Emily2040/seedance-2.0](https://github.com/Emily2040/seedance-2.0)，固定版本 `4668457e560eee06e95d7fcfdf441c8c0bba802e`。参考 seedance-prompt、seedance-sequence、shot-table、directors-read 的空间调度、可见表演、参考职责、计划与实际状态区分、跨段续接。原 MIT 许可和版权保留在 [licenses/emily-MIT.txt](licenses/emily-MIT.txt)。

## 本地改写（2026-10-11，v1.0.0）

- 合并重复的人物一致性、动作、对白、空间、声音及质量检查规则，改成中文制作流程。
- 移除原项目 JSON、代码、外部 Skill 与文件树前提，纯文本可用。
- 去掉固定 15 秒、固定切数、每切 2–5 秒、每集必须运动开场等硬门，改为按剧情、对白与平台能力选择。
- 统一“整集规划可一次交付”与“实际续接按成片修正”，不让续接门槛阻断完整拆镜。
- 不继承上游对合法剧情词汇的一刀切删除／替换规则，也不静默重写剧本。
- 不把仓库作者的模型参数、英文偏好、最多续接次数或协议写法当作平台通用事实。
- 加入嘉伟 3:4 人物卡的参考使用边界：不把资产卡排版、人物名字或多视图复制进单帧视频。
- 保留局部修改范围，控制提示词长度，不把内部分镜推理塞入生产提示词。

本包新编文本采用 Apache-2.0；上游原始通知及各自许可仍有效。随包保留来源和许可，不能宣称这些被借鉴的方法均为独创。
