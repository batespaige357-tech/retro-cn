# Retro CN

**复盘一次编程会话，找到下次少走弯路的改进。**

基于 [mattpocock/skills 的 retro](https://github.com/mattpocock/skills/tree/main/skills/engineering/retro) 小幅中文适配，独立维护、非官方。

## 保留什么

保留上游按严重程度呈现改进候选的流程：文件导航、自动化检查、编码规范、全局指引、工具开销、无效指令和信息访问。先查看项目实际工具与原始会话，再判断哪里值得调整。

附带上游 writing-for-agents 的写作参考和技能机制说明，免去另装依赖；中文补充强调证据、最小改进与验证方式，防止把一次偶发问题写成长期全局规则。

## 安装与调用

```bash
npx skills add batespaige357-tech/retro-cn --skill retro-cn
```

显式告诉助手：“用 retro-cn 复盘本次编程会话，按严重程度提出改进建议，先不修改环境。”Codex 可使用 `$retro-cn`。本包保留上游显式调用意图，在支持 openai.yaml 的宿主中关闭隐式调用；其他宿主以其调用规则为准。

手动安装复制 `skills/retro-cn` 完整目录，保留 references 和 agents。工具需要能读取用户指定会话与相关项目材料；本包不包含日志采集器，不会安装工具或自动修改全局配置。

## 来源与检查

MIT，保留 Matt Pocock 原版权和完整许可证，详见 [CHANGES.md](CHANGES.md)。

已检查正文保留情况、两份依赖参考、调用策略、UTF-8、本地引用和技能格式。未运行真实复盘或助手行为评估；未读取其他会话日志、修改全局指引或运行前端编译。不含示例网页、效果截图或前后对比。
