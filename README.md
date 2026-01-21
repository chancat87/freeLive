# freeLive

[![Stars](https://img.shields.io/github/stars/Ruk1ng001/freeLive)](https://github.com/Ruk1ng001/freeLive/stargazers)
[![Release](https://img.shields.io/github/v/release/Ruk1ng001/freeLive)](https://github.com/Ruk1ng001/freeLive/releases)
[![License](https://img.shields.io/github/license/Ruk1ng001/freeLive)](https://github.com/Ruk1ng001/freeLive/blob/main/LICENSE)
[![TG](https://img.shields.io/badge/Telegram-群组-blue?logo=Telegram)](https://t.me/Ruk1ng001)

### 🎬 直播源聚合服务 | 斗鱼 · 虎牙 · B站 · YouTube

> 直播源地址每 30 分钟自动更新，支持 FLV / HLS 双模式

[<img src="https://api.gitsponsors.com/api/badge/img?id=779725311" height="90">](https://api.gitsponsors.com/api/badge/link?p=UzxWE0/Sr257rDsDOuSqJybSqPcdqpjHYJR0q6o44Hd1s2+cDhmwJ1g71rFRC1LH52MmKxi6BK9cFmnqazFVAuG4tVdTOfyJv9R4qlN+XVOnQGwG7eU1aDgQHALuEmhnodpPykVztqQr9YVEgkauCg==)

---

## 📢 社区

| 渠道 | 链接 |
|:---:|:---:|
| Telegram 频道 | [t.me/Ruk1ng001](https://t.me/Ruk1ng001) |
| Telegram 交流群 | [点击加入](https://t.me/+-e-b04EE5Cw2NmU1) |

---

## ☕ 打赏支持

| 支付宝 | 微信 |
|:---:|:---:|
| ![支付宝](FUNDING/支付宝.png) | ![微信](FUNDING/微信.png) |

---

## 🌐 服务线路

| 线路 | 地址 | 状态 |
|:---:|------|:---:|
| 家宽线路 | `http://live.997269.xyz:19527` | ✅ |

> 💡 访问根地址可打开 [**可视化配置页面**](http://live.997269.xyz:19527)，无需手动拼接 URL

---

## 🚀 快速开始

### 获取直播源

| 格式 | 地址 |
|------|------|
| M3U | `http://live.997269.xyz:19527/lives/all.m3u` |
| TXT | `http://live.997269.xyz:19527/lives/all.txt` |
| M3U (HLS) | `http://live.997269.xyz:19527/lives/all.m3u?hls=1` |

### 平台代号

| 平台 | 代号 | 图标 |
|:---:|:---:|:---:|
| 斗鱼 | `douyu` | 🐠 |
| 虎牙 | `huya` | 🐯 |
| B站 | `bili` | 📺 |
| YouTube | `youtube` | ▶️ |

---

## 📖 URL 格式说明

### 基础格式

```
/lives/{平台}.{格式}
```

### 示例

```bash
# 全部平台
/lives/all.m3u

# 单平台
/lives/douyu.m3u
/lives/bili.txt

# 多平台组合（下划线连接）
/lives/douyu_huya.m3u
/lives/bili_huya_douyu.m3u
```

---

## ⚙️ 高级参数

### 流媒体协议

| 参数 | 模式 | 延迟 | 适用场景 |
|:---:|:---:|:---:|------|
| 默认 | FLV | 2-5秒 | PC播放器、追求低延迟 |
| `?hls=1` | HLS | 5-15秒 | iOS/Safari、IPTV盒子、长时间观看 |

```bash
# FLV 模式（默认）
/lives/all.m3u

# HLS 模式
/lives/all.m3u?hls=1
```

### 分类筛选

```bash
# 筛选单平台分类
/lives/douyu.m3u?douyu=赛事_一起看

# 筛选多平台分类
/lives/douyu_bili.m3u?douyu=赛事&bili=生活_娱乐

# 组合使用
/lives/huya_bili.m3u?hls=1&huya=一起看&bili=赛事
```

### 支持的分类

<details>
<summary><b>🐠 斗鱼</b></summary>

赛事、一起看、人文社科、户外、数码科技、美食、英雄联盟、王者荣耀、三角洲行动、和平精英、云顶之弈、DOTA2、穿越火线、CSGO、地下城与勇士、炉石传说、绝地求生、永劫无间、金铲铲之战、原神、崩坏3、明日方舟、单机热游、主机游戏、黑神话悟空、我的世界、纪录片、萌宠、星秀、音乐、颜值、欢乐麻将、棋牌、象棋

</details>

<details>
<summary><b>🐯 虎牙</b></summary>

英雄联盟、王者荣耀、三角洲行动、DOTA2、穿越火线、CS2、吃鸡、和平精英、无畏契约、云顶之弈、地下城与勇士、炉石传说、永劫无间、魔兽世界、金铲铲之战、原神、绝区零、鸣潮、崩坏星穹铁道、蛋仔派对、DNF手游、英雄联盟手游、单机热游、主机游戏、黑神话悟空、我的世界、艾尔登法环、恐怖游戏、一起看、原创、体育、户外、吃喝玩乐、星秀、颜值、音乐、交友、科技、旅游、二次元、虚拟偶像、中国象棋、欢乐斗地主、欢乐麻将、掼蛋、狼人杀、鹅鸭杀

</details>

<details>
<summary><b>📺 B站</b></summary>

网游、英雄联盟、无畏契约、守望先锋、最终幻想14、绝地求生、逃离塔科夫、CS2、DOTA2、永劫无间、云顶之弈、DNF、三角洲行动、手游、王者荣耀、原神、崩坏星穹铁道、和平精英、明日方舟、绝区零、金铲铲之战、蛋仔派对、单机、主机游戏、独立游戏、黑神话悟空、我的世界、怪物猎人、艾尔登法环、饥荒、恐怖游戏、娱乐、视频唱见、萌宠、互动玩法、美食、生活、户外、手工、日常、虚拟主播、虚拟Singer、虚拟日常、赛事、知识、社会观察、教育学习、科技科学、电台

</details>

<details>
<summary><b>▶️ YouTube</b></summary>

游戏、体育、新闻、正在直播、音乐

</details>

---

## 📊 平台支持情况

| 平台 | FLV | HLS | 备注 |
|:---:|:---:|:---:|------|
| 斗鱼 | ✅ | ⚠️ | 部分房间自动回退 FLV |
| 虎牙 | ✅ | ✅ | 完美支持 |
| B站 | ✅ | ✅ | 完美支持 |
| YouTube | ✅ | ❌ | 需设备使用代理 |

---

## 📋 常用地址速查

| 用途 | 地址 |
|------|------|
| 全部直播 | `/lives/all.m3u` |
| 全部直播 (HLS) | `/lives/all.m3u?hls=1` |
| 国内平台 | `/lives/douyu_huya_bili.m3u` |
| 国内平台 (HLS) | `/lives/douyu_huya_bili.m3u?hls=1` |
| 仅B站 (HLS) | `/lives/bili.m3u?hls=1` |
| 斗鱼赛事 | `/lives/douyu.m3u?douyu=赛事` |
| 虎牙一起看 | `/lives/huya.m3u?huya=一起看` |

---

## ❓ 常见问题

<details>
<summary><b>播放一段时间后断流？</b></summary>

使用 HLS 模式：在 URL 后添加 `?hls=1`

</details>

<details>
<summary><b>iOS / Safari 无法播放？</b></summary>

iOS 不支持 FLV 格式，请使用 HLS 模式：`?hls=1`

</details>

<details>
<summary><b>YouTube 无法播放？</b></summary>

YouTube 需要设备开启代理才能访问

</details>

<details>
<summary><b>某个直播间打不开？</b></summary>

可能主播已下播，直播源每 30 分钟更新一次

</details>

<details>
<summary><b>HLS 延迟比较高？</b></summary>

HLS 延迟约 5-15 秒，追求低延迟请使用 FLV 模式（默认）

</details>

<details>
<summary><b>斗鱼 HLS 失败？</b></summary>

斗鱼部分房间不支持 HLS，系统会自动回退到 FLV

</details>

---

## 📈 Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Ruk1ng001/freeLive&type=Date)](https://star-history.com/#Ruk1ng001/freeLive&Date)

---

## 📝 更新日志

| 版本 | 更新内容 |
|------|----------|
| v1.2 | ✨ 新增可视化配置页面 |
| v1.1 | ✨ 支持 HLS 流媒体模式 |
| v1.0 | 🎉 首次发布 |
