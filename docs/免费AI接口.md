# 免费 AI 接口实测（国内外）

> 本表是 2026-11-24 在本机实测的连通性结果，不是抄来的清单。
> 判定：HTTPS 根路径返回码。200/401/404 = 可达（404 只是根路径无内容）；403 = 被 WAF 或地区策略拦；000 = 连不上。

## 实测结果

| 平台 | 接口域名 | 实测 | 免费额度 | 注册 |
|---|---|---|---|---|
| 智谱 GLM | open.bigmodel.cn | 200 可达 | glm-4-flash 长期免费；注册需手机号 | https://open.bigmodel.cn |
| 硅基流动 | api.siliconflow.cn | 404 可达 | 多个开源模型免费额度；注册送额度 | https://cloud.siliconflow.cn |
| Moonshot | api.moonshot.cn | 200 可达 | 新用户赠额度；长上下文见长 | https://platform.moonshot.cn |
| OpenRouter | openrouter.ai | 200 可达 | 聚合平台，含 :free 模型 | https://openrouter.ai |
| 火山方舟 | ark.cn-beijing.volces.com | 401 可达 | 豆包系列，新用户有赠送额度 | https://console.volcengine.com/ark |
| 阿里百炼 | dashscope.aliyuncs.com | 404 可达 | 通义千问，新用户免费额度 | https://bailian.console.aliyun.com |
| 百度千帆 | qianfan.baidubce.com | 404 可达 | 文心系列，有免费额度 | https://qianfan.cloud.baidu.com |
| 阶跃星辰 | api.stepfun.com | 404 可达 | step 系列，注册送额度 | https://platform.stepfun.com |
| MiniMax | api.minimax.chat | 301 可达 | abab 系列，有免费额度 | https://platform.minimaxi.com |
| 腾讯混元 | hunyuan.tencentcloudapi.com | 200 可达 | hunyuan-lite 有免费额度 | https://cloud.tencent.com/product/hunyuan |
| Groq | api.groq.com | 403 被拦 | 速度快但国内直连受限 | https://console.groq.com |
| Cerebras | api.cerebras.ai | 403 被拦 | 推理极快，国内不可直连 | https://cloud.cerebras.ai |
| Together | api.together.xyz | 403 被拦 | 开源模型托管 | https://api.together.xyz |
| Cohere | api.cohere.com | 403 被拦 | 有免费试用额度 | https://dashboard.cohere.com |
| Anthropic | api.anthropic.com | 403 被拦 | Claude 系列 | https://console.anthropic.com |
| OpenAI | api.openai.com | 000 不通 | 需代理 | https://platform.openai.com |
| Mistral | api.mistral.ai | 000 不通 | 需代理 | https://console.mistral.ai |
| Google Gemini | generativelanguage.googleapis.com | 000 不通 | 有免费额度但需代理 | https://aistudio.google.com |
| 讯飞星火 | spark-api.xf-yun.com | 403 被拦 | 有免费额度 | https://xinghuo.xfyun.cn |

## 结论：国内直连可用 10 家

能直接用的：智谱、硅基流动、Moonshot、OpenRouter、火山方舟、阿里百炼、百度千帆、阶跃星辰、MiniMax、腾讯混元。

被拦的：Groq、Cerebras、Together、Cohere、Anthropic、讯飞星火（403）；OpenAI、Mistral、Gemini（000）。

## 推荐顺序

| 排名 | 平台 | 为什么 |
|---|---|---|
| 1 | 智谱 GLM | glm-4-flash 长期免费，注册只要手机号，OpenAI 兼容 |
| 2 | 硅基流动 | 免费模型多，注册送额度，OpenAI 兼容 |
| 3 | Moonshot | 长上下文强，赠额够用一阵 |
| 4 | OpenRouter | 一个 key 打通几十家，含免费模型 |

## 怎么接进 OpenClaw

拿到 key 后写入 models.providers，并把两处指向免费模型：

    agents.defaults.utilityModel      // 摘要/分类等小任务
    agents.defaults.compaction.model  // 上下文压缩

日常开销从付费模型转到免费额度，主对话仍保留 DeepSeek。

## 注意

1. 免费额度都有速率限制（每分钟/每天），跑批量任务会撞墙。
2. 长期免费以厂商官网当前政策为准；本表只记录实测连通性。
3. 部分平台需实名认证才能领额度。
4. 不要把 key 写进仓库；OpenClaw 支持 SecretRef，我会用引用方式保存。

_实测日期：2026-11-24_