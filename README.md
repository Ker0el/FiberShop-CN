<div align="center">

# FiberShop 汉化词条库

**FiberShop 3.18.0.8 简体中文汉化 · 词条库**

459 条英中对照 · 纯文本 · 不含任何商业软件本体

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE)
[![Entries](https://img.shields.io/badge/entries-459-brightgreen.svg)](#统计)
[![Target](https://img.shields.io/badge/target-FiberShop%203.18.0.8-orange.svg)](#适用版本)

</div>

---

## 这是什么

一份 **`英文界面文本 = 中文译文`** 的对照表，用来把 FiberShop 的界面换成中文。

它只是一个词条库，不含可执行文件、不含 DLL、不含 FiberShop 的任何资源或代码。

| | |
|---|---|
| **适用版本** | FiberShop **3.18.0.8** |
| **条目数** | 459 条 |
| **文件** | [`dict/dict.txt`](dict/dict.txt) · UTF-8 |
| **覆盖面** | 菜单、面板、按钮、弹窗提示、导出流程 |

## 统计

```
文件行数      465
有效映射      459
唯一键        459
前缀匹配键      7   ← 键以 * 结尾，用来翻拼接出来的句子
重复键         0
```

## 文件格式

一行一条，**英文与中文之间是制表符（TAB）**：

```text
File	文件
Edit	编辑
```

| 规则 | 说明 |
|---|---|
| 注释 | 以 `#` 开头的整行跳过 |
| 分隔符 | **制表符**，不是等号 |
| 大小写 | **区分** —— `Normal` 是法线贴图、`normal` 是混合模式、`Shift` 是 Curl 参数里的偏移 |
| `\n` | 表示换行 |
| 键尾 `*` | **前缀匹配**，用来翻 `Export Done Successfully:   ` + 文件路径这种拼接出来的句子 |

## 数据键保护

有一批界面文字会被软件**读回去当数据用**，翻了会坏功能，词典里有意保持英文：

- 自定义输出的**通道下拉** —— 选项文字同时是着色器关键字
- **输出格式下拉** —— 选项文字同时被当文件扩展名用

## 怎么用

词条本身是纯数据，要配合配套的汉化补丁才能生效。

想自己接的话：按上面的格式把 `dict/dict.txt` 读进一张哈希表，在文本绘制前做匹配替换。
**测量和绘制要一并处理**，否则中文变宽会把控件挤到截断。

## 授权

- 译文以 **CC BY-SA 4.0** 授权，见 [LICENSE](LICENSE)：署名 · 相同方式共享 ——
  拿去卖也可以，但改过的版本要用同样的许可。
- **FiberShop 是 CGPal（www.cgpal.com）的产品**，本项目与其无任何关联。
- 本授权只覆盖译文本身。程序本体、界面英文原文都归 CGPal，详见 [NOTICE.md](NOTICE.md)。

<div align="center">
<sub>星空汉化 · <a href="https://space.bilibili.com/177308205">B 站主页</a></sub>
</div>
