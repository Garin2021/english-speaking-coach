# English Speaking Coach · 英文口语教练

一个 agent skill：每天 5 分钟英文口语纠错。输入是中英混杂的口语文本（英文为主，想不起来的词用中文占位），输出「问题诊断」+「修正后的完整版本」。

An agent skill for a daily 5-minute English speaking practice. Input: mixed Chinese–English speaking text (mostly English, with Chinese placeholders for forgotten words). Output: an issue-by-issue diagnosis plus a fully corrected, natural spoken-English version.

## 文件结构 / Structure

```
english-speaking-coach/
├── SKILL.md                    # 主流程 / main workflow
├── references/
│   └── common-errors.md        # 中文母语者常见口语错误速查 / common error cheat sheet
└── README.md
```

## 用法 / Usage

1. 把整个文件夹放进你的 agent 的 skills 目录。 Put this folder into your agent's skills directory.
2. 对它说“学英文”，然后贴上你的口语文本。 Say “学英文” (or ask for speaking correction) and paste your text.

## 可选：飞书归档 / Optional: Feishu archiving

SKILL.md 默认会把每轮练习插到一篇飞书文档顶部，并支持每周复盘。使用前请把 `<YOUR_FEISHU_DOC_URL>` 替换成你自己的文档链接；该功能依赖已登录的 `lark-cli`。不需要的话，删掉 SKILL.md 里的「第五步」和「每周复盘」即可。

By default the skill archives each session to the top of a Feishu (Lark) doc and supports a weekly review. Replace `<YOUR_FEISHU_DOC_URL>` with your own doc URL; this requires an authenticated `lark-cli`. If you don't need it, remove “第五步” and “每周复盘” from SKILL.md.
