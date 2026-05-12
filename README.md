# gics-data

## [English]

### Data for GICS (Global Industry Classification Standard)

This repository provides datasets aligned with the Global Industry Classification Standard (GICS) 2023 edition. The data is ready for integration into database dictionaries, reference systems, and similar applications.
The resources are provided in two language versions: English and Simplified Chinese.

Available formats:

- CSV Comma seperated file
- MySQL table schema with data
- JSON metadata file

All files contain the same GICS classification data. Use whichever format works best for your needs.


### References

You can download the raw data at the following URLs:

https://www.msci.com/indexes/index-resources/gics

https://en.wikipedia.org/wiki/Global_Industry_Classification_Standard

https://zh.wikipedia.org/zh-cn/%E5%85%A8%E7%90%83%E8%A1%8C%E4%B8%9A%E5%88%86%E7%B1%BB%E6%A0%87%E5%87%86


### History

- Initial version: Provide GICS 2023 structure data in CSV/JSON/MySQL (en/ and zh-CN-and-en/).
- 2026-05-12:
  - Validate that the structure (code/parent/level) matches the official workbook `original-docs/GICS Map 2025.xlsx` (structure effective close of Mar 17 2023). No structure/code changes were required.
  - Update a small set of Chinese display names in `zh-CN-and-en` (only `name_cn`, codes unchanged): 2550, 3010, 4020, 6010, 301010, 402010. Sync changes across CSV/JSON/SQL.

------

## [中文说明]

### GICS数据

全球行业分类标准（GICS）是由摩根士丹利资本国际公司（MSCI）与标准普尔（S&P）于1999年共同制定的行业分类体系，旨在为全球金融行业提供统一参考。

该标准采用四级分类结构，包含11个板块（部门）、25个行业组、74个行业及163个子行业，标准普尔据此对所有主要上市公司进行归类。此体系与富时集团维护的行业分类基准（ICB）具有相似性。

GICS是标准普尔与MSCI金融领域指数产品的编制基础。每家公司的分类由其主营业务决定，逐级归属于特定子行业、行业、行业组及部门。"GICS"为麦格劳希尔金融公司与MSCI Inc.的注册商标。

如果您的系统数据只涉及到国内企业，建议使用国标：国民经济行业分类 (GB/T 4754-2017)。

这里提供的格式有：
- CSV格式
- MySQL库结构和数据
- JSON格式数据

这些数据内容相同，只是格式不同。


### 参考资料

您可以在以下地址下载到原始数据:

https://www.msci.com/indexes/index-resources/gics

https://en.wikipedia.org/wiki/Global_Industry_Classification_Standard

https://zh.wikipedia.org/zh-cn/%E5%85%A8%E7%90%83%E8%A1%8C%E4%B8%9A%E5%88%86%E7%B1%BB%E6%A0%87%E5%87%86


### 修改历史

- 初始版：提供 GICS 2023 版结构数据（四级结构），并输出 en/ 与 zh-CN-and-en/ 两套数据，格式包含 CSV/JSON/MySQL。
- 2026-05-12：
  - 依据 `original-docs/GICS Map 2025.xlsx` 进行结构核对（该表结构生效点为 2023-03-17），确认 code/parent_code/level_num 无需变更。
  - 更新 `zh-CN-and-en` 中少量中文展示名称（仅改 `name_cn`，不改 code）：2550、3010、4020、6010、301010、402010，并同步到 CSV/JSON/SQL。
