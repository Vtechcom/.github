# Contributing to VTechcom Labs

Thanks for your interest in contributing to VTechcom Labs and the HydraOne ecosystem! 🎉
*Tiếng Việt: xem [phần tóm tắt bên dưới](#tóm-tắt-tiếng-việt).*

This guide applies to every repository in the `Vtechcom` organization unless a repository has its own `CONTRIBUTING.md`.

## Before you start

1. **Join our [Discord](https://discord.gg/NPfH5gRbHC)** and read `#rules` and `#start-here`.
2. **Sign the CLA (and NDA) on paper.** All contributions require a signed Contributor License Agreement. Agreements are signed by hand at the VTechcom Labs office in one session during week 0. If you cannot come to the office, print, sign, scan and email the signed copy to haipham@vtechcom.org, then hand in the original later. You are invited to the GitHub organization only after your signature is recorded.
3. **Enable 2FA** on your GitHub account.
4. Read the [Code of Conduct](CODE_OF_CONDUCT.md).

## Contributor tiers

| Tier | What you do | Access |
|---|---|---|
| **X3 – Tester** | Test alpha builds, file test reports | Open issues on public repos |
| **X2 – Contributor** | Fix issues on public repos via fork + PR | Triage on public repos |
| **X1 – Builder** | Build HydraOne games / tooling in squads | Write on assigned private repos (**NDA required**) |
| **DevX-Intern** | Work on the SDK / HydraOne core with the core team (max 1 seat) | As assigned |
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
- **Private repositories** (after signing the NDA) — only these, **with data sharing for model training turned off**:
  - Claude, Codex/ChatGPT, Gemini (paid plan or API)
  - GitHub Copilot (disable the setting that allows GitHub to use your data for product improvement / model training)
  - Cursor (**Privacy Mode** on)
  - Local models (Ollama, llama.cpp, LM Studio, …)

  Send screenshots of these settings to your mentor when you sign the NDA. Disable any other AI extension before opening a private repo.
- **Free models that require sharing your data** — e.g. Google AI Studio free tier (Gemini, Gemma), `:free` models on OpenRouter, free-tier models in opencode, Meta AI, DeepSeek / Qwen / Kimi / GLM via their own apps or APIs, free or unknown IDE extensions — may be used **on open-source repositories only**. If you are not sure whether a tool trains on your data, assume it does.
- **Never** paste secrets, keys or `.env` files into any AI tool, on any repository.
- Issues/test reports may be polished with AI but must contain real evidence (screenshots, video, tx hash, steps).

## High-risk areas

Contributors must not change, without an explicit DevX assignment:

- Transaction signing, keys, mnemonics, wallets
- Dependencies (`package.json`, lockfiles)
- CI/CD workflows, deployment config, secrets

PRs touching these are labelled `high-risk` and need two DevX reviews.

**DevX-Intern** may write code in these areas when explicitly assigned, with **two DevX approvals** (including Ania or Randolph). Interns do not merge `high-risk` PRs, do not access secrets or infrastructure, do not merge to `release` or deploy, and do not publish npm packages.

## Commit messages

Use [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`.

## Licensing

- Public repositories are licensed under **Apache 2.0**; by signing the CLA you grant VTechcom Labs a license to your contributions.
- Private repositories are covered by your **NDA**, which assigns the economic rights of your contributions to VTechcom Labs.

---

## Tóm tắt tiếng Việt

1. Vào Discord, đọc `#rules`, `#start-here`. **Ký tay CLA và NDA tại văn phòng** (1 buổi ở tuần 0; ở xa: ký tay, scan gửi haipham@vtechcom.org, nộp bản gốc sau). Bật **2FA** GitHub. Chỉ được mời vào tổ chức GitHub sau khi đã ký.
2. Chọn issue có nhãn `good first issue` / `green 🤟` / `amber !` → comment xin nhận → **chờ được assign** rồi mới làm.
3. Giới hạn: X2 tối đa 1 PR mở, X1 tối đa 2 PR mở; mỗi PR khoảng **≤ 400 dòng**.
4. Điền **đầy đủ PR template** (thiếu mục sẽ bị đóng không review). CI phải xanh trước khi review.
5. **Được dùng AI** nhưng phải khai báo và **hiểu, chịu trách nhiệm 100%**. Chỉ dùng API **Hydra v2**. Repo private: chỉ Claude/Codex/Gemini (trả phí/API), Copilot, Cursor (Privacy Mode) hoặc model local, và **tắt chia sẻ dữ liệu huấn luyện**. Model miễn phí bắt buộc chia sẻ dữ liệu (Google AI Studio free, `:free` OpenRouter, free-tier opencode, Meta AI, DeepSeek…) **chỉ dùng với repo mã nguồn mở**. Không bao giờ đưa secret vào AI.
6. Một số PR được chọn để **"bảo vệ PR"** 5 phút — tự giải thích thay đổi, không dùng AI.
7. Không push thẳng `main`/`master`/`release`; không tự merge PR; không sửa vùng high-risk (ký tx, khoá, dependency, CI, secret). DevX-Intern được làm vùng high-risk khi được giao, cần 2 DevX duyệt.
