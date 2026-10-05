# Security Policy

## Reporting a vulnerability

**Do not open a public issue for security vulnerabilities.**

Please report privately using one of:

1. **GitHub private vulnerability reporting** — on the affected repository, go to *Security → Report a vulnerability*.
2. Email haipham@vtechcom.org.

Please include:

- Affected repository, package and version / commit
- Description and impact (e.g. key exposure, incorrect signing, fund loss on testnet/mainnet)
- Steps to reproduce or a proof of concept
- Your GitHub / Discord handle for follow-up

We aim to acknowledge reports within **3 business days** and will keep you informed of the fix progress.

## Scope

Of particular interest:

- `@hydra-sdk/*` packages: transaction building, signing, key derivation, WASM loading
- Hydra Head interaction (bridge, deposits, fanout)
- Leaked credentials or secrets in any repository

## Out of scope

- Vulnerabilities in upstream projects (report to them directly, e.g. `cardano-scaling/hydra`)
- Social engineering, physical attacks, denial of service

---

**Tiếng Việt:** Không tạo issue công khai cho lỗ hổng bảo mật. Báo riêng qua *Security → Report a vulnerability* trên repo hoặc email haipham@vtechcom.org. Chúng tôi phản hồi trong vòng 3 ngày làm việc.
