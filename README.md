# 隐私政策托管说明

本目录下的页面用于托管隐私政策，推荐使用 GitHub Pages（免费、地址稳定）。

## 部署步骤

1. 把本仓库推送到 GitHub（仓库需为 public，免费版 GitHub Pages 只支持公开仓库）。
2. 仓库主页 → Settings → Pages → Build and deployment → Source 选择 **Deploy from a branch**，Branch 选 `main`，目录选 `/docs`，保存。
3. 等 1–2 分钟，即可通过以下地址访问：
   - 中文版：`https://<你的用户名>.github.io/<仓库名>/privacy-policy/`
   - 英文版：`https://<你的用户名>.github.io/<仓库名>/privacy-policy/en.html`
4. 把实际地址填回代码中的 `app/src/main/java/com/jieduan/app/AppConfig.kt`（`PRIVACY_POLICY_URL`），重新打包。
5. 在 Play Console 的“数据安全表单 / 商店信息”中填入同一 URL。

## 注意

- 页面内容与 `docs/隐私政策_zh.md`、`docs/privacy_policy_en.md` 同步维护；改文案时两边一起改。
- 托管地址一旦对外公开，就不要再改动 URL 本身（内容更新没问题）。
