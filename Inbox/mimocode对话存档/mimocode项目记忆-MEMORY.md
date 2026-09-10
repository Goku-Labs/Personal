# Project memory
_Durable project-level knowledge. Persists across all sessions in this project. Edit only content under italic instructions._

## Project context
_Personal knowledge management system (PKM) for daily thoughts, finance literacy, and personal image management. Pure Markdown files in `D:\documents\Knowledge\Personal\`. Git-backed, GitHub-hosted (private)._

## Rules
_Hard constraints from user that every session must respect._

- **Time sensitivity**: When user says "今天" (today), ALWAYS call `Get-Date` first to confirm the current date. Never assume the system date or rely on context. User explicitly enforced: "时间你不能调用出来吗"
- **Professional terminology**: All note content must use professional terms, not casual/spoken language. Even if source input is informal, output must be properly formatted.
- **Standards first**: CONVENTIONS.md is the canonical source of truth for all note standards. Follow it strictly.
- **Git repo**: `git@github.com:Goku-Labs/Personal.git` (private), branch `main`
- **Daily note recording rules**: When recording work to daily notes, only log actions taken (e.g. "初始化 Git 仓库"), NOT specific content details (e.g. repo description text) or next-step plans. Keep entries factual and action-oriented.
- **Emotional content preservation**: When merging or editing content, preserve verbatim quotes and emotional content (e.g., "你值得被爱"). User values these deeply and notices their absence. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **User identity**: The user is 朱方勇 (called 方勇). Friend is 肖大帅 (肖哥). Never confuse them. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Cherished quotes**: Preserve these verbatim: 「你值得被爱，这句话不是安慰，是事实。」, 「你不需要每句话都很有趣，沉默也是一种陪伴。」, 「有些话不说，对方永远觉得理所当然。我的好意不是应该，我的耐心也不是无限。将心比心，是友情最基本的底线。」, 「花看半开，酒饮微醺，情到深处人自懂。」 [ses_0718a4312ffewlq3XO1kVNX3aB]
- **Family communication guidance**: "多打电话回家，哪怕只是聊聊；听她说说烦恼，不用给解决方案，听着就行。" — user explicitly requested this be recorded as an action reminder. [ses_10c5957d2ffeD6LZ81u0pXgOaH]

## Architecture decisions
_Major design choices with rationale. The "why" matters more than the "what" for future sessions._

- **Inbox → Daily → Topics workflow**: Quick capture into Inbox, structured daily notes, domain knowledge in Topics subdirectories
- **Markdown-only**: Pure Markdown files, compatible with any editor. Obsidian recommended for best experience (双链/图谱).
- **Topic structure**: Each topic is a subdirectory with README.md as index file
- **Daily note template**: Focus on what happened ("今日事项") and how user feels ("心情"). No "下一步计划" section — daily notes record the present, not future plans. [ses_10c5957d2ffeD6LZ81u0pXgOaH]

## Discovered durable knowledge
_Cross-task facts that survive across sessions. Promoted from session checkpoints' §7 when proven durable._

- Finance knowledge base: 25 chapters across 5 stages (金融基础/投资进阶/综合方法论/实践落地/进阶深化) + glossary (~80 terms), estimated 10-12h study time
- Finance chapters 1-17 were restructured on 2026-06-23; chapters 18-25 added 2026-06-24
- Appearance knowledge base: 37 documents across 7 modules (形象管理/服装搭配/护肤美容/体态管理/配饰搭配/品牌购物/场景应用), stored at `D:\documents\Knowledge\Appearance`
- LLM knowledge base: 10 documents (~3573 lines) covering prompt engineering, RAG, AI agents, multimodal, production deployment, conversation systems, AI safety, open-source models, fine-tuning, long text processing. Chinese filenames, per-doc glossary, cross-references, INDEX.md with difficulty ratings. Other 9 knowledge directories remain as outlines.
- **Directory feature lifecycle**: Adding/removing a directory feature requires same 4-file update: README.md (structure), INDEX.md (entry), CONVENTIONS.md (format+tag), Templates/ (template). Diary feature was created then merged back into Daily — same pattern applies in reverse.
- **Mood tracking lives in Daily**: Emotional/mood content consolidated into Daily notes under "心情" section. No separate Diary directory.
- **SSH host key fix**: When `git push` fails with "Host key verification failed", reliable fix: (1) `ssh-keyscan github.com >> known_hosts`, then (2) `ssh -o StrictHostKeyChecking=no -T git@github.com` to force-accept, then (3) `git push`. `ssh-keyscan` alone is insufficient.
- **Emotional resilience in investing**: User's fund profit celebration ("拨开乌云见天日") follows earlier market concerns ("7月都是绿的", "注意力不能太放到上面") — demonstrates that patience and long-term thinking yields emotional rewards. Worth noting in finance learning context. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Fund volatility emotional pattern**: User experienced 大赚 on 7/9 ("拨开乌云见天日") → 血亏 on 7/13 ("我敲啦") → cumulative loss approaching 4000 by 7/16. The emotional contrast is notable — fund returns create significant mood swings. The earlier patience lesson still holds but the volatility is real. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Fund emotional normalization (7/22)**: User experienced 3.61% gain (largest single-day increase) but felt平淡 compared to 7/9's first big gain ("拨开乌云见天日"). This is healthy investment maturity — novelty wears off, rational mindset stabilizes. Pattern: initial excitement → repeated exposure → emotional baseline normalizes. Positive sign for long-term investing. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **IMA project onboarding progression**: 7/9 project plan → 7/13 domain knowledge entry + stakeholder communication → 7/14 full module implementation → 7/15 optimization. Structured incremental onboarding and development process for IMA avionics network end-system delay analysis tool. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **INFP personality traits**: User identified as INFP (introverted, intuitive, feeling, perceiving). Key traits: deep emotional processing, idealistic, sensitive to external stimuli, needs time to recharge after social interactions. This explains online comfort vs. real-life social reservation. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **High sensitivity trait (HSP)**: User absorbs all external signals (expressions, tones, body language), leading to emotional overload in real-life social situations. Online chat provides buffer time and safety distance that real-life interaction lacks. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Self-protection mechanism**: User instinctively activates avoidance/withdrawal when feeling threatened. This is a survival strategy learned in childhood but now limiting opportunities. Awareness of this pattern is the first step to managing it. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Learned helplessness cycle**: User experiences cumulative exhaustion from repeated defeats by the same issue — each failure to restart reinforces "我不行"belief, creating self-fulfilling prophecy. Breaking cycle requires: (1) awareness, (2) lowering the bar ("多撑一天"), (3) celebrating small wins. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Deep交流 deprivation**: User admitted "我已经好久没和人深层交流了" — as INFP/HSP, needs deep connection but finds real-life interaction draining. Creates paradox: need for depth vs. energy cost. AI conversation can partially fulfill this need. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **"直面恐惧" mindset**: User demonstrated ability to recognize emotional decision-making (wanting to sell all funds) and consciously choose to pause ("我选择先冷静，不要清仓"). Pattern: panic → blame → courage → calm. This shows awareness can translate into action when given space. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Family business pressure**: Mother runs a business facing: new competitor (棋牌室) nearby, rising operational costs, summer heat increasing physical burden. Net income significantly reduced. This is a real stressor affecting family wellbeing. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Expanded emotional awareness**: User's reflection "我有时候也需要去关注家人的情绪" shows growth from self-focused emotional processing to recognizing family members' emotional needs. Important developmental step. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Family communication commitment**: User adopted guidance: "多打电话回家，哪怕只是聊聊；听她说说烦恼，不用给解决方案，听着就行." Explicitly requested this be recorded as a lasting action reminder. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Philosophical inspiration "喜欢不一定要拥有"**: On 2026-07-22, user generated this quote as a personal insight after finishing 《小岛经济学》. Connected to experiences: romantic interest in female colleague, friendship ending. Explored similar quotes about letting go and emotional maturity. [ses_0718a4312ffewlq3XO1kVNX3aB]
- **Friendship boundary setting and ending**: User demonstrated ability to directly express dissatisfaction with a friend who repeatedly broke promises and disrespected boundaries. Key statement: "你可以问题不大，但在我这里是个问题." After reflection, concluded the friendship is over due to "思维完全不同" — fundamentally different values about money, respect, and friendship. The friend only responded about money (remaining 1k debt), not about feelings. "金钱驱动回复，情感无人在意" confirmed the value mismatch. Final closure: user reflected on the friend's perspective (friend sees borrowing money as "小事"), recognized the fundamental value mismatch ("你在意的是「情义」，他在意的是「方便」"), and declared "我放下了" — emotional release, not just logical conclusion. Growth from passive acceptance to active boundary enforcement to decisive closure to emotional letting go. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Investment strategy maturation**: User evolved from panic selling (7/16-17) to creating concrete rules: "一周操作一次" (operate once per week) to prevent impulsive decisions. The uncertainty about own motivation ("不知道是我被套住了或害怕还是沉默成本太高，还是相信市场会好起来") is healthy self-awareness. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **"将心比心" as personal principle**: The quote "有些话不说，对方永远觉得理所当然。我的好意不是应该，我的耐心也不是无限。将心比心，是友情最基本的底线。" was chosen by user as their expression of this experience. Now a cherished quote. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Money-driven response pattern**: User discovered that a friend only responded when reminded about remaining debt — all emotional messages about feelings and boundaries were read but ignored. "金钱驱动回复，情感无人在意" — a clear pattern confirming the friend's priorities. This is a red flag for any relationship. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Small-step social goal**: User set an achievable goal: "下次就算只是面对面微笑也好，从最小的动作开始练习主动." This is healthy for an INFP — not overwhelming, just a small step toward social confidence. Worth reinforcing in future sessions. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Sister visit promise**: User promised younger sister a visit from father + sister to visit user. Father may not come due to business pressures (new competitor 棋牌室, rising costs, summer heat). User weighing options to honor the promise — shows growing family responsibility. [ses_10c5957d2ffeD6LZ81u0pXgOaH]
- **Low-stakes social joy (bus encounter 2026-07-23)**: User had a spontaneous wordless interaction with a ~9-year-old girl on the bus (listening to song "女孩"). They exchanged smiles, half-heart gestures, and a goodbye wave — no words at all. He was happy all day and described his own reaction as "小男孩的羞涩" — sweet bashfulness, not painful avoidance. This proves his INFP/HSP nature doesn't prevent joyful connection, just makes it rare. The key: safe environment + warm other party + no stakes = genuine social joy. Contrasts with earlier self-description of social anxiety and avoidance. [ses_0718a4312ffewlq3XO1kVNX3aB]
- **Company network monitoring (7/28)**: Company IT can monitor web browsing activity including Douyin usage. Need to use mobile data for personal browsing during work hours. Practical workplace privacy awareness. [ses_0718a4312ffewlq3XO1kVNX3aB]
- **Fund app uninstall strategy (7/28)**: User uninstalled fund app after market crash, demonstrating strongest investment discipline yet. Goes beyond "一周操作一次" — removes the temptation entirely. Behavioral design: making bad habits harder to execute. [ses_0718a4312ffewlq3XO1kVNX3aB]
