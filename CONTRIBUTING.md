# Contributing to VTechcom

Thanks for your interest in contributing to VTechcom and the HydraOne ecosystem! 🎉
*Tiếng Việt: xem [phần tóm tắt bên dưới](#tóm-tắt-tiếng-việt).*

This guide applies to every repository in the `Vtechcom` organization unless a repository has its own `CONTRIBUTING.md`.

## Before you start

1. **Join our Discord** and read `#rules` and `#start-here`.
2. **Sign the CLA.** All contributions require a signed Contributor License Agreement. The CLA bot will prompt you on your first pull request.
3. **Enable 2FA** on your GitHub account.
4. Read the [Code of Conduct](CODE_OF_CONDUCT.md).

## Contributor tiers

| Tier | What you do | Access |
|---|---|---|
| **X3 – Tester** | Test alpha builds, file test reports | Open issues on public repos |
| **X2 – Contributor** | Fix issues on public repos via fork + PR | Triage on public repos |
| **X1 – Builder** | Build HydraOne games / tooling in squads | Write on assigned private repos (**NDA required**) |
| **DevX** | Core team | Maintainers |

Promotion is based on merged work and mentor review. See the contributor handbook (linked in Discord `#start-here`).

## Workflow

1. **Pick an issue.** Look for `good first issue`, `green 🤟` (easy) or `amber !` (medium). Comment to ask for it.
2. **Wait to be assigned.** PRs that are not linked to an issue assigned to you will be closed.
3. **Work in progress limits:**
   - X2: at most **1** open PR and **2** assigned issues.
   - X1: at most **2** open PRs and **2** assigned issues.
4. **Fork** (public repos) or create a branch (private repos, X1 only). Branch name: `<type>/<issue-number>-<short-slug>`, e.g. `fix/58-bridge-docs`.
5. **Keep PRs small:** about **400 changed lines** max (excluding lockfiles, fixtures, generated code). Split larger work.
6. **Run checks locally** (lint, typecheck, build, tests — see the repo README / `AGENTS.md`).
7. **Open the PR** using the template. **Every section is required.** Incomplete PRs are closed without review.
8. **Fix CI first.** Reviewers only look at PRs with green CI.
9. **Review.** A mentor reviews your PR. Some PRs are selected for a short **"PR defense"** (`needs-defense`): you explain your change in a 5-minute call or by answering questions in the PR, without AI help.
10. **Never** push directly to `main`/`master`/`release`. Contributors do not merge their own PRs.

## Using AI tools

AI assistants are **allowed**. You must:

- **Declare** how much AI you used in the PR template.
- **Understand and own every line** you submit. "The AI wrote it" is not an excuse.
- Use **Hydra v2** APIs only. AI models often produce outdated Hydra v1 code (`Commit`, `HeadIsInitializing`, `Abort`, …) — this will be rejected.
- **Private repositories:** only Claude, Codex/ChatGPT or Gemini, **with data sharing for model training turned off** (see your NDA).
- Issues/test reports may be polished with AI but must contain real evidence (screenshots, video, tx hash, steps).

## High-risk areas (DevX only)

Contributors must not change, without an explicit DevX assignment:

- Transaction signing, keys, mnemonics, wallets
- Dependencies (`package.json`, lockfiles)
- CI/CD workflows, deployment config, secrets

PRs touching these are labelled `high-risk` and need two DevX reviews.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`.

## Licensing

- Public repositories are licensed under **Apache 2.0**; by signing the CLA you grant VTechcom a license to your contributions.
- Private repositories are covered by your **NDA**, which assigns the economic rights of your contributions to VTechcom.

---

## Tóm tắt tiếng Việt

1. Vào Discord, đọc `#rules`, `#start-here`. **Ký CLA** (bot sẽ nhắc ở PR đầu tiên). Bật **2FA** GitHub.
2. Chọn issue có nhãn `good first issue` / `green 🤟` / `amber !` → comment xin nhận → **chờ được assign** rồi mới làm.
3. Giới hạn: X2 tối đa 1 PR mở, X1 tối đa 2 PR mở; mỗi PR khoảng **≤ 400 dòng**.
4. Điền **đầy đủ PR template** (thiếu mục sẽ bị đóng không review). CI phải xanh trước khi review.
5. **Được dùng AI** nhưng phải khai báo và **hiểu, chịu trách nhiệm 100%**. Chỉ dùng API **Hydra v2**. Repo private: chỉ Claude/Codex/Gemini và **tắt chia sẻ dữ liệu huấn luyện**.
6. Một số PR được chọn để **"bảo vệ PR"** 5 phút — tự giải thích thay đổi, không dùng AI.
7. Không push thẳng `main`/`master`/`release`; không tự merge PR; không sửa vùng high-risk (ký tx, khoá, dependency, CI, secret).
