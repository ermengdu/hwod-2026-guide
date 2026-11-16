# 2026 华为 OD 机考新题库刷题指南（180 题全考点图谱 + 力扣 Hot100 对照）

> **数据来源与在线评测平台**：[CodeSeeking 华为 OD 在线题库](https://www.codeseeking.com)  
> **题库规模**：截至 **2026-11-15** 考期，共收录 **180 道 2026 真题**（100 分题 120 道 + 200 分题 60 道），按 **21 个算法考点** 分组，为 **114 道真题** 映射了力扣 Hot100 关联原题，每周随新考期同步更新。

## 项目简介

**CodeSeeking**（`https://www.codeseeking.com`）是专注**华为 OD 机考**的在线判题平台（Online Judge），重点解决备考过程中的三类核心痛点：

1. **新题同步慢、缺乏真题判题环境**：覆盖 2026 最新考期真题（支持 **Core 核心代码模式** 与 **ACM 模式**），每题配备 **20 组严苛测试点**，全站所有题目均支持**免费提交评测**。
2. **刷题孤立、不知道和力扣对应关系**：本指南为每道真题标注了**考期、分值（100/200 分）、站内同类题**以及**力扣 Hot100 对应原题**，方便按专题集中突破。
3. **本地样例能过但提交 WA 难以定位**：支持 **Java / C++ / Python / JavaScript** 四语言提交与参考题解，并提供**失败测试点输入/期望输出对拍**与 **AI 三段式错题定位**。

## 在线刷题与免费权益说明

| 功能模块 | 普通注册用户（免费） | 永久 VIP 用户（爱发电一次开通） |
| :--- | :--- | :--- |
| **全站真题提交评测** | 全站所有题目**完全免费提交**（20 组测试点全量判题） | 同左，全站题目无限提交 |
| **高质量四语言题解** | **考期 8 周之前**的老题与真题题解**免费开放** | 解锁近 8 周最新考期原题题解（标配 Java/C++/Python/JS 代码 + 坑点） |
| **AI 智能错题分析** | 每日 **3 次免费**（0 点重置），精准定位错误代码行与改法 | 每日**不限次数**使用 |
| **失败测试点对拍** | 显示基础评测状态（AC / WA / TLE / RE） | 解锁失败用例详细输入（Input）、期望输出与实际输出对比 |

## 2026 华为 OD 机考考点分布统计（180 题）

按真题出现频次划分为 **P0（高频基石）→ P1（重点拉分）→ P2（中频专题）→ P3（专项补齐）**，建议按专题顺序集中刷题：

| 考点分类 | 真题数 | 100 分题 | 200 分题 | 占比 | 备考优先级 | 关联 Hot100 题数 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 模拟 | 22 | 20 | 2 | 12.2% | P0 核心高频 | 9 |
| 数组和字符串 | 21 | 21 | 0 | 11.7% | P0 核心高频 | 6 |
| 位运算和数学 | 17 | 12 | 5 | 9.4% | P0 核心高频 | 6 |
| 哈希表 | 14 | 12 | 2 | 7.8% | P0 核心高频 | 11 |
| 滑动窗口和双指针 | 13 | 11 | 2 | 7.2% | P0 核心高频 | 13 |
| 图 | 12 | 4 | 8 | 6.7% | P1 重点必刷 | 9 |
| 排序算法 | 11 | 11 | 0 | 6.1% | P1 重点必刷 | 5 |
| 普通树 | 11 | 4 | 7 | 6.1% | P1 重点必刷 | 10 |
| 队列与栈 | 8 | 7 | 1 | 4.4% | P1 重点必刷 | 7 |
| 递归和分治 | 8 | 3 | 5 | 4.4% | P1 重点必刷 | 7 |
| 前缀和 | 6 | 4 | 2 | 3.3% | P2 中频专题 | 5 |
| 状压、计数 & 数位问题 | 6 | 0 | 6 | 3.3% | P2 中频专题 | 1 |
| 广度优先搜索 | 5 | 1 | 4 | 2.8% | P2 中频专题 | 5 |
| 二分查找 | 5 | 1 | 4 | 2.8% | P2 中频专题 | 0 |
| 线性 & 区间问题 | 5 | 2 | 3 | 2.8% | P2 中频专题 | 5 |
| 贪心算法 | 4 | 4 | 0 | 2.2% | P3 专项补齐 | 3 |
| 深度优先搜索 | 3 | 0 | 3 | 1.7% | P3 专项补齐 | 3 |
| 动态规划基础模型 | 3 | 0 | 3 | 1.7% | P3 专项补齐 | 3 |
| 链表 | 2 | 2 | 0 | 1.1% | P3 专项补齐 | 2 |
| 堆 | 2 | 1 | 1 | 1.1% | P3 专项补齐 | 2 |
| 树形、图上、概率 & 博弈问题 | 2 | 0 | 2 | 1.1% | P3 专项补齐 | 2 |
| **合计** | **180** | **120** | **60** | **100%** | — | **114** |

## 高效备考路线建议

1. **先打通 P0 核心专题（87 题，占比 48.3%）**：优先攻克「模拟（22）」「数组和字符串（21）」「位运算和数学（17）」「哈希表（14）」「滑动窗口和双指针（13）」，其中 100 分基础题占比高，是机考保底拿满的关键。
2. **再突破 P1 重点拉分专题（50 题，占比 27.8%）**：集中刷「图（12）」「普通树（11）」「排序算法（11）」「队列与栈（8）」「递归和分治（8）」，其中图、普通树、递归分治包含大量 200 分题。
3. **利用“Hot100 + 同类题”联动刷法**：遇到卡壳的 OD 真题，先做表格最后一列对应的力扣 Hot100 原题巩固模板，再顺着“同类题”连刷 2~3 道巩固手感。

---

## 2026 华为 OD 机考真题全量目录（按 21 个考点分类）

> 组内按最新考期降序排列，所有题目链接直达 CodeSeeking 在线评测页（免费提交）。

### 数组和字符串（21 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [整理学生编号](https://www.codeseeking.com/problem/OD_1218) | 11-01 | 100分 | [简单 URL 路径提取器](https://www.codeseeking.com/problem/OD_1205) / [字符串分组求和](https://www.codeseeking.com/problem/OD_1204) | [字母异位词分组](https://leetcode.cn/problems/group-anagrams/description/) |
| [字符串分组求和](https://www.codeseeking.com/problem/OD_1204) | 09-20 | 100分 | [整理学生编号](https://www.codeseeking.com/problem/OD_1218) | — |
| [查找幸运数](https://www.codeseeking.com/problem/OD_1189) | 09-02 | 100分 | [查找能被整除的最大整数](https://www.codeseeking.com/problem/OD_1093) | — |
| [小牛牛超市选品](https://www.codeseeking.com/problem/OD_1181) | 08-23 | 100分 | [基站低能耗时段统计](https://www.codeseeking.com/problem/OD_1177) | [最小覆盖子串](https://leetcode.cn/problems/minimum-window-substring/description/) |
| [最长不连续子串](https://www.codeseeking.com/problem/OD_1165) | 08-05 | 100分 | [美观的灯笼](https://www.codeseeking.com/problem/OD_1090) / [Skill执行链完整性检测](https://www.codeseeking.com/problem/OD_1106) | — |
| [语义化版本号对比](https://www.codeseeking.com/problem/OD_1163) | 08-02 | 100分 | [日期格式统一与排序](https://www.codeseeking.com/problem/OD_1148) | — |
| [不同Tag类型统计](https://www.codeseeking.com/problem/OD_1153) | 07-22 | 100分 | [循环内存存取计算](https://www.codeseeking.com/problem/OD_1091) | — |
| [日期格式统一与排序](https://www.codeseeking.com/problem/OD_1148) | 07-15 | 100分 | [语义化版本号对比](https://www.codeseeking.com/problem/OD_1163) / [准备生日礼物](https://www.codeseeking.com/problem/OD_1087) | — |
| [字符串压缩编码](https://www.codeseeking.com/problem/OD_1144) | 07-12 | 100分 | [API日志去重合并统计](https://www.codeseeking.com/problem/OD_1067) | [字符串解码](https://leetcode.cn/problems/decode-string/description/) |
| [字符串处理](https://www.codeseeking.com/problem/OD_1123) | 06-17 | 100分 | [酒店服务记录分析](https://www.codeseeking.com/problem/OD_1150) | [划分字母区间](https://leetcode.cn/problems/partition-labels/description/) |
| [字符串格式调整](https://www.codeseeking.com/problem/OD_1120) | 06-14 | 100分 | [设备重排SN](https://www.codeseeking.com/problem/OD_1117) | — |
| [设备重排SN](https://www.codeseeking.com/problem/OD_1117) | 06-10 | 100分 | [整理学生编号](https://www.codeseeking.com/problem/OD_1218) / [字符串格式调整](https://www.codeseeking.com/problem/OD_1120) | — |
| [查找温度记录统计信息](https://www.codeseeking.com/problem/OD_1118) | 06-10 | 100分 | [数据中心最佳维护窗口](https://www.codeseeking.com/problem/OD_1124) / [小花获胜的奶茶](https://www.codeseeking.com/problem/OD_1186) | — |
| [内网IP有效性校验](https://www.codeseeking.com/problem/OD_1115) | 06-07 | 100分 | [IP地址分类识别](https://www.codeseeking.com/problem/OD_1096) / [IPv4 等长子网划分与自动分配系统](https://www.codeseeking.com/problem/OD_1167) | — |
| [Skill执行链完整性检测](https://www.codeseeking.com/problem/OD_1106) | 05-27 | 100分 | [美观的灯笼](https://www.codeseeking.com/problem/OD_1090) / [最长不连续子串](https://www.codeseeking.com/problem/OD_1165) | — |
| [简单表达式运算](https://www.codeseeking.com/problem/OD_1102) | 05-24 | 100分 | [信道资源分配与掩码运算](https://www.codeseeking.com/problem/OD_1175) / [日志规则逆波兰转换](https://www.codeseeking.com/problem/OD_1215) | — |
| [IP地址分类识别](https://www.codeseeking.com/problem/OD_1096) | 05-17 | 100分 | [内网IP有效性校验](https://www.codeseeking.com/problem/OD_1115) / [IPv4 等长子网划分与自动分配系统](https://www.codeseeking.com/problem/OD_1167) | — |
| [查找能被整除的最大整数](https://www.codeseeking.com/problem/OD_1093) | 05-13 | 100分 | [查找幸运数](https://www.codeseeking.com/problem/OD_1189) | — |
| [美观的灯笼](https://www.codeseeking.com/problem/OD_1090) | 05-10 | 100分 | [最长不连续子串](https://www.codeseeking.com/problem/OD_1165) / [Skill执行链完整性检测](https://www.codeseeking.com/problem/OD_1106) | — |
| [匹配命令行前缀的关键字](https://www.codeseeking.com/problem/OD_1081) | 05-06 | 100分 | [简单 URL 路径提取器](https://www.codeseeking.com/problem/OD_1205) | [实现 Trie (前缀树)](https://leetcode.cn/problems/implement-trie-prefix-tree/description/) |
| [失灵的键盘](https://www.codeseeking.com/problem/OD_1066) | 04-15 | 100分 | [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) / [仓库盘点](https://www.codeseeking.com/problem/OD_1135) | [前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/description/) |

### 哈希表（14 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [均衡调度](https://www.codeseeking.com/problem/OD_1210) | 09-27 | 100分 | [双系统资源类型调配](https://www.codeseeking.com/problem/OD_1119) / [终端设备档位差异统计](https://www.codeseeking.com/problem/OD_1129) | [两数之和](https://leetcode.cn/problems/two-sum/description/) |
| [简单 URL 路径提取器](https://www.codeseeking.com/problem/OD_1205) | 09-20 | 100分 | [空间占用计算](https://www.codeseeking.com/problem/OD_1084) / [匹配命令行前缀的关键字](https://www.codeseeking.com/problem/OD_1081) | [实现 Trie (前缀树)](https://leetcode.cn/problems/implement-trie-prefix-tree/description/) |
| [酒店服务记录分析](https://www.codeseeking.com/problem/OD_1150) | 07-19 | 100分 | [文档特征提取](https://www.codeseeking.com/problem/OD_1072) / [字符串处理](https://www.codeseeking.com/problem/OD_1123) | — |
| [谁没交卷](https://www.codeseeking.com/problem/OD_1147) | 07-15 | 100分 | — | [缺失的第一个正数](https://leetcode.cn/problems/first-missing-positive/description/) |
| [仓库盘点](https://www.codeseeking.com/problem/OD_1135) | 07-01 | 100分 | [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) / [失灵的键盘](https://www.codeseeking.com/problem/OD_1066) / [快递驿站计费系统](https://www.codeseeking.com/problem/OD_1187) | [前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/description/) |
| [终端设备档位差异统计](https://www.codeseeking.com/problem/OD_1129) | 06-24 | 100分 | [均衡调度](https://www.codeseeking.com/problem/OD_1210) | [两数之和](https://leetcode.cn/problems/two-sum/description/) |
| [日志关键词统计](https://www.codeseeking.com/problem/OD_1126) | 06-22 | 100分 | [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) | — |
| [双系统资源类型调配](https://www.codeseeking.com/problem/OD_1119) | 06-10 | 200分 | [均衡调度](https://www.codeseeking.com/problem/OD_1210) | — |
| [小学生班长选举](https://www.codeseeking.com/problem/OD_1105) | 05-27 | 100分 | [小学生班长选举增强版](https://www.codeseeking.com/problem/OD_1074) | [多数元素](https://leetcode.cn/problems/majority-element/description/) |
| [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) | 04-29 | 100分 | [仓库盘点](https://www.codeseeking.com/problem/OD_1135) / [失灵的键盘](https://www.codeseeking.com/problem/OD_1066) / [快递驿站计费系统](https://www.codeseeking.com/problem/OD_1187) | [前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/description/) |
| [文档特征提取](https://www.codeseeking.com/problem/OD_1072) | 04-22 | 100分 | [酒店服务记录分析](https://www.codeseeking.com/problem/OD_1150) | [字母异位词分组](https://leetcode.cn/problems/group-anagrams/description/) |
| [小学生班长选举增强版](https://www.codeseeking.com/problem/OD_1074) | 04-22 | 200分 | [小学生班长选举](https://www.codeseeking.com/problem/OD_1105) | [多数元素](https://leetcode.cn/problems/majority-element/description/) |
| [准备生日礼物](https://www.codeseeking.com/problem/OD_1087) | 04-08 | 100分 | [日期格式统一与排序](https://www.codeseeking.com/problem/OD_1148) | [两数之和](https://leetcode.cn/problems/two-sum/description/) |
| [空间占用计算](https://www.codeseeking.com/problem/OD_1084) | 04-01 | 100分 | [简单 URL 路径提取器](https://www.codeseeking.com/problem/OD_1205) / [部门绩效汇总](https://www.codeseeking.com/problem/OD_1185) / [告警抑制编排](https://www.codeseeking.com/problem/OD_1242) | [实现 Trie (前缀树)](https://leetcode.cn/problems/implement-trie-prefix-tree/description/) |

### 排序算法（11 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [近邻向量检索](https://www.codeseeking.com/problem/OD_1243) | 11-15 | 100分 | [分辨率排序](https://www.codeseeking.com/problem/OD_1070) / [库存补货优先级排序](https://www.codeseeking.com/problem/OD_1240) | [前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/description/) |
| [管线同类区段归并](https://www.codeseeking.com/problem/OD_1237) | 11-11 | 100分 | [螳螂领地争霸](https://www.codeseeking.com/problem/OD_1190) / [智能广播合并台号](https://www.codeseeking.com/problem/OD_1166) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |
| [工具慢调用均值](https://www.codeseeking.com/problem/OD_1238) | 11-11 | 100分 | [仓库盘点](https://www.codeseeking.com/problem/OD_1135) / [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) | — |
| [分组字符串排序](https://www.codeseeking.com/problem/OD_1224) | 10-14 | 100分 | [区分奇偶的数组排序](https://www.codeseeking.com/problem/OD_1156) / [货运装载顺序校验](https://www.codeseeking.com/problem/OD_1232) | — |
| [库存补货优先级排序](https://www.codeseeking.com/problem/OD_1240) | 10-11 | 100分 | [分辨率排序](https://www.codeseeking.com/problem/OD_1070) / [省超足球比赛获胜队伍计算](https://www.codeseeking.com/problem/OD_1138) / [近邻向量检索](https://www.codeseeking.com/problem/OD_1243) | — |
| [螳螂领地争霸](https://www.codeseeking.com/problem/OD_1190) | 09-02 | 100分 | [统计不重叠区间的个数](https://www.codeseeking.com/problem/OD_1133) / [智能广播合并台号](https://www.codeseeking.com/problem/OD_1166) / [管线同类区段归并](https://www.codeseeking.com/problem/OD_1237) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |
| [智能广播合并台号](https://www.codeseeking.com/problem/OD_1166) | 08-05 | 100分 | [螳螂领地争霸](https://www.codeseeking.com/problem/OD_1190) / [管线同类区段归并](https://www.codeseeking.com/problem/OD_1237) | [最长连续序列](https://leetcode.cn/problems/longest-consecutive-sequence/description/) |
| [区分奇偶的数组排序](https://www.codeseeking.com/problem/OD_1156) | 07-26 | 100分 | [链表数字游戏](https://www.codeseeking.com/problem/OD_1108) / [分组字符串排序](https://www.codeseeking.com/problem/OD_1224) | — |
| [最小极差分组](https://www.codeseeking.com/problem/OD_1132) | 06-28 | 100分 | — | — |
| [统计不重叠区间的个数](https://www.codeseeking.com/problem/OD_1133) | 06-28 | 100分 | [螳螂领地争霸](https://www.codeseeking.com/problem/OD_1190) / [最大化游戏试玩资格分发](https://www.codeseeking.com/problem/OD_1076) / [LLM推理批次最大化](https://www.codeseeking.com/problem/OD_1171) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |
| [分辨率排序](https://www.codeseeking.com/problem/OD_1070) | 04-19 | 100分 | [省超足球比赛获胜队伍计算](https://www.codeseeking.com/problem/OD_1138) / [库存补货优先级排序](https://www.codeseeking.com/problem/OD_1240) / [近邻向量检索](https://www.codeseeking.com/problem/OD_1243) | — |

### 链表（2 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [手机桌面整理](https://www.codeseeking.com/problem/OD_1198) | 09-13 | 100分 | [操作历史管理器的撤销/重做能力](https://www.codeseeking.com/problem/OD_1079) | [LRU 缓存](https://leetcode.cn/problems/lru-cache/description/) |
| [操作历史管理器的撤销/重做能力](https://www.codeseeking.com/problem/OD_1079) | 04-29 | 100分 | [手机桌面整理](https://www.codeseeking.com/problem/OD_1198) | [LRU 缓存](https://leetcode.cn/problems/lru-cache/description/) |

### 深度优先搜索（3 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [单词搜索计数](https://www.codeseeking.com/problem/OD_1188) | 08-30 | 200分 | [勇攀数字高峰](https://www.codeseeking.com/problem/OD_1086) | [单词搜索](https://leetcode.cn/problems/word-search/description/) |
| [抗洪救灾](https://www.codeseeking.com/problem/OD_1182) | 08-23 | 200分 | [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) / [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) | [岛屿数量](https://leetcode.cn/problems/number-of-islands/description/) |
| [WiFi 设备网络规划](https://www.codeseeking.com/problem/OD_1071) | 04-19 | 200分 | [云服务安全策略最优选择](https://www.codeseeking.com/problem/OD_1131) / [智能家居模式调度优化](https://www.codeseeking.com/problem/OD_1176) | [N 皇后](https://leetcode.cn/problems/n-queens/description/) |

### 广度优先搜索（5 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [小菊的寻宝之旅](https://www.codeseeking.com/problem/OD_1208) | 09-23 | 100分 | [直捣黄龙](https://www.codeseeking.com/problem/OD_1089) / [迷宫相遇](https://www.codeseeking.com/problem/OD_1143) / [毕业旅行](https://www.codeseeking.com/problem/OD_1149) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |
| [软件依赖树](https://www.codeseeking.com/problem/OD_1146) | 07-12 | 200分 | [项目模块依赖构建顺序规划](https://www.codeseeking.com/problem/OD_1077) / [返回所有加载的AGENTS.md文件ID列表](https://www.codeseeking.com/problem/OD_1112) | [二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/description/) |
| [迷宫相遇](https://www.codeseeking.com/problem/OD_1143) | 07-08 | 200分 | [直捣黄龙](https://www.codeseeking.com/problem/OD_1089) / [小菊的寻宝之旅](https://www.codeseeking.com/problem/OD_1208) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |
| [社交网络相同爱好好友查询](https://www.codeseeking.com/problem/OD_1095) | 05-13 | 200分 | [社交网络消息转发](https://www.codeseeking.com/problem/OD_1216) / [小菊的寻宝之旅](https://www.codeseeking.com/problem/OD_1208) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |
| [直捣黄龙](https://www.codeseeking.com/problem/OD_1089) | 04-08 | 200分 | [小菊的寻宝之旅](https://www.codeseeking.com/problem/OD_1208) / [迷宫相遇](https://www.codeseeking.com/problem/OD_1143) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |

### 二分查找（5 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [港口运输](https://www.codeseeking.com/problem/OD_1231) | 10-21 | 100分 | [末世分配资源包](https://www.codeseeking.com/problem/OD_1173) / [数据包分段传输的最小最大延迟](https://www.codeseeking.com/problem/OD_1128) / [园区基站节能部署规划](https://www.codeseeking.com/problem/OD_1203) | — |
| [坚果巧克力](https://www.codeseeking.com/problem/OD_1212) | 09-27 | 200分 | [园区基站节能部署规划](https://www.codeseeking.com/problem/OD_1203) / [相机对焦区域最优选择](https://www.codeseeking.com/problem/OD_1223) | — |
| [园区基站节能部署规划](https://www.codeseeking.com/problem/OD_1203) | 09-16 | 200分 | [末世分配资源包](https://www.codeseeking.com/problem/OD_1173) / [数据包分段传输的最小最大延迟](https://www.codeseeking.com/problem/OD_1128) / [坚果巧克力](https://www.codeseeking.com/problem/OD_1212) | — |
| [末世分配资源包](https://www.codeseeking.com/problem/OD_1173) | 08-12 | 200分 | [数据包分段传输的最小最大延迟](https://www.codeseeking.com/problem/OD_1128) / [园区基站节能部署规划](https://www.codeseeking.com/problem/OD_1203) / [港口运输](https://www.codeseeking.com/problem/OD_1231) | — |
| [数据包分段传输的最小最大延迟](https://www.codeseeking.com/problem/OD_1128) | 06-22 | 200分 | [末世分配资源包](https://www.codeseeking.com/problem/OD_1173) / [园区基站节能部署规划](https://www.codeseeking.com/problem/OD_1203) / [港口运输](https://www.codeseeking.com/problem/OD_1231) | — |

### 普通树（11 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [山区救援路线规划](https://www.codeseeking.com/problem/OD_1220) | 11-01 | 200分 | [盘丝洞破阵寻珠](https://www.codeseeking.com/problem/OD_1134) | [路径总和 III](https://leetcode.cn/problems/path-sum-iii/description/) |
| [深度奇偶前序筛选](https://www.codeseeking.com/problem/OD_1230) | 10-21 | 100分 | [盘丝洞破阵寻珠](https://www.codeseeking.com/problem/OD_1134) / [企业内部部门的最大层级](https://www.codeseeking.com/problem/OD_1109) | [二叉树的中序遍历](https://leetcode.cn/problems/binary-tree-inorder-traversal/description/) |
| [告警抑制编排](https://www.codeseeking.com/problem/OD_1242) | 10-11 | 200分 | [返回所有加载的AGENTS.md文件ID列表](https://www.codeseeking.com/problem/OD_1112) / [空间占用计算](https://www.codeseeking.com/problem/OD_1084) | — |
| [部门绩效汇总](https://www.codeseeking.com/problem/OD_1185) | 08-26 | 200分 | [空间占用计算](https://www.codeseeking.com/problem/OD_1084) / [点亮战争迷雾](https://www.codeseeking.com/problem/OD_1179) | [二叉树的直径](https://leetcode.cn/problems/diameter-of-binary-tree/description/) |
| [获取二叉树第k层的数值](https://www.codeseeking.com/problem/OD_1172) | 08-12 | 100分 | [企业内部部门的最大层级](https://www.codeseeking.com/problem/OD_1109) / [返回所有加载的AGENTS.md文件ID列表](https://www.codeseeking.com/problem/OD_1112) | [二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/description/) |
| [二叉树两节点间的最小跳数](https://www.codeseeking.com/problem/OD_1140) | 07-05 | 200分 | [企业内部部门的最大层级](https://www.codeseeking.com/problem/OD_1109) | [二叉树的最近公共祖先](https://leetcode.cn/problems/lowest-common-ancestor-of-a-binary-tree/description/) |
| [盘丝洞破阵寻珠](https://www.codeseeking.com/problem/OD_1134) | 06-28 | 200分 | [山区救援路线规划](https://www.codeseeking.com/problem/OD_1220) / [深度奇偶前序筛选](https://www.codeseeking.com/problem/OD_1230) | [路径总和 III](https://leetcode.cn/problems/path-sum-iii/description/) |
| [返回所有加载的AGENTS.md文件ID列表](https://www.codeseeking.com/problem/OD_1112) | 06-03 | 100分 | [获取二叉树第k层的数值](https://www.codeseeking.com/problem/OD_1172) / [软件依赖树](https://www.codeseeking.com/problem/OD_1146) / [告警抑制编排](https://www.codeseeking.com/problem/OD_1242) | [二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/description/) |
| [企业内部部门的最大层级](https://www.codeseeking.com/problem/OD_1109) | 05-31 | 100分 | [获取二叉树第k层的数值](https://www.codeseeking.com/problem/OD_1172) / [二叉树两节点间的最小跳数](https://www.codeseeking.com/problem/OD_1140) | [二叉树的最大深度](https://leetcode.cn/problems/maximum-depth-of-binary-tree/description/) |
| [输出二叉树后序遍历结果](https://www.codeseeking.com/problem/OD_1098) | 05-17 | 200分 | — | [从前序与中序遍历序列构造二叉树](https://leetcode.cn/problems/construct-binary-tree-from-preorder-and-inorder-traversal/description/) |
| [寻找重复子数据](https://www.codeseeking.com/problem/OD_1083) | 05-06 | 200分 | [部门绩效汇总](https://www.codeseeking.com/problem/OD_1185) | [对称二叉树](https://leetcode.cn/problems/symmetric-tree/description/) |

### 图（12 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [流水线最短总时间](https://www.codeseeking.com/problem/OD_1245) | 11-15 | 200分 | [小花的AI Workflow设计](https://www.codeseeking.com/problem/OD_1228) / [项目模块依赖构建顺序规划](https://www.codeseeking.com/problem/OD_1077) | [课程表](https://leetcode.cn/problems/course-schedule/description/) |
| [小花的AI Workflow设计](https://www.codeseeking.com/problem/OD_1228) | 10-18 | 100分 | [勇攀数字高峰](https://www.codeseeking.com/problem/OD_1086) / [项目模块依赖构建顺序规划](https://www.codeseeking.com/problem/OD_1077) / [流水线最短总时间](https://www.codeseeking.com/problem/OD_1245) | [课程表](https://leetcode.cn/problems/course-schedule/description/) |
| [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) | 09-13 | 200分 | [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) / [分析电网负载均衡](https://www.codeseeking.com/problem/OD_1122) / [计算碳排放减少量](https://www.codeseeking.com/problem/OD_1142) | [岛屿数量](https://leetcode.cn/problems/number-of-islands/description/) |
| [图的遍历](https://www.codeseeking.com/problem/OD_1196) | 09-09 | 100分 | [寻找孤立水站](https://www.codeseeking.com/problem/OD_1092) | — |
| [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) | 07-26 | 200分 | [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) / [分析电网负载均衡](https://www.codeseeking.com/problem/OD_1122) / [计算碳排放减少量](https://www.codeseeking.com/problem/OD_1142) | [岛屿数量](https://leetcode.cn/problems/number-of-islands/description/) |
| [毕业旅行](https://www.codeseeking.com/problem/OD_1149) | 07-15 | 200分 | [小菊的寻宝之旅](https://www.codeseeking.com/problem/OD_1208) | — |
| [计算碳排放减少量](https://www.codeseeking.com/problem/OD_1142) | 07-08 | 100分 | [分析电网负载均衡](https://www.codeseeking.com/problem/OD_1122) / [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) / [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) | [岛屿数量](https://leetcode.cn/problems/number-of-islands/description/) |
| [SQL记录拆分](https://www.codeseeking.com/problem/OD_1139) | 07-05 | 100分 | [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) / [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) | [划分字母区间](https://leetcode.cn/problems/partition-labels/description/) |
| [分析电网负载均衡](https://www.codeseeking.com/problem/OD_1122) | 06-14 | 200分 | [计算碳排放减少量](https://www.codeseeking.com/problem/OD_1142) / [炸弹人的雷区数量](https://www.codeseeking.com/problem/OD_1158) / [路由器网络连通性检测](https://www.codeseeking.com/problem/OD_1200) | [岛屿数量](https://leetcode.cn/problems/number-of-islands/description/) |
| [资源二分类隔离判定](https://www.codeseeking.com/problem/OD_1113) | 06-03 | 200分 | — | — |
| [寻找孤立水站](https://www.codeseeking.com/problem/OD_1092) | 05-10 | 200分 | [社交网络消息转发](https://www.codeseeking.com/problem/OD_1216) / [图的遍历](https://www.codeseeking.com/problem/OD_1196) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |
| [项目模块依赖构建顺序规划](https://www.codeseeking.com/problem/OD_1077) | 04-26 | 200分 | [软件依赖树](https://www.codeseeking.com/problem/OD_1146) / [魔法咒语组合](https://www.codeseeking.com/problem/OD_1141) / [流水线最短总时间](https://www.codeseeking.com/problem/OD_1245) | [课程表](https://leetcode.cn/problems/course-schedule/description/) / [全排列](https://leetcode.cn/problems/permutations/description/) |

### 前缀和（6 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [寻找服务器组的最小差值下标](https://www.codeseeking.com/problem/OD_1234) | 11-08 | 100分 | [查找最佳充电策略](https://www.codeseeking.com/problem/OD_1168) | [除自身以外数组的乘积](https://leetcode.cn/problems/product-of-array-except-self/description/) |
| [相机对焦区域最优选择](https://www.codeseeking.com/problem/OD_1223) | 11-04 | 200分 | [坚果巧克力](https://www.codeseeking.com/problem/OD_1212) | — |
| [获取利润第K大的值](https://www.codeseeking.com/problem/OD_1219) | 11-01 | 100分 | [统计盈利目标区间](https://www.codeseeking.com/problem/OD_1111) / [仓库查询](https://www.codeseeking.com/problem/OD_1183) / [货运装载顺序校验](https://www.codeseeking.com/problem/OD_1232) | [数组中的第K个最大元素](https://leetcode.cn/problems/kth-largest-element-in-an-array/description/) |
| [数据中心最佳维护时间窗](https://www.codeseeking.com/problem/OD_1211) | 09-27 | 100分 | [数据中心最佳维护窗口](https://www.codeseeking.com/problem/OD_1124) / [基于上报数据的实时最大值](https://www.codeseeking.com/problem/OD_1160) / [矿区最短开采段](https://www.codeseeking.com/problem/OD_1239) | [滑动窗口最大值](https://leetcode.cn/problems/sliding-window-maximum/description/) |
| [统计盈利目标区间](https://www.codeseeking.com/problem/OD_1111) | 06-03 | 100分 | [魔法阵的能量收集](https://www.codeseeking.com/problem/OD_1110) / [获取利润第K大的值](https://www.codeseeking.com/problem/OD_1219) | [和为 K 的子数组](https://leetcode.cn/problems/subarray-sum-equals-k/description/) |
| [魔法阵的能量收集](https://www.codeseeking.com/problem/OD_1110) | 05-31 | 200分 | [统计盈利目标区间](https://www.codeseeking.com/problem/OD_1111) | [和为 K 的子数组](https://leetcode.cn/problems/subarray-sum-equals-k/description/) |

### 滑动窗口和双指针（13 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [矿区最短开采段](https://www.codeseeking.com/problem/OD_1239) | 11-11 | 200分 | [数据中心最佳维护时间窗](https://www.codeseeking.com/problem/OD_1211) / [基站低能耗时段统计](https://www.codeseeking.com/problem/OD_1177) / [快递传送带分拣](https://www.codeseeking.com/problem/OD_1241) | [滑动窗口最大值](https://leetcode.cn/problems/sliding-window-maximum/description/) |
| [HTTP 访问日志峰值请求数](https://www.codeseeking.com/problem/OD_1235) | 11-08 | 100分 | [基站低能耗时段统计](https://www.codeseeking.com/problem/OD_1177) / [统计能源使用时段](https://www.codeseeking.com/problem/OD_1154) | [无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/description/) |
| [汽车出行路线重复检测](https://www.codeseeking.com/problem/OD_1221) | 11-04 | 100分 | [小学英语老师批改作文](https://www.codeseeking.com/problem/OD_1099) / [统计能源使用时段](https://www.codeseeking.com/problem/OD_1154) | [无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/description/) |
| [快递传送带分拣](https://www.codeseeking.com/problem/OD_1241) | 10-11 | 100分 | [矿区最短开采段](https://www.codeseeking.com/problem/OD_1239) / [数据中心最佳维护时间窗](https://www.codeseeking.com/problem/OD_1211) | [滑动窗口最大值](https://leetcode.cn/problems/sliding-window-maximum/description/) |
| [小花获胜的奶茶](https://www.codeseeking.com/problem/OD_1186) | 08-30 | 100分 | [数据中心最佳维护窗口](https://www.codeseeking.com/problem/OD_1124) / [查找最佳充电策略](https://www.codeseeking.com/problem/OD_1168) | [找到字符串中所有字母异位词](https://leetcode.cn/problems/find-all-anagrams-in-a-string/description/) |
| [字符串回文判断](https://www.codeseeking.com/problem/OD_1184) | 08-26 | 100分 | — | [最长回文子串](https://leetcode.cn/problems/longest-palindromic-substring/description/) |
| [基站低能耗时段统计](https://www.codeseeking.com/problem/OD_1177) | 08-19 | 100分 | [统计能源使用时段](https://www.codeseeking.com/problem/OD_1154) / [小牛牛超市选品](https://www.codeseeking.com/problem/OD_1181) / [HTTP 访问日志峰值请求数](https://www.codeseeking.com/problem/OD_1235) | [无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/description/) |
| [查找最佳充电策略](https://www.codeseeking.com/problem/OD_1168) | 08-09 | 100分 | [数据中心最佳维护窗口](https://www.codeseeking.com/problem/OD_1124) / [小花获胜的奶茶](https://www.codeseeking.com/problem/OD_1186) / [寻找服务器组的最小差值下标](https://www.codeseeking.com/problem/OD_1234) | [找到字符串中所有字母异位词](https://leetcode.cn/problems/find-all-anagrams-in-a-string/description/) |
| [统计能源使用时段](https://www.codeseeking.com/problem/OD_1154) | 07-22 | 100分 | [小学英语老师批改作文](https://www.codeseeking.com/problem/OD_1099) / [基站低能耗时段统计](https://www.codeseeking.com/problem/OD_1177) / [HTTP 访问日志峰值请求数](https://www.codeseeking.com/problem/OD_1235) | [无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/description/) |
| [奇偶三数之和](https://www.codeseeking.com/problem/OD_1136) | 07-01 | 100分 | — | [三数之和](https://leetcode.cn/problems/3sum/description/) |
| [收集灵草](https://www.codeseeking.com/problem/OD_1137) | 07-01 | 200分 | [战士技能规划设计](https://www.codeseeking.com/problem/OD_1164) | [最大子数组和](https://leetcode.cn/problems/maximum-subarray/description/) |
| [数据中心最佳维护窗口](https://www.codeseeking.com/problem/OD_1124) | 06-17 | 100分 | [查找最佳充电策略](https://www.codeseeking.com/problem/OD_1168) / [小花获胜的奶茶](https://www.codeseeking.com/problem/OD_1186) / [数据中心最佳维护时间窗](https://www.codeseeking.com/problem/OD_1211) | [找到字符串中所有字母异位词](https://leetcode.cn/problems/find-all-anagrams-in-a-string/description/) |
| [小学英语老师批改作文](https://www.codeseeking.com/problem/OD_1099) | 05-20 | 100分 | [统计能源使用时段](https://www.codeseeking.com/problem/OD_1154) / [汽车出行路线重复检测](https://www.codeseeking.com/problem/OD_1221) | [无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/description/) |

### 队列与栈（8 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [河流水系流量评估](https://www.codeseeking.com/problem/OD_1222) | 11-04 | 100分 | [日志规则逆波兰转换](https://www.codeseeking.com/problem/OD_1215) | [字符串解码](https://leetcode.cn/problems/decode-string/description/) |
| [日志规则逆波兰转换](https://www.codeseeking.com/problem/OD_1215) | 10-28 | 100分 | [简单表达式运算](https://www.codeseeking.com/problem/OD_1102) / [河流水系流量评估](https://www.codeseeking.com/problem/OD_1222) | [字符串解码](https://leetcode.cn/problems/decode-string/description/) |
| [AI推理任务并行额度最大值](https://www.codeseeking.com/problem/OD_1217) | 10-28 | 200分 | [物流仓库货物调配优化](https://www.codeseeking.com/problem/OD_1082) | [柱状图中最大的矩形](https://leetcode.cn/problems/largest-rectangle-in-histogram/description/) |
| [仓储货物有序出库](https://www.codeseeking.com/problem/OD_1192) | 09-06 | 100分 | [消消乐-能量对撞](https://www.codeseeking.com/problem/OD_1159) | — |
| [消消乐-能量对撞](https://www.codeseeking.com/problem/OD_1159) | 07-29 | 100分 | [仓储货物有序出库](https://www.codeseeking.com/problem/OD_1192) | [有效的括号](https://leetcode.cn/problems/valid-parentheses/description/) |
| [查找满足条件的数据包](https://www.codeseeking.com/problem/OD_1145) | 07-12 | 100分 | [数据包优先级窗口查找](https://www.codeseeking.com/problem/OD_1094) / [端口流量统计](https://www.codeseeking.com/problem/OD_1075) | [每日温度](https://leetcode.cn/problems/daily-temperatures/description/) |
| [数据包优先级窗口查找](https://www.codeseeking.com/problem/OD_1094) | 05-13 | 100分 | [端口流量统计](https://www.codeseeking.com/problem/OD_1075) / [查找满足条件的数据包](https://www.codeseeking.com/problem/OD_1145) | [每日温度](https://leetcode.cn/problems/daily-temperatures/description/) |
| [端口流量统计](https://www.codeseeking.com/problem/OD_1075) | 04-26 | 100分 | [数据包优先级窗口查找](https://www.codeseeking.com/problem/OD_1094) / [查找满足条件的数据包](https://www.codeseeking.com/problem/OD_1145) | [每日温度](https://leetcode.cn/problems/daily-temperatures/description/) |

### 堆（2 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [仓库查询](https://www.codeseeking.com/problem/OD_1183) | 08-26 | 100分 | [优化充电桩调度算法](https://www.codeseeking.com/problem/OD_1104) | [数据流的中位数](https://leetcode.cn/problems/find-median-from-data-stream/description/) |
| [优化充电桩调度算法](https://www.codeseeking.com/problem/OD_1104) | 05-24 | 200分 | [路口等待时间](https://www.codeseeking.com/problem/OD_1161) / [仓库查询](https://www.codeseeking.com/problem/OD_1183) | [数组中的第K个最大元素](https://leetcode.cn/problems/kth-largest-element-in-an-array/description/) |

### 递归和分治（8 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [货运装载顺序校验](https://www.codeseeking.com/problem/OD_1232) | 10-21 | 200分 | [获取利润第K大的值](https://www.codeseeking.com/problem/OD_1219) / [分组字符串排序](https://www.codeseeking.com/problem/OD_1224) | [排序链表](https://leetcode.cn/problems/sort-list/description/) |
| [递增差排列](https://www.codeseeking.com/problem/OD_1206) | 09-20 | 200分 | [魔法咒语组合](https://www.codeseeking.com/problem/OD_1141) | [全排列](https://leetcode.cn/problems/permutations/description/) |
| [统计特殊数字](https://www.codeseeking.com/problem/OD_1201) | 09-16 | 100分 | — | [组合总和](https://leetcode.cn/problems/combination-sum/description/) |
| [受限任务分配](https://www.codeseeking.com/problem/OD_1197) | 09-09 | 200分 | — | — |
| [智能家居模式调度优化](https://www.codeseeking.com/problem/OD_1176) | 08-16 | 200分 | [云服务安全策略最优选择](https://www.codeseeking.com/problem/OD_1131) / [WiFi 设备网络规划](https://www.codeseeking.com/problem/OD_1071) | [子集](https://leetcode.cn/problems/subsets/description/) |
| [魔法咒语组合](https://www.codeseeking.com/problem/OD_1141) | 07-08 | 100分 | [递增差排列](https://www.codeseeking.com/problem/OD_1206) / [项目模块依赖构建顺序规划](https://www.codeseeking.com/problem/OD_1077) | [全排列](https://leetcode.cn/problems/permutations/description/) |
| [云服务安全策略最优选择](https://www.codeseeking.com/problem/OD_1131) | 06-24 | 200分 | [WiFi 设备网络规划](https://www.codeseeking.com/problem/OD_1071) / [智能家居模式调度优化](https://www.codeseeking.com/problem/OD_1176) | [子集](https://leetcode.cn/problems/subsets/description/) |
| [麻将基本胡牌型判断](https://www.codeseeking.com/problem/OD_1097) | 05-17 | 100分 | — | [组合总和](https://leetcode.cn/problems/combination-sum/description/) |

### 贪心算法（4 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [视频监控系统](https://www.codeseeking.com/problem/OD_1214) | 10-25 | 100分 | — | — |
| [LLM推理批次最大化](https://www.codeseeking.com/problem/OD_1171) | 08-12 | 100分 | [最大化游戏试玩资格分发](https://www.codeseeking.com/problem/OD_1076) / [统计不重叠区间的个数](https://www.codeseeking.com/problem/OD_1133) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |
| [物流仓库货物调配优化](https://www.codeseeking.com/problem/OD_1082) | 05-07 | 100分 | [AI推理任务并行额度最大值](https://www.codeseeking.com/problem/OD_1217) | [柱状图中最大的矩形](https://leetcode.cn/problems/largest-rectangle-in-histogram/description/) |
| [最大化游戏试玩资格分发](https://www.codeseeking.com/problem/OD_1076) | 04-26 | 100分 | [LLM推理批次最大化](https://www.codeseeking.com/problem/OD_1171) / [统计不重叠区间的个数](https://www.codeseeking.com/problem/OD_1133) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |

### 位运算和数学（17 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [社交网络消息转发](https://www.codeseeking.com/problem/OD_1216) | 10-28 | 100分 | [寻找孤立水站](https://www.codeseeking.com/problem/OD_1092) / [社交网络相同爱好好友查询](https://www.codeseeking.com/problem/OD_1095) | [腐烂的橘子](https://leetcode.cn/problems/rotting-oranges/description/) |
| [社区赢手机比赛](https://www.codeseeking.com/problem/OD_1229) | 10-18 | 200分 | [最小代价完成论文评审](https://www.codeseeking.com/problem/OD_1155) | [子集](https://leetcode.cn/problems/subsets/description/) |
| [世界杯徽章换购](https://www.codeseeking.com/problem/OD_1207) | 09-23 | 100分 | [物流运输队列调度优化](https://www.codeseeking.com/problem/OD_1227) | — |
| [受限序列重排](https://www.codeseeking.com/problem/OD_1199) | 09-13 | 100分 | [获取大写字母瓷砖拼出独特图案数量](https://www.codeseeking.com/problem/OD_1080) | [全排列](https://leetcode.cn/problems/permutations/description/) |
| [嵌入式传感器寄存器数据解析](https://www.codeseeking.com/problem/OD_1194) | 09-06 | 200分 | [8位LED控制器](https://www.codeseeking.com/problem/OD_1069) | — |
| [大整数位序反转](https://www.codeseeking.com/problem/OD_1178) | 08-19 | 100分 | [数字系统转换器](https://www.codeseeking.com/problem/OD_1157) | [两数相加](https://leetcode.cn/problems/add-two-numbers/description/) |
| [电池充电时间计算](https://www.codeseeking.com/problem/OD_1174) | 08-16 | 100分 | [计算电动车续航里程](https://www.codeseeking.com/problem/OD_1162) | — |
| [信道资源分配与掩码运算](https://www.codeseeking.com/problem/OD_1175) | 08-16 | 100分 | [8位LED控制器](https://www.codeseeking.com/problem/OD_1069) / [简单表达式运算](https://www.codeseeking.com/problem/OD_1102) | — |
| [IPv4 等长子网划分与自动分配系统](https://www.codeseeking.com/problem/OD_1167) | 08-05 | 200分 | [IP地址分类识别](https://www.codeseeking.com/problem/OD_1096) / [内网IP有效性校验](https://www.codeseeking.com/problem/OD_1115) | — |
| [计算电动车续航里程](https://www.codeseeking.com/problem/OD_1162) | 08-02 | 100分 | [电池充电时间计算](https://www.codeseeking.com/problem/OD_1174) | — |
| [数字系统转换器](https://www.codeseeking.com/problem/OD_1157) | 07-26 | 100分 | [大整数位序反转](https://www.codeseeking.com/problem/OD_1178) / [进制转换后自定义排序](https://www.codeseeking.com/problem/OD_1121) | [两数相加](https://leetcode.cn/problems/add-two-numbers/description/) |
| [最小代价完成论文评审](https://www.codeseeking.com/problem/OD_1155) | 07-22 | 200分 | [云南菌子加工](https://www.codeseeking.com/problem/OD_1170) / [无人机巡检航线规划](https://www.codeseeking.com/problem/OD_1191) / [社区赢手机比赛](https://www.codeseeking.com/problem/OD_1229) | [子集](https://leetcode.cn/problems/subsets/description/) |
| [预测新能源发电量](https://www.codeseeking.com/problem/OD_1127) | 06-22 | 100分 | — | — |
| [数组按二进制比特排序](https://www.codeseeking.com/problem/OD_1125) | 06-17 | 200分 | [矩阵螺旋遍历与二进制特征](https://www.codeseeking.com/problem/OD_1202) / [等距二进制判断](https://www.codeseeking.com/problem/OD_1100) | — |
| [进制转换后自定义排序](https://www.codeseeking.com/problem/OD_1121) | 06-14 | 100分 | [数字系统转换器](https://www.codeseeking.com/problem/OD_1157) | — |
| [等距二进制判断](https://www.codeseeking.com/problem/OD_1100) | 05-20 | 100分 | [数组按二进制比特排序](https://www.codeseeking.com/problem/OD_1125) | — |
| [8位LED控制器](https://www.codeseeking.com/problem/OD_1069) | 04-19 | 100分 | [嵌入式传感器寄存器数据解析](https://www.codeseeking.com/problem/OD_1194) / [信道资源分配与掩码运算](https://www.codeseeking.com/problem/OD_1175) | — |

### 动态规划基础模型（3 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [自由摄影师的最大收益](https://www.codeseeking.com/problem/OD_1209) | 09-23 | 200分 | [最佳任务统筹](https://www.codeseeking.com/problem/OD_1116) / [多模型版本的最优调度](https://www.codeseeking.com/problem/OD_1101) | [分割等和子集](https://leetcode.cn/problems/partition-equal-subset-sum/description/) |
| [最佳任务统筹](https://www.codeseeking.com/problem/OD_1116) | 06-07 | 200分 | [自由摄影师的最大收益](https://www.codeseeking.com/problem/OD_1209) / [多模型版本的最优调度](https://www.codeseeking.com/problem/OD_1101) | [分割等和子集](https://leetcode.cn/problems/partition-equal-subset-sum/description/) |
| [多模型版本的最优调度](https://www.codeseeking.com/problem/OD_1101) | 05-20 | 200分 | [最佳任务统筹](https://www.codeseeking.com/problem/OD_1116) / [自由摄影师的最大收益](https://www.codeseeking.com/problem/OD_1209) | [零钱兑换](https://leetcode.cn/problems/coin-change/description/) |

### 线性 & 区间问题（5 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [少儿爬山闯关积分游戏](https://www.codeseeking.com/problem/OD_1193) | 09-06 | 100分 | [直线冲刺](https://www.codeseeking.com/problem/OD_1180) / [充电桩最优布局规划](https://www.codeseeking.com/problem/OD_1107) | [爬楼梯](https://leetcode.cn/problems/climbing-stairs/description/) |
| [战士技能规划设计](https://www.codeseeking.com/problem/OD_1164) | 08-02 | 200分 | [收集灵草](https://www.codeseeking.com/problem/OD_1137) | [除了自身以外数组的乘积](https://leetcode.cn/problems/product-of-array-except-self/description/) |
| [小明的顺风车](https://www.codeseeking.com/problem/OD_1152) | 07-19 | 200分 | [最大化游戏试玩资格分发](https://www.codeseeking.com/problem/OD_1076) / [LLM推理批次最大化](https://www.codeseeking.com/problem/OD_1171) | [打家劫舍](https://leetcode.cn/problems/house-robber/description/) |
| [充电桩最优布局规划](https://www.codeseeking.com/problem/OD_1107) | 05-27 | 200分 | [最小请求间隔限流策略](https://www.codeseeking.com/problem/OD_1103) / [少儿爬山闯关积分游戏](https://www.codeseeking.com/problem/OD_1193) | [打家劫舍](https://leetcode.cn/problems/house-robber/description/) |
| [最小请求间隔限流策略](https://www.codeseeking.com/problem/OD_1103) | 05-24 | 100分 | [充电桩最优布局规划](https://www.codeseeking.com/problem/OD_1107) | [最长递增子序列](https://leetcode.cn/problems/longest-increasing-subsequence/description/) |

### 状压、计数 & 数位问题（6 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [订单配送路径规划](https://www.codeseeking.com/problem/OD_1236) | 11-08 | 200分 | [无人机巡检航线规划](https://www.codeseeking.com/problem/OD_1191) / [云南菌子加工](https://www.codeseeking.com/problem/OD_1170) / [进化长廊展示](https://www.codeseeking.com/problem/OD_1233) | — |
| [进化长廊展示](https://www.codeseeking.com/problem/OD_1233) | 10-25 | 200分 | [无人机巡检航线规划](https://www.codeseeking.com/problem/OD_1191) / [云南菌子加工](https://www.codeseeking.com/problem/OD_1170) | — |
| [模减合并方案数](https://www.codeseeking.com/problem/OD_1226) | 10-14 | 200分 | — | — |
| [无人机巡检航线规划](https://www.codeseeking.com/problem/OD_1191) | 09-02 | 200分 | [订单配送路径规划](https://www.codeseeking.com/problem/OD_1236) / [云南菌子加工](https://www.codeseeking.com/problem/OD_1170) / [进化长廊展示](https://www.codeseeking.com/problem/OD_1233) | — |
| [云南菌子加工](https://www.codeseeking.com/problem/OD_1170) | 08-09 | 200分 | [无人机巡检航线规划](https://www.codeseeking.com/problem/OD_1191) / [最小代价完成论文评审](https://www.codeseeking.com/problem/OD_1155) / [进化长廊展示](https://www.codeseeking.com/problem/OD_1233) | — |
| [获取大写字母瓷砖拼出独特图案数量](https://www.codeseeking.com/problem/OD_1080) | 04-29 | 200分 | [受限序列重排](https://www.codeseeking.com/problem/OD_1199) | [全排列](https://leetcode.cn/problems/permutations/description/) |

### 树形、图上、概率 & 博弈问题（2 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [点亮战争迷雾](https://www.codeseeking.com/problem/OD_1179) | 08-19 | 200分 | [部门绩效汇总](https://www.codeseeking.com/problem/OD_1185) | [二叉树中的最大路径和](https://leetcode.cn/problems/binary-tree-maximum-path-sum/description/) |
| [勇攀数字高峰](https://www.codeseeking.com/problem/OD_1086) | 04-01 | 200分 | [单词搜索计数](https://www.codeseeking.com/problem/OD_1188) / [小花的AI Workflow设计](https://www.codeseeking.com/problem/OD_1228) | [不同路径](https://leetcode.cn/problems/unique-paths/description/) |

### 模拟（22 题）

| 题目 | 考期 | 分值 | 站内同类题 | 力扣 Hot100 映射 |
| :--- | :---: | :---: | :--- | :--- |
| [卡车货物装载](https://www.codeseeking.com/problem/OD_1244) | 11-15 | 100分 | — | — |
| [乘车顺序](https://www.codeseeking.com/problem/OD_1213) | 10-25 | 100分 | — | [轮转数组](https://leetcode.cn/problems/rotate-array/description/) |
| [物流运输队列调度优化](https://www.codeseeking.com/problem/OD_1227) | 10-18 | 100分 | [世界杯徽章换购](https://www.codeseeking.com/problem/OD_1207) | — |
| [物流配送路线规划](https://www.codeseeking.com/problem/OD_1225) | 10-14 | 100分 | — | — |
| [矩阵螺旋遍历与二进制特征](https://www.codeseeking.com/problem/OD_1202) | 09-16 | 100分 | [数组按二进制比特排序](https://www.codeseeking.com/problem/OD_1125) | [螺旋矩阵](https://leetcode.cn/problems/spiral-matrix/description/) |
| [数列求值](https://www.codeseeking.com/problem/OD_1195) | 09-09 | 100分 | [计算数列位置N的值](https://www.codeseeking.com/problem/OD_1085) | — |
| [快递驿站计费系统](https://www.codeseeking.com/problem/OD_1187) | 08-30 | 100分 | [计费时段计算](https://www.codeseeking.com/problem/OD_1073) / [日志文件异常检测](https://www.codeseeking.com/problem/OD_1078) | [前 K 个高频元素](https://leetcode.cn/problems/top-k-frequent-elements/description/) |
| [直线冲刺](https://www.codeseeking.com/problem/OD_1180) | 08-23 | 100分 | [少儿爬山闯关积分游戏](https://www.codeseeking.com/problem/OD_1193) | [跳跃游戏 II](https://leetcode.cn/problems/jump-game-ii/description/) |
| [灯带颜色变换](https://www.codeseeking.com/problem/OD_1169) | 08-09 | 100分 | — | [环形链表 II](https://leetcode.cn/problems/linked-list-cycle-ii/description/) |
| [基于上报数据的实时最大值](https://www.codeseeking.com/problem/OD_1160) | 07-29 | 100分 | [数据中心最佳维护时间窗](https://www.codeseeking.com/problem/OD_1211) | [滑动窗口最大值](https://leetcode.cn/problems/sliding-window-maximum/description/) |
| [路口等待时间](https://www.codeseeking.com/problem/OD_1161) | 07-29 | 200分 | [优化充电桩调度算法](https://www.codeseeking.com/problem/OD_1104) | — |
| [物流仓储多维度成本利润综合查询系统](https://www.codeseeking.com/problem/OD_1151) | 07-19 | 100分 | — | — |
| [省超足球比赛获胜队伍计算](https://www.codeseeking.com/problem/OD_1138) | 07-05 | 100分 | [分辨率排序](https://www.codeseeking.com/problem/OD_1070) / [库存补货优先级排序](https://www.codeseeking.com/problem/OD_1240) | — |
| [设计能量管理系统](https://www.codeseeking.com/problem/OD_1130) | 06-24 | 100分 | [计费时段计算](https://www.codeseeking.com/problem/OD_1073) | [合并区间](https://leetcode.cn/problems/merge-intervals/description/) |
| [网络数据包收发处理](https://www.codeseeking.com/problem/OD_1114) | 06-07 | 100分 | [配置操作失败数量统计](https://www.codeseeking.com/problem/OD_1088) | — |
| [链表数字游戏](https://www.codeseeking.com/problem/OD_1108) | 05-31 | 100分 | [区分奇偶的数组排序](https://www.codeseeking.com/problem/OD_1156) | [颜色分类](https://leetcode.cn/problems/sort-colors/description/) |
| [循环内存存取计算](https://www.codeseeking.com/problem/OD_1091) | 05-10 | 100分 | [不同Tag类型统计](https://www.codeseeking.com/problem/OD_1153) | — |
| [计费时段计算](https://www.codeseeking.com/problem/OD_1073) | 04-22 | 100分 | [快递驿站计费系统](https://www.codeseeking.com/problem/OD_1187) / [设计能量管理系统](https://www.codeseeking.com/problem/OD_1130) | — |
| [API日志去重合并统计](https://www.codeseeking.com/problem/OD_1067) | 04-15 | 100分 | [字符串压缩编码](https://www.codeseeking.com/problem/OD_1144) | — |
| [小猫钓鱼纸牌游戏](https://www.codeseeking.com/problem/OD_1068) | 04-15 | 200分 | — | — |
| [配置操作失败数量统计](https://www.codeseeking.com/problem/OD_1088) | 04-08 | 100分 | [网络数据包收发处理](https://www.codeseeking.com/problem/OD_1114) | — |
| [计算数列位置N的值](https://www.codeseeking.com/problem/OD_1085) | 04-01 | 100分 | [数列求值](https://www.codeseeking.com/problem/OD_1195) | [滑动窗口最大值](https://leetcode.cn/problems/sliding-window-maximum/description/) |

---

## 常见问题解答（FAQ）

### Q1：2026 年华为 OD 机考新题库一共有多少道题？
截至 **2026-11-15** 考期，CodeSeeking 已收录并验证 **180 道** 2026 年华为 OD 机考真题，其中 **100 分题 120 道、200 分题 60 道**，涵盖 21 个算法考点，后续新考场真题每周同步更新。

### Q2：CodeSeeking 刷题需要付费吗？
**所有题目提交评测完全免费**（包含每题 20 组严苛测试点）。同时，**考期 8 周之前的真题与老题题解全部免费**，普通用户每天还可免费使用 **3 次 AI 智能错题分析**；只有解锁近 8 周最新考期题解、不限次 AI 分析及失败测试点详细输入/输出对拍时，才需要赞助开通永久 VIP（一次开通，无需按月续费）。

### Q3：支持哪些编程语言和做题模式？
支持 **Java、C++、Python、JavaScript** 四种主流语言。题目默认采用与当前机考高度贴近的 **Core 核心代码模式**，对于需要读取复杂命令流或自定义结构的题目则提供 **ACM 模式**，并支持四语言标准解题模板与参考实现。

### Q4：本地 IDE 样例全过，但提交 OJ 报 WA（答案错误）怎么办？
华为 OD 机考常见扣分点集中在空数组/单元素边界、整数溢出、排序稳定性与多关键字次序、特殊字符分隔及死循环上限处理。建议先使用每日免费的 **AI 错题分析**定位问题代码行，或对照**失败测试点输入与期望输出**进行边界对拍。

### Q5：表格里的「同类题」和「Hot100」怎么配合使用？
如果某道 200 分真题没有思路，建议先点击右侧对应的 **力扣 Hot100** 原题掌握核心算法模型（例如`合并区间`、`课程表`、`滑动窗口最大值`等），再回到 CodeSeeking 连续完成该题及其**站内同类题**，通常 2~3 道即可吃透同一考点的变形。
