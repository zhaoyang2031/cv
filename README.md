<style>
/* 全局字体与基础设置（Markdown PDF 导出时生效） */
@page {
    margin: 18mm 18mm 18mm 18mm;
}
html, body {
    font-family: 'Microsoft YaHei', '微软雅黑', 'SimHei', 'PingFang SC', sans-serif !important;
    font-size: 14px;
    line-height: 1.65;
    color: #1a1a1a;
}
/* 去掉超链接的蓝色下划线，外观变成普通文字 */
a, a:link, a:visited, a:hover, a:active {
    color: inherit !important;
    text-decoration: none !important;
    pointer-events: none !important;
    cursor: default !important;
}
/* 标题样式 */
h1 {
    font-size: 26px;
    text-align: center;
    margin: 10px 0 16px 0;
    color: #111;
    font-weight: 700;
}
h2 {
    font-size: 17px;
    color: #004689;
    margin: 26px 0 8px 0;
    padding-bottom: 4px;
    border-bottom: 1px solid #004689;
    font-weight: 700;
}
/* 分割线 */
hr {
    border: none;
    border-top: 1px solid #d9d9d9;
    margin: 18px 0;
}
/* 联系方式行：灰色小字居中 */
.contact-line {
    text-align: center;
    color: #555;
    font-size: 13px;
    line-height: 1.7;
}
/* 经历标题行：左标题 + 右时间 真正的左右分栏对齐 */
.exp-row {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin: 6px 0 4px 0;
    width: 100%;
    page-break-inside: avoid;
}
.exp-title {
    font-weight: 700;
    font-size: 14.5px;
    color: #151515;
    flex-shrink: 1;
}
.exp-date {
    font-weight: 400;
    font-size: 13px;
    color: #5a5a5a;
    white-space: nowrap;
    margin-left: 16px;
    flex-shrink: 0;
}
/* 没有时间的纯标题经历 */
.exp-row-single {
    margin: 6px 0 4px 0;
    font-weight: 700;
    font-size: 14.5px;
    color: #151515;
}
/* 列表 */
ul {
    margin: 4px 0 12px 0;
    padding-left: 22px;
}
li {
    margin: 3px 0;
    color: #2a2a2a;
}
/* 段落 */
p {
    margin: 4px 0;
    color: #2a2a2a;
}
</style>

# 卢逸扬

<p class="contact-line">18367210405<br>241300037@smail.nju.edu.cn</p>

## 🎓 教育经历

<div class="exp-row">
<div class="exp-title">南京大学 — 人工智能 — 本科</div>
<div class="exp-date">2024.9-2028.6</div>
</div>

gpa 4.46/5 — rk 16/104

主修课程：机器学习、数据结构与算法、python程序设计、C++程序设计

## 🔬 科研经历

<div class="exp-row">
<div class="exp-title">lamda11 | llm as optimizer</div>
<div class="exp-date">2025.9-至今</div>
</div>

- **test-time compute**：利用CoT、self-refine、ReAct、OPRO、BOPRO等思想提高llm as optimizer的能力，本地部署qwen2-7B、qwen3.5-4B模型进行推理

- **llm post-training**：利用SFT、DPO等后训练算法对qwen模型进行微调，针对具体BBO问题使用Forward-Reverse KL捕捉数据的长尾分布等特征

- Agentic BBO**: 近期了解agent在bbo领域的应用，可通过多agent协作提高llm as optimizer的能力

<div class="exp-row">
<div class="exp-title">lamda3 | PyCIL | 持续学习工具包完善及其算法实现</div>
<div class="exp-date">2025.1-2025.8</div>
</div>

- 学习pytorch相关框架及缓解模型灾难性遗忘的典型方法；复现一些经典算法如EWC、IL2A、WA

- 对已有代码设计相应的补充材料，实现说明文档、设计tutorial

## 💼 项目经历

<div class="exp-row-single">华泰证券|面向上市公司的事件驱动智能识别、可信评估与脉络追踪</div>

- 处理30万条excel形式多源高噪声舆情数据集（约1%带标签），进行要素抽取与标准化，实现金融文本的统一理解、事件可信度评估

- 实现同源事件的聚合、事件脉络的追踪与动态预警

<div class="exp-row-single">LLM function calling</div>

- 引入**外部工具调用机制**，增强 LLM 的能力。具体实现豆瓣影评问答、天气查询、股票金融查询和数值计算等功能，提升 LLM 在特定领域的回答精准度，缓解LLM的幻觉问题。

- 实现大模型工具调用框架 ：基于 qwen2.5-turbo Function Calling 构建多轮对话循环，支持多工具并行调用与结果回填

- 与 MySQL 数据库建立连接并执行查询操作，支持基本信息、热门影评、情感分布统计多维度查询

## 🛠 技术能力

- 熟悉c++、python、shell等语言，熟悉linux环境及git、tmux、latex等工具

- 具备llm数据构建、推理优化、评测分析的经验

- 熟悉codex、claude code、cursor等AI编程工具辅助开发并提高工程效率
