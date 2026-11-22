<p align="center">
  <img src="assets/banner.svg" alt="Terminal: datashield --about — DataShield Lightweight Labs. Practical privacy, security and AI-safety tools for everyday developers. Five live projects." width="100%" />
</p>

<p align="center">
  <img src="https://img.shields.io/github/last-commit/liuxiaomingskm/datashield-lightweight-labs?style=flat&color=30363d&labelColor=0d1117&label=last%20commit" alt="Last commit" />
  <img src="https://img.shields.io/github/commit-activity/m/liuxiaomingskm/datashield-lightweight-labs?style=flat&color=30363d&labelColor=0d1117&label=activity" alt="Commit activity" />
  <img src="https://img.shields.io/github/license/liuxiaomingskm/datashield-lightweight-labs?style=flat&color=30363d&labelColor=0d1117" alt="License" />
  <img src="https://img.shields.io/github/stars/liuxiaomingskm/datashield-lightweight-labs?style=flat&color=30363d&labelColor=0d1117" alt="Stars" />
  <img src="https://img.shields.io/badge/next.js-11-30363d?style=flat&labelColor=0d1117&logo=nextdotjs&logoColor=white" alt="Next.js 11" />
  <img src="https://img.shields.io/badge/mdx-1.6-30363d?style=flat&labelColor=0d1117&logo=mdx&logoColor=white" alt="MDX" />
  <img src="https://img.shields.io/badge/tailwind-2-30363d?style=flat&labelColor=0d1117&logo=tailwindcss&logoColor=38bdf8" alt="Tailwind CSS 2" />
</p>

<p align="center">
  <code>about</code> · <a href="#02--projects"><code>projects</code></a> · <a href="#03--privacy-guide"><code>privacy-guide</code></a> · <a href="#04--run-it"><code>run-it</code></a> · <a href="#05--roadmap"><code>roadmap</code></a> · <a href="#06--contribute"><code>contribute</code></a>
</p>

---

## 01 · about

> **Privacy shouldn't be a barrier — it should be built in.**

DataShield Lightweight Labs is an open-source initiative for **small, sharp tools** that make data privacy, application security and AI safety easier to get right. No platforms, no sign-ups, no lock-in. Just utilities a developer can read in one sitting and adopt in an afternoon.

```yaml
focus:
  ai-privacy-and-safety:
    - stop PII from leaking into LLM prompts
    - redaction pipelines for model inputs and outputs
    - privacy-preserving middleware for generative-AI workflows
  application-security:
    - open-source security scanners
    - misconfiguration detection for cloud and databases
    - threat-modeling templates and tooling
  compliance-and-risk:
    - developer-first tooling aligned with GDPR, CCPA and SOC 2
    - data-minimization utilities
    - consent and data-lifecycle tracking
principles: [lightweight, transparent, local-first, open-source]
```

## 02 · projects

DataShield Lightweight Labs is the hub. Each project below was **developed under the initiative** and carries it into a different industry.

```text
datashield-lightweight-labs ··· initiative hub
│
├── tools ─────────────── enforce privacy in code
│   ├── ai-privacy-guardrail ............ AI / LLM
│   ├── medredact ....................... healthcare
│   └── cloud-sec-auditor ............... cloud & SaaS
│
├── knowledge ─────────── teach AI agents compliance
│   └── privacy-data-protection-skills .. GDPR · HIPAA · EU AI Act · +14 more
│
└── education
    └── privacy-guide ................... this repository
```

```diff
+ [live]  ai-privacy-guardrail            AI / LLM      Redact PII & secrets before prompting, restore them in the reply
+ [live]  medredact                       healthcare    De-identify clinical notes against HIPAA's 18 Safe Harbor identifiers
+ [live]  cloud-sec-auditor               cloud / SaaS  Grade AWS · GCP · Azure configs for public exposure, with CIS fixes
+ [live]  privacy-data-protection-skills  compliance    282 structured privacy skills AI agents load on demand
+ [live]  privacy-guide                   education     Next.js + MDX guide to staying private online
! [next]  finance pack                    finance       PCI DSS / GLBA checks for payment and banking data
```

| project | industry | what it does | links |
|---|---|---|---|
| **AI Privacy Guardrail** | 🤖 AI / LLM | Turns `jane@acme.com` into `[EMAIL_1]` before it reaches a model, and back again after | [repo](https://github.com/liuxiaomingskm/AI-Privacy-Guardrail) · [demo](https://liuxiaomingskm.github.io/AI-Privacy-Guardrail/) |
| **MedRedact** | 🏥 healthcare | Auto-detects 15 of HIPAA's 18 Safe Harbor identifier types (names, MRNs, dates…); date shifting; re-identifies AI replies | [repo](https://github.com/liuxiaomingskm/MedRedact) · [demo](https://liuxiaomingskm.github.io/MedRedact/) |
| **cloud-sec-auditor** | ☁️ cloud & SaaS | Audits Terraform plans and CLI exports; letter grade, 24 rules, SARIF for CI | [repo](https://github.com/liuxiaomingskm/cloud-sec-auditor) · [demo](https://liuxiaomingskm.github.io/cloud-sec-auditor/#demo) |
| **Privacy & Data Protection Skills** | ⚖️ compliance | 282 agentskills.io skills across GDPR, CCPA, HIPAA, EU AI Act, PIPL and more, extending mukul975's open-source skills library | [repo](https://github.com/zecongyu/Privacy-Data-Protection-Skills) |
| **Privacy guide** | 📖 education | The website in this repository | [details ↓](#03--privacy-guide) |

**Building under the initiative?** Add the badge to your README:

[![Developed under the DataShield Lightweight Labs initiative](https://img.shields.io/badge/%F0%9F%9B%A1%EF%B8%8F%20DataShield%20Lightweight%20Labs-initiative%20project-4f46e5?style=flat-square)](https://github.com/liuxiaomingskm/datashield-lightweight-labs)

```markdown
[![Developed under the DataShield Lightweight Labs initiative](https://img.shields.io/badge/%F0%9F%9B%A1%EF%B8%8F%20DataShield%20Lightweight%20Labs-initiative%20project-4f46e5?style=flat-square)](https://github.com/liuxiaomingskm/datashield-lightweight-labs)
```

## 03 · privacy-guide

This repo builds a static site that publishes **《如何在网络中保护隐私》** (*How to Protect Your Privacy Online*), a hands-on, Chinese-language guide.

> [!NOTE]
> Guide written by **[KallyDev](https://github.com/kallydev) and the community** (Oct 2021), as credited in the article's byline. It's hosted here as part of the lab's privacy-education resources.

```text
如何在网络中保护隐私
├── 网络隐私的定义 ............ what privacy is (vs. anonymity)
├── 隐私泄漏的危害 ............ what leaked data is used for
├── 检查隐私泄漏情况 .......... Firefox Monitor, Have I Been Pwned
├── 防范隐私泄漏的方法
│   ├── 使用开源浏览器 ........ open-source browsers
│   ├── 增强你的浏览器 ........ tracker-blocking extensions
│   ├── 使用开源输入法 ........ open-source input methods
│   ├── 使用虚拟机 ............ sandbox untrusted apps in a VM
│   ├── 拒绝上传非必要信息 .... refuse unnecessary data collection
│   ├── 避免使用人脸识别 ...... avoid face recognition
│   ├── 关闭邮箱和手机号搜索 .. hide your email and phone from search
│   ├── 检查应用权限 .......... audit app permissions
│   └── 给图片打码和添加水印 .. blur and watermark shared images
└── 保护隐私的意义 ............ why it matters
```

**How the site is put together**

```text
posts/index.mdx ──► pages/index.tsx ──► next build ──► next export ──► ./out (static HTML)
   (content)          (layout + Disqus)                     │
                                                            └──► next-sitemap: sitemap.xml + robots.txt
styles: Tailwind CSS 2 + styles/markdown.css
```

## 04 · run-it

> [!IMPORTANT]
> Next.js 11 needs **Node.js 14–16**. With newer Node versions, switch first, for example `nvm use 16`.

```console
$ git clone https://github.com/liuxiaomingskm/datashield-lightweight-labs.git
$ cd datashield-lightweight-labs
$ yarn install
$ yarn dev
  ready - started server on http://localhost:3000
```

**Static deploy**

```console
$ export SITE_URL=https://your-domain.example              # sitemap + robots.txt
$ export NEXT_PUBLIC_SITE_URL=https://your-domain.example  # Disqus thread URL
$ export NEXT_PUBLIC_SITE_TITLE="Privacy Guide"
$ yarn deploy                                              # → ./out
```

Upload `./out` to GitHub Pages, Netlify, Vercel or Cloudflare Pages.

| command | does |
|---|---|
| `yarn dev` | dev server with hot reload |
| `yarn build` | production build |
| `yarn start` | serve the production build |
| `yarn lint` | ESLint via `next lint` |
| `yarn deploy` | sitemap → build → static export |

```text
.
├── pages/            _app.tsx · _document.tsx · index.tsx (guide + comments)
├── posts/            index.mdx (the guide)
├── styles/           globals.css · markdown.css
├── public/           static assets
├── assets/           README artwork
├── next.config.js    MDX support
└── next-sitemap.js   sitemap / robots.txt
```

## 05 · roadmap

- [x] Privacy guide site (Next.js + MDX)
- [x] `ai-privacy-guardrail`: client-side PII and secret redaction for LLM prompts
- [x] `medredact`: HIPAA Safe Harbor de-identification for clinical text
- [x] `cloud-sec-auditor`: multi-cloud misconfiguration scanner (web + CLI)
- [x] `privacy-data-protection-skills`: privacy-compliance skills for AI agents
- [ ] Finance pack: PCI DSS / GLBA checks for payment and banking data
- [ ] Server-side redaction middleware for LLM pipelines
- [ ] Data-minimization and consent-tracking utilities
- [ ] English edition of the privacy guide

## 06 · contribute

```console
$ git checkout -b feat/your-idea
$ git commit -m "feat: something that makes data a little safer"
$ git push origin feat/your-idea   # then open a pull request
```

Bug, idea or a tool you wish existed? **[Open an issue](https://github.com/liuxiaomingskm/datashield-lightweight-labs/issues).** Small, focused PRs are easiest to review.

---

<p align="center">
  <sub><a href="LICENSE">MIT License</a> · built one line of code at a time · <b>⭐ star the repo if it's useful</b></sub>
</p>
