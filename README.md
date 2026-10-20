# 高性价比体检筛查指南

## 在线阅读

- 在线阅读页：https://kexin1409.github.io/how-to-check-better/ （单文件零依赖，手机/断网可读，可搜索、可按性价比/证据等级/风险筛选）
- PDF 下载（国内直连）：https://kexin1409.github.io/how-to-check-better/how-to-check-better.pdf
- 仓库：https://github.com/kexin1409/how-to-check-better

循「高性价比」系列第八本。前七本（[饮食](https://github.com/kexin1409/how-to-eat-better)、[睡眠](https://github.com/kexin1409/how-to-sleep-better)、[运动](https://github.com/kexin1409/how-to-exercise-better)、[搞钱](https://github.com/kexin1409/how-to-earn-better)、[投资](https://github.com/kexin1409/how-to-invest-better)、[避坑](https://github.com/kexin1409/how-to-decide-better)、[养老](https://github.com/kexin1409/how-to-retire-better)）之后，这本把镜头转向**体检与筛查**——不是教你买更贵的套餐，而是分清哪些检查真能降低死亡率、哪些只是花钱买焦虑。

## 核心来源与口径

- **中国口径**：国家癌症中心《6 种主要癌症筛查方法》（肺癌、胃癌、食管癌、结直肠癌、乳腺癌、宫颈癌的高危人群界定、筛查手段与间隔）https://literature.chinacdc.cn/xuekefuwu/gonggongweishengxueshuredianzhuiz/202205/t20220517_259261.html
- **国际分级**：USPSTF《Adult Preventive Health Care Schedule》（2024-05-09）A/B/C/D/I 分级建议 https://www.aafp.org/assets/image/upload/v1780508286/USPSTFHealthCareSchedule2024.pdf
- **反面证据**：PLCO 等大型筛查试验——卵巢癌 CA125+超声（约 78,216 人、6 年）未降低死亡率；前列腺癌 PSA（76,693 人、7 年）获益不显著
- **过度诊断**：甲状腺癌、前列腺癌、卵巢癌的过度诊断与主动监测证据
- **诚实说明**：本书只讲"无症状人群的筛查"，不讲已出现症状的就医与诊断。有症状请直接就诊，不要用体检代替看病。

## 内容规模

12 节 **144 条**：
- 证据等级分布见在线页筛选
- 卡片沿用系列「成本 × 收益 × 证据 × 性价比 × 风险」框架，风险字段标注"据此操作可能付出什么代价"
- 外链 2 条，均为上述原始文献（国家癌症中心、USPSTF）

## 12 节结构

1. 体检的底层逻辑，什么才叫有效筛查（筛查≠诊断、领先时间偏倚、过度诊断、假阳性概率）
2. 体检前的准备，别让结果白查（空腹、经期、停药、肠道准备、标本采集）
3. 最值钱的四个基础指标（血压、血糖、血脂、体重腰围）
4. 血尿便常规和肝肾功能，怎么读不慌（参考区间、脂肪肝、Hp、甲功）
5. 肿瘤标志物，最贵也最容易被误用（为什么指南不推荐筛查）
6. 真正能降低死亡率的影像与内镜（LDCT、钼靶、胃肠镜、FIT、骨密度）
7. 六大癌症逐个说：肺、胃、食管、结直肠、乳腺、宫颈（含中美口径差异）
8. 不推荐普筛的四种，过度诊断重灾区（甲状腺、前列腺、卵巢、胰腺；肝癌只查高危）
9. 心脑血管检查，哪些有用哪些是安慰（风险评估优先于找斑块）
10. 高端体检和基因检测，智商税清单（PET-CT、全身核磁、一滴血查癌、天赋基因）
11. 报告怎么读，别被箭头牵着走（动态变化、结节分级、何时直接就医）
12. 避坑清单：体检中心最常见的 12 个坑

## 交付物

- `index.html` — 单文件零依赖阅读页（搜索、按性价比/证据等级/风险/成本筛选、章节跳转、明暗主题）
- `how-to-check-better.pdf` — PDF（封面 + 目录 + 前言 + 12 节正文，带书签）
- `book/*.md` — 12 节正文源文件
- `build.py` / `make_pdf.py` / `tools/test_page.js` — 构建与回归脚本

## 构建

```bash
python build.py -o index.html      # 生成单文件阅读页
python make_pdf.py -o how-to-check-better.pdf   # 生成 PDF（需 reportlab + 中文字体）
```

## 声明

本书整理自国家癌症中心筛查方法、USPSTF 分级建议与公开研究。具体筛查方案以国家卫健委、国家癌症中心等官方发布及你的主诊医生意见为准，所有结论都注明出处，**不构成任何医疗建议**；书里的内容可能过时，也可能有错，是否筛查请与医生共同决定。发现写错了欢迎提 issue。

许可证：内容 CC BY 4.0；代码见 LICENSE / LICENSE-CODE。
