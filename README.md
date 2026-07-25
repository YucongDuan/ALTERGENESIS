# ALTERGENESIS · 异生

**多认知世界生成与超个体判断引擎**  
*Plural Worldmaking & Transindividual Judgment Engine*

![ALTERGENESIS Studio](docs/images/ALTERGENESIS_Studio_CN.png)

ALTERGENESIS 不在一个预先给定的世界里优化答案。它让不同的认知世界被显式生成，让它们在相遇时彼此改变而不被合并，并只在一个判断确实超出任何单一来源的能力时，将其标记为“超个体判断”。

它不是多智能体投票器，也不是意见摘要器。

```text
片段与位置
    ↓
生成多个认知世界
    ↓
世界 A ↘ 世界 B      世界 B ↘ 世界 A
双方改变，差异仍保留
    ↓
未知作为生成压力，而非待填空白
    ↓
规则自身成为认知对象
    ↓
跨世界行动组合 + 反事实移除
    ↓
无人单独拥有的判断事件
    ↓
闭合产生新世界入口，而非终点
```

## 现在能运行什么

- 五类世界生成算子：关系先行、观察者去中心、未知先行、深时、规则显形。
- 双向相遇：A 和 B 分别生成 A′ 与 B′，不产生吞并式统一体。
- 不可译缝隙：明确保存无法被另一世界语法吸收的部分。
- 未知生成器：从价值冲突、认知规则差异和共同不可见中生成新世界种子。
- 规则反身化：把支配“什么可见、谁能发言”的规则本身转成可改变对象。
- 超个体判断：计算组合价值、最佳单体、协同增量、最低世界满足度、差异保持和反事实必要性。
- 开放闭合：每次运行以 `OPEN_WITH_NEW_WORLDS` 结束。
- Mesh 5.4 桥：导出局部 Chart、开放 Seam、UAX 类义务和 `S5.4-OPERABLE-OPEN` 包络。
- ALTERGENESIS Studio：可引入新世界、选择两个世界相遇、查看判断与新世界入口。

## 五分钟运行

```bash
python -m venv .venv
. .venv/bin/activate
python -m pip install -e .

altergenesis demo --out artifacts/demo
altergenesis verify artifacts/demo/session.json
altergenesis serve --scenario examples/research_commons.json
```

浏览器打开：

```text
http://127.0.0.1:8765
```

也可以直接打开 `studio/index.html` 查看冻结的离线演示。

## 固定参考结果

```text
原生认知世界       5
演化世界状态       14
双向相遇           4
生成性未知         8
新世界入口         8
必要世界来源       4
最佳单体价值       0.695051
共同生成价值       0.985129
超个体协同增量    +0.290078
最终状态           OPEN_WITH_NEW_WORLDS
Mesh 5.4           S5.4-OPERABLE-OPEN
```

该数值来自合成研究共同体场景，只证明算法和交互链能够执行，不证明现实群体必然产生同等协同。

## 为什么不是现有 DIKWP 项目的改名

段玉聪当前公开项目已经大量覆盖无定义语义、意图场、世界塑造、跨模型交流、证据与治理。ALTERGENESIS 刻意不再增加一套“大一统语义协议”，而是补充此前未形成独立运行对象的层：

1. **认知世界本身可生成**，而非只在同一任务中路由多个意图；
2. **相遇产生两个被改变的后代**，而非融合成共同表示；
3. **未知拥有改变问题的作用**，而非仅进入 Residual 队列；
4. **整体判断必须通过反事实必要性和协同增量证明其非单体性**；
5. **闭合的产物是 Opening，而非完成证书。**

详见 [`docs/PORTFOLIO_GAP_ANALYSIS_CN.md`](docs/PORTFOLIO_GAP_ANALYSIS_CN.md)。

## 项目状态

这是为段玉聪审阅准备的独立候选实现，尚未成为其 GitHub 正式仓库，也不代表本人、所在机构或任何第三方背书。正式发布前应确认项目名称、作者归属、维护责任和许可证。

## License

Apache-2.0。见 [LICENSE](LICENSE)。
