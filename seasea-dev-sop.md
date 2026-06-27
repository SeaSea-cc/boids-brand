# seasea-dev 账号设置 + 接入 WorkBuddy 操作手册
# seasea-dev Account Setup & WorkBuddy Integration SOP

> **文档版本 / Document Version**: v1.0
> **最后更新 / Last Updated**: 2026-06-28
> **维护人 / Maintainer**: Aaron (@aaronwz0)
> **适用范围 / Scope**: SeaSea-cc 组织内所有需要 AI 协同的仓库
> **状态 / Status**: Active — seasea-dev 账号已创建(dev@seasea.cc),已加入 SeaSea-cc 组织并获得所有相关项目权限

---

## 目录 / Table of Contents

1. [背景与目标 / Background & Goals](#1-背景与目标--background--goals)
2. [角色定位 / Role Definition](#2-角色定位--role-definition)
3. [前置条件 / Prerequisites](#3-前置条件--prerequisites)
4. [Step 1 — 创建 seasea-dev 账号 / Create the Dev Account](#step-1--创建-seasea-dev-账号--create-the-dev-account)
5. [Step 2 — 加入组织与仓库授权 / Add to Org & Repos](#step-2--加入组织与仓库授权--add-to-org--repos)
6. [Step 3 — 生成 Fine-grained PAT / Generate Token](#step-3--生成-fine-grained-pat--generate-token)
7. [Step 4 — 接入 WorkBuddy / Integrate with WorkBuddy](#step-4--接入-workbuddy--integrate-with-workbuddy)
8. [Step 5 — 协同工作流 / Collaboration Workflow](#step-5--协同工作流--collaboration-workflow)
9. [权限矩阵 / Permission Matrix](#6-权限矩阵--permission-matrix)
10. [安全与回收 / Security & Rotation](#7-安全与回收--security--rotation)
11. [故障排查 / Troubleshooting](#8-故障排查--troubleshooting)
12. [FAQ](#9-faq)

---

## 1. 背景与目标 / Background & Goals

### 中文

SeaSea 集团正在多项目中引入 WorkBuddy(云端 AI Agent)进行代码协同,涉及 seasea-main、seasea-gtm-os、boids-brand 等仓库。直接使用个人账号(aaronwz0)的 token 给 AI 使用存在以下风险:

- **权限过宽**:个人 token 通常可访问所有仓库,泄漏影响面大
- **追溯困难**:AI 生成的 commit/PR 与人工操作混在一起,难以审计
- **回收不便**:临时 token 散落各处,过期管理混乱

**目标**:建立独立的 `seasea-dev` 开发账号,以最小权限原则接入 WorkBuddy,实现安全、可追溯、可回收的 AI 协同。

### English

SeaSea Group is introducing WorkBuddy (a cloud-based AI Agent) for code collaboration across multiple repositories including seasea-main, seasea-gtm-os, and boids-brand. Using personal account tokens (aaronwz0) directly for AI access carries these risks:

- **Over-privileged**: Personal tokens often access all repos, magnifying breach impact
- **Poor traceability**: AI-generated commits/PRs mix with human work, hard to audit
- **Messy rotation**: Ad-hoc tokens scatter around, expiry management is chaotic

**Goal**: Establish a dedicated `seasea-dev` dev account with least-privilege access for WorkBuddy, enabling secure, traceable, and rotatable AI collaboration.

---

## 2. 角色定位 / Role Definition

| 维度 / Dimension | 说明 / Description |
|---|---|
| **账号类型 / Account Type** | GitHub 用户账号(User Account),非 GitHub App,非 Deploy Key |
| **身份性质 / Identity** | 开发账号(Dev Identity),由团队共同拥有,非个人归属 |
| **显示名 / Display Name** | `seasea-dev` |
| **邮箱 / Email** | `dev@seasea.cc` |
| **头像 / Avatar** | 建议使用 SeaSea 品牌 dev 图标,便于在 PR/Commit 列表中识别 |
| **职责 / Responsibilities** | 接收 WorkBuddy 的 git 操作(clone/push/PR),执行 CI 触发,提交 AI 生成代码 |
| **禁止行为 / Prohibited** | 不得拥有 Admin 权限;不得直接 merge 到 main;不得访问非授权仓库 |

> **为什么用 User Account 而不是 GitHub App?**
> Why User Account instead of GitHub App?
>
> WorkBuddy 当前的 git 操作基于 `gh` CLI + PAT 模式,User Account + fine-grained PAT 最简单直接,无需额外开发 OAuth 流程。后续若引入更多自动化,可再迁移到 GitHub App。
> WorkBuddy's git operations use `gh` CLI + PAT pattern. User Account + fine-grained PAT is simplest, no OAuth dev needed. Migrate to GitHub App later if automation grows.

---

## 3. 前置条件 / Prerequisites

执行本 SOP 前,需确认:

- [ ] 你拥有 SeaSea-cc 组织的 **Owner** 权限 / You have **Owner** role in SeaSea-cc org
- [ ] 已确认要接入 WorkBuddy 的仓库清单 / Confirmed list of repos to integrate
- [ ] 已阅读 WorkBuddy 协同机制(单会话独占、teammate 共享 `/workspace`)/ Read WorkBuddy collaboration model
- [ ] seasea-dev 账号已创建并加入 SeaSea-cc 组织 / seasea-dev account created and joined SeaSea-cc org

---

## Step 1 — 确认 seasea-dev 账号 / Verify the Dev Account

> ✅ **已完成**:seasea-dev 账号已通过 `dev@seasea.cc` 邮箱创建,并已加入 SeaSea-cc 组织。
> ✅ **Done**: seasea-dev account has been created via `dev@seasea.cc` and joined SeaSea-cc org.

### 1.1 账号信息确认 / Account Info Verification

确认以下信息已到位:

**账号信息 / Account Info**:
- Username: `seasea-dev`
- Email: `dev@seasea.cc`
- 密码: 存入团队密码管理器(1Password / Bitwarden),**不要告知个人**
- 2FA: **必须开启**,密钥备份到密码管理器 / **Mandatory**, backup recovery codes

### 1.2 完善账号基础设置

登录 seasea-dev 后,在 Settings 中确认:

- [ ] 上传 SeaSea 品牌 dev 头像 / Upload brand dev avatar
- [ ] 设置 Bio: `Dev account for WorkBuddy AI collaboration. Maintained by SeaSea dev team.`
- [ ] 开启 2FA(TOTP)/ Enable 2FA (TOTP)
- [ ] 保存 recovery codes 到密码管理器

> ⚠️ **不要给 seasea-dev 账号添加任何 SSH key**,后续只用 PAT。
> **Do NOT add SSH keys to seasea-dev account**, PAT only.

---

## Step 2 — 确认组织与仓库授权 / Verify Org & Repo Permissions

> ✅ **已完成**:seasea-dev 已加入 SeaSea-cc 组织,并获得所有相关项目权限。
> ✅ **Done**: seasea-dev has joined SeaSea-cc org and obtained all relevant project permissions.

### 2.1 确认组织成员身份 / Verify Org Membership

登录 seasea-dev,确认在 `github.com/orgs/SeaSea-cc/people` 中可以看到 `seasea-dev`,角色为 **Member**(不要给 Owner)。

如需后续新增成员,组织 Owner 可操作:

**Web UI 路径**: `SeaSea-cc` → `People` → `Invite member` → 输入 `seasea-dev` → 角色选 **Member**

**CLI 路径 / CLI alternative**(需 Owner 本地用 gh):
```bash
gh api --method POST orgs/SeaSea-cc/memberships \
  -f username=seasea-dev \
  -f role=member
```

### 2.2 确认仓库级权限 / Verify Repo-level Permissions

确认 seasea-dev 在各目标仓库拥有适当权限。当前 seasea-dev 已获得所有相关项目权限,后续新增仓库时按以下方式授权:

逐仓库授权(不要给组织级 Write 权限,会波及所有仓库):

**Web UI**: 仓库 → `Settings` → `Collaborators` → `Add people` → `seasea-dev` → 权限选 `Write`

**CLI 批量授权 / CLI batch**:
```bash
# 仓库清单 / Repo list
REPOS=("seasea-main" "seasea-gtm-os" "boids-brand")

for repo in "${REPOS[@]}"; do
  gh api --method PUT repos/SeaSea-cc/$repo/collaborators/seasea-dev \
    -f permission=write
  echo "✓ Granted Write on $repo"
done
```

> **为什么是 Write 而不是 Maintain/Triage?**
> WorkBuddy 需要 push 分支、开 PR、触发 CI,Write 是最低满足权限。Maintain 无法 push,Triage 无法 push 代码。
> WorkBuddy needs to push branches, open PRs, trigger CI. Write is the minimum sufficient. Maintain can't push, Triage can't push code.

---

## Step 3 — 生成 Fine-grained PAT / Generate Token

> 🔑 **这是唯一需要手动操作的步骤**。账号已创建、组织已加入,接下来只需生成 token。

### 3.1 为什么要 Fine-grained PAT

Classic token 一旦泄漏,影响该账号所有授权仓库。Fine-grained PAT 可限定:

- 仓库范围(只列需要的几个)/ Repo scope
- 权限细粒度(只读/读写分开)/ Granular permissions
- 过期时间(强制 30 天)/ Forced expiry

### 3.2 直接链接生成(推荐)/ Direct Link Generation

> 💡 **直接用下面的链接,免去手动导航。**
> **Use the direct links below to skip manual navigation.**

**1. 登录 seasea-dev 账号 / Log in to seasea-dev**

👉 https://github.com/login

使用 `dev@seasea.cc` 邮箱 + 密码登录。

**2. 打开 Fine-grained Token 生成页 / Open token generation page**

👉 https://github.com/settings/personal-access-tokens/new?fine_grained=true

> 📸 **截图位 Screenshot 1**: 登录后看到的 token 生成页面,截图存档以备新成员参考。

**3. 填写配置 / Fill Configuration**

| 字段 / Field | 值 / Value | 备注 / Notes |
|---|---|---|
| **Token name** | `workbuddy-cloud-sandbox` | 便于识别用途 |
| **Expiration** | **30 days** | ⏰ 2026-07-28 过期,到期前 7 天轮换 |
| **Description** | `WorkBuddy cloud sandbox access for SeaSea-cc repos` | 可选,方便审计 |
| **Resource owner** | `SeaSea-cc` | ⚠️ 必须选组织,不要选 seasea-dev 个人 |
| **Repository access** | **Only select repositories** | ⚠️ 不要选 All repositories |

点击 "Only select repositories" 后,逐个勾选:

> 📸 **截图位 Screenshot 2**: 仓库选择界面,确保只勾选需要的仓库。

| 勾选 / Select | 说明 |
|---|---|
| ☑️ `seasea-main` | 主仓库 |
| ☑️ `seasea-gtm-os` | GTM 埋点 |
| ☑️ `boids-brand` | Boids 品牌 skill |
| ☐ 其他仓库 | 不勾选,后续需要时再加 |

**4. 配置权限 / Configure Permissions**

展开 "Repository permissions" 区域,按以下表格逐一设置:

> 📸 **截图位 Screenshot 3**: 权限配置完成后的界面,确认每项级别正确。

| 权限 / Permission | 级别 / Level | 操作 / How to set | 用途 / Purpose |
|---|---|---|---|
| **Contents** | Read and write | 下拉选 "Read and write" | clone / push / commit |
| **Metadata** | Read-only | 默认值,不需改 | GitHub 强制要求 |
| **Pull requests** | Read and write | 下拉选 "Read and write" | 开 PR / 评论 PR |
| **Workflows** | Read and write | 下拉选 "Read and write" | 触发 CI workflow |
| **Actions** | Read-only | 下拉选 "Read-only" | 查看 CI 运行结果 |
| **Issues** | Read and write | 下拉选 "Read and write" | 创建/评论 issue |
| **Commit statuses** | Read-only | 下拉选 "Read-only" | 查看检查状态 |
| **Administration** | No access | ⚠️ 确保不选 | 禁止 |
| **Webhooks** | No access | ⚠️ 确保不选 | 禁止 |
| **Secrets** | No access | ⚠️ 确保不选 | 禁止 |

**5. 生成 token / Generate**

点击页面底部绿色按钮 **"Generate token"**。

> 📸 **截图位 Screenshot 4**: token 生成成功页面(只显示一次!),立即复制。

### 3.3 安全保存 token / Save Token Securely

token 生成后 **只显示一次**,立即复制并存入团队密码管理器:

```
Entry: seasea-dev / workbuddy-cloud-sandbox PAT
Vault: SeaSea / Engineering / Dev Accounts
Fields:
  - token: github_pat_xxxxxxxxxxxx ← 立即粘贴,不要拖延
  - expiry: 2026-07-28
  - repos: seasea-main, seasea-gtm-os, boids-brand
  - generated_by: <操作人名字>
  - rotation_reminder: 2026-07-21 (到期前 7 天)
```

> 🚨 **绝对不要把 token 发到微信群、飞书群、Slack、邮件正文、截图里**。
> 需要传递给 WorkBuddy 时,直接在对话中粘贴(沙箱隔离,会话结束即销毁)。
> 需要传递给团队成员时,用密码管理器的共享功能。
>
> **Never share token in WeChat/Feishu/Slack/email/screenshots**.
> Paste directly in WorkBuddy conversation (sandbox isolated, destroyed on session end).
> Use password manager sharing for team members.

---

## Step 4 — 接入 WorkBuddy / Integrate with WorkBuddy

### 4.1 快速接入(一句话搞定)/ Quick Integration (One-liner)

拿到 token 后,在 WorkBuddy 开新会话,直接发:

```
clone SeaSea-cc/seasea-main 到 /workspace,token: github_pat_xxx...xxx
```

WorkBuddy 会自动执行:

```bash
# 设置鉴权
export GH_TOKEN=github_pat_xxx...xxx

# clone 仓库(含子模块)
gh repo clone SeaSea-cc/seasea-main /workspace/seasea-main -- --recurse-submodules

# 设置 git 身份为 seasea-dev
cd /workspace/seasea-main
git config user.name "seasea-dev"
git config user.email "dev@seasea.cc"
```

token 仅存在于该会话的环境变量中,**不会写入 `.gitconfig` 或任何配置文件**,会话结束后随沙箱销毁。

### 4.2 多仓库同时 clone / Clone Multiple Repos

如果需要同时操作多个仓库,一句搞定:

```
clone SeaSea-cc/seasea-main 和 SeaSea-cc/seasea-gtm-os 到 /workspace,token: github_pat_xxx...xxx
```

WorkBuddy 会并行 clone 并分别设置 git 身份。

### 4.3 验证接入 / Verify Integration

clone 完成后,确认以下三项:

**① 验证身份 / Verify Identity**
```bash
cd /workspace/seasea-main
git config user.name   # 应输出: seasea-dev
git config user.email  # 应输出: dev@seasea.cc
git remote -v          # 应输出: origin → https://github.com/SeaSea-cc/seasea-main.git
```

**② 验证 push 权限 / Verify Push Permission**
```bash
git checkout -b test/dev-integration-20260628
echo "# dev integration test $(date)" >> .dev-test.md
git add .dev-test.md
git commit -m "test: verify seasea-dev can push to SeaSea-cc repos via WorkBuddy cloud sandbox — this is a one-time integration test commit that will be deleted after verification is complete"
git push origin test/dev-integration-20260628
```

**③ 验证 PR 权限 / Verify PR Permission**
```bash
GH_TOKEN=github_pat_xxx...xxx gh pr create \
  --title "[dev] test: verify PR creation" \
  --body "Integration test PR — will be closed after verification." \
  --base main \
  --head test/dev-integration-20260628 \
  --repo SeaSea-cc/seasea-main
```

验证成功后,关闭测试 PR 并删除分支:
```bash
# 关闭 PR
gh pr close <PR号> --repo SeaSea-cc/seasea-main
# 删除远程分支
git push origin --delete test/dev-integration-20260628
# 回到 main
git checkout main
# 删除本地分支
git branch -D test/dev-integration-20260628
```

> 📸 **截图位 Screenshot 5**: PR 成功创建的 GitHub 页面,存档证明接入流程跑通。

### 4.4 接入方式权衡 / Method Trade-offs

| 方式 / Method | 安全性 / Security | 便利性 / Convenience | 能 push 回 GitHub | 当前推荐 |
|---|---|---|---|---|
| 对话粘贴 token | 中(token 30 天有效,沙箱隔离,会话结束销毁) | 高(一句话搞定) | ✅ | ✅ 推荐 |
| tar 上传仓库 | 高(无鉴权) | 低(每次手动打包) | ❌ 需手动 diff 回传 | ❌ |
| GitHub App(未来) | 最高(短-lived token,自动轮换) | 中(需开发 OAuth) | ✅ | 🔜 v2.0 |

---

## Step 5 — 协同工作流 / Collaboration Workflow

### 5.1 标准协同流程

团队某成员想用 WorkBuddy 改 seasea-main 仓库时:

```
1. 在 WorkBuddy 开新会话
2. 告知:"clone SeaSea-cc/seasea-main,用这个 token: <PAT>"
3. 描述任务:"创建团队,fe-dev 改 X,be-dev 改 Y,reviewer 审"
4. WorkBuddy:clone → 建团 → spawn teammates → 并行工作
5. teammates 在 feature 分支提交,开 PR,作者署名 seasea-dev
6. 人类 reviewer 在 GitHub 上 review + merge
7. 会话结束,沙箱销毁
```

### 5.2 分支与提交规范 / Branch & Commit Conventions

**分支命名 / Branch Naming**:
```
dev/<feature>-<date>
例: dev/gtm-event-spec-20260628
```

**Commit 规范 / Commit Convention**(遵循 Aaron 已有规则):
- commit message **不少于 250 字符**
- 格式: `<type>(<scope>): <subject>\n\n<body>\n\n<footer>`
- footer 必须包含 `Generated-by: WorkBuddy\nReviewed-by: <human>`
- type 使用 conventional commits: feat / fix / docs / refactor / chore / test

**示例 / Example**:
```
feat(gtm): add boids-brand event spec for one-click flow

This commit introduces the GTM event specification for the boids-brand
one-click interaction flow, covering click, impression, and conversion
events. The spec includes event names, parameters, trigger conditions,
and data layer push examples. Also updates the seasea-gtm-os README to
reference the new spec and adds validation tests to ensure event names
match the approved tracking taxonomy. This unblocks the marketing team
from instrumenting the one-click flow in the next release cycle.

Generated-by: WorkBuddy
Reviewed-by: @aaronwz0
```

### 5.3 PR 规范 / PR Convention

PR 标题前缀加 `[dev]`,便于筛选:
```
[dev] feat(gtm): add boids-brand one-click event spec
```

PR 描述模板:
```markdown
## 变更说明 / Summary
<本次改动做了什么,为什么>

## WorkBuddy 会话 / Session
- 会话 ID: <可选,便于回溯>
- 执行角色: fe-dev, be-dev, reviewer
- 触发指令: <原始任务描述摘要>

## 人类 Review / Human Review
- [ ] 代码已人工审查
- [ ] 测试通过
- [ ] 无硬编码密钥/凭据

Generated-by: WorkBuddy
```

---

## 6. 权限矩阵 / Permission Matrix

### seasea-dev 在各仓库的权限

| 仓库 / Repo | Contents | PR | Workflows | Issues | Administration |
|---|---|---|---|---|---|
| seasea-main | RW | RW | RW | RW | ❌ |
| seasea-gtm-os | RW | RW | RW | RW | ❌ |
| boids-brand | RW | RW | RW | RW | ❌ |
| 其他仓库 | ❌ | ❌ | ❌ | ❌ | ❌ |

### 组织级权限

| 权限 | 是否授予 / Granted | 说明 |
|---|---|---|
| Org Member | ✅ | 加入组织 |
| Org Owner | ❌ | 绝对禁止 |
| Org-wide repo creation | ❌ | 不允许建新仓库 |
| Org-wide package admin | ❌ | - |

---

## 7. 安全与回收 / Security & Rotation

### 7.1 Token 轮换周期

- **强制 30 天过期**:fine-grained PAT 设置 30 天 expiry
- **提前 7 天提醒**:密码管理器设置 `rotation_reminder`
- **轮换流程 / Rotation Flow**:
  1. 生成新 token(同权限,新过期时间)
  2. 更新密码管理器条目
  3. 通知当前正在使用 WorkBuddy 的成员换用新 token
  4. 在 GitHub 上 revoke 旧 token
  5. 验证旧 token 已失效(`gh auth status` 应报错)

### 7.2 紧急回收 / Emergency Revocation

**触发条件 / Triggers**:
- 怀疑 token 泄漏(出现在聊天记录、截图、日志)
- seasea-dev 账号异常登录告警
- 团队成员离职且曾接触 token
- WorkBuddy 沙箱被怀疑被入侵

**操作 / Action**:
1. 立即登录 seasea-dev → Settings → Developer settings → PAT → Revoke 对应 token
2. 在密码管理器标记 token 为 `REVOKED <日期>`
3. 通知所有正在使用 WorkBuddy 的成员停止会话
4. 审计 seasea-dev 近 30 天的 commit/PR 记录,确认无异常
5. 生成新 token,通知团队恢复使用

### 7.3 账号级回收 / Account-level Revocation

若 seasea-dev 账号本身被怀疑入侵:
1. 组织 Owner 在 `SeaSea-cc/People` 移除 seasea-dev
2. 修改 seasea-dev 密码 + 重新生成 2FA
3. Revoke 所有 PAT
4. 审计所有仓库的 seasea-dev commit

---

## 8. 故障排查 / Troubleshooting

| 症状 / Symptom | 原因 / Cause | 解决 / Fix |
|---|---|---|
| `gh repo clone` 返回空目录 | token 未鉴权或无该仓库权限 | 检查 token expiry、仓库 collaborator 配置 |
| `git push` 报 403 | Write 权限缺失 | 仓库 Settings → Collaborators 重新授权 |
| `gh pr create` 报 422 | 分支保护规则阻止 seasea-dev push | 调整 branch protection,允许 seasea-dev push 到 feature 分支(不是 main) |
| CI 不触发 | Workflows 权限缺失 | PAT 重新勾选 Workflows: Read and write |
| Commit 作者显示成你个人账号 | git config user 没设置 | 执行 `git config user.name "seasea-dev"; git config user.email "dev@seasea.cc"` |
| WorkBuddy 会话结束代码丢失 | 沙箱不持久 | 重要改动必须 push 到 GitHub,不要只留在 /workspace |

---

## 9. FAQ

**Q1: 为什么不用 GitHub App?**
A: WorkBuddy 当前基于 `gh` CLI + PAT,User Account + fine-grained PAT 零开发成本。等自动化任务多了再迁移 GitHub App,届时本 SOP 升级 v2.0。

**Q2: seasea-dev 能 merge PR 吗?**
A: 默认不能。分支保护规则要求人工 approve + merge。如果某个仓库允许 seasea-dev auto-merge,需在该仓库分支保护里显式开启 `Allow auto-merge`,且 PR 必须带 `[auto-merge]` 标识,由人工触发。

**Q3: 多人同时用 WorkBuddy 会冲突吗?**
A: 每人开自己的 WorkBuddy 会话,各自 clone 独立沙箱,不会互相干扰。但若同时改同一仓库同一文件,PR 层面会有 merge conflict,需人工解决。建议不同人用不同 feature 分支。

**Q4: WorkBuddy 之外的 AI 工具(Cursor、Copilot)能用这个 seasea-dev 账号吗?**
A: 可以,只要工具支持 PAT 鉴权。但建议不同工具用不同 token(都挂在 seasea-dev 下,token name 区分),便于审计哪个工具做了什么。

**Q5: token 过期了但有人还在用 WorkBuddy 怎么办?**
A: 旧 token 会直接失效,clone/push 报 401。应提前 7 天在群里通知轮换,密码管理器里查新 token。应急情况下可生成一个 7 天临时 token 过渡。

**Q6: 子模块仓库怎么处理?**
A: clone 时加 `--recurse-submodules`。若子模块在另一个组织/账号下,seasea-dev 也需在那个仓库有 read 权限。

---

## 附录 A — 快速上手 Checklist / Quick Start Checklist

seasea-dev 账号到第一次协同的完整步骤:

- [x] 注册 seasea-dev 账号(dev@seasea.cc + 强密码 + 2FA)
- [ ] 上传品牌头像,设置 Bio
- [x] 加入 SeaSea-cc 组织(Member 角色) ✅ 已完成
- [x] seasea-dev 已加入组织(已完成 ✅)
- [ ] 逐仓库授权 Write(seasea-main / seasea-gtm-os / boids-brand)
- [ ] 生成 fine-grained PAT(30 天,限定仓库,Contents/PR/Workflows/Issues RW)
- [ ] 存入密码管理器,设置轮换提醒
- [ ] 在 WorkBuddy 会话测试 clone + push
- [ ] 设置 git config user 为 seasea-dev
- [ ] 开第一个测试 PR,验证流程跑通
- [ ] 把本文档入库到 `seasea-main/docs/seasea-dev-sop.md`
- [ ] 团队同步宣讲,明确轮换与回收流程

---

## 附录 B — 联系人 / Contacts

| 角色 / Role | 负责人 / Owner | 职责 / Responsibility |
|---|---|---|
| SOP 维护人 | Aaron (@aaronwz0) | 文档更新、流程演进 |
| 组织 Owner | <待填> | seasea-dev 账号管理、权限授予、紧急回收 |
| 密码管理器管理员 | <待填> | token 存储、轮换提醒 |
| 安全审计 | <待填> | 季度审计 seasea-dev 操作记录 |

---

**文档结束 / End of Document**

> 本文档已就绪,将入库到 `SeaSea-cc/seasea-main` 仓库的 `docs/seasea-dev-sop.md`。后续更新走 PR 流程,由 Aaron review 合并。
> This document is ready to be committed to `SeaSea-cc/seasea-main` under `docs/seasea-dev-sop.md`. Future updates via PR, reviewed by Aaron.
