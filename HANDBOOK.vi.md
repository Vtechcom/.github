# Sổ tay Contributor VTechcom Labs

> Phiên bản 0.1 (bản nháp) · Áp dụng từ đợt 1  
> Tài liệu đi kèm: [Contributing guide](https://github.com/Vtechcom/.github/blob/main/CONTRIBUTING.md) · [Code of Conduct](https://github.com/Vtechcom/.github/blob/main/CODE_OF_CONDUCT.md) · [Security policy](https://github.com/Vtechcom/.github/blob/main/SECURITY.md)

Chào mừng bạn đến với Chương trình Contributor của VTechcom Labs! 👋

Sổ tay này giải đáp các câu hỏi bạn sẽ gặp trong suốt quá trình tham gia: bạn làm gì, phối hợp cùng ai, theo quy trình kỹ thuật nào và được ghi nhận đóng góp ra sao. Hãy đọc kỹ toàn bộ tài liệu trước buổi họp weekly đầu tiên và lưu lại để tra cứu khi cần.

---

## Mục lục

1. [VTechcom Labs là ai](#1-vtechcom-labs-là-ai)
2. [Chương trình dành cho ai](#2-chương-trình-dành-cho-ai)
3. [Thang bậc](#3-thang-bậc)
4. [Hành trình của bạn](#4-hành-trình-của-bạn)
5. [Tuần đầu tiên](#5-tuần-đầu-tiên)
6. [Quy trình làm việc trên GitHub](#6-quy-trình-làm-việc-trên-github)
7. [Dùng AI đúng cách](#7-dùng-ai-đúng-cách)
8. [Nhịp làm việc](#8-nhịp-làm-việc)
9. [Giao tiếp](#9-giao-tiếp)
10. [Ghi nhận và lên bậc](#10-ghi-nhận-và-lên-bậc)
11. [Pháp lý và bảo mật](#11-pháp-lý-và-bảo-mật)
12. [Quy tắc và kỷ luật](#12-quy-tắc-và-kỷ-luật)
13. [Khi bạn cần dừng lại](#13-khi-bạn-cần-dừng-lại)
14. [Câu hỏi thường gặp](#14-câu-hỏi-thường-gặp)
15. [Liên hệ](#15-liên-hệ)

---

## 1. VTechcom Labs là ai

VTechcom Labs là đội ngũ kỹ thuật chuyên sâu về **Hydra** — giải pháp Layer 2 của mạng Cardano, mang lại tốc độ xử lý giao dịch tức thì với chi phí tối ưu gần như bằng 0. Các sản phẩm trọng tâm của đội ngũ gồm:

- **Hydra SDK**: Bộ công cụ mã nguồn mở giúp lập trình viên xây dựng ví và ứng dụng trên Cardano + Hydra.
- **Hexcore**: Công cụ trực quan giúp khởi tạo và vận hành Hydra Head chỉ với vài thao tác.
- **HydraOne**: Nền tảng kết nối người dùng với các tựa game và ứng dụng phi tập trung (DApp) chạy trên Hydra.
- Đóng góp trực tiếp cho dự án Hydra open-source chính thức và hoàn thành nhiều đề án thuộc Project Catalyst.

**Đội ngũ nòng cốt (Core DevX):**

| Thành viên | Vai trò trong chương trình |
| ---------- | -------------------------- |
| **Tony** | CEO, quản trị Discord |
| **Ania** | CTO, mentor chung, kiến trúc hệ thống, QA chính |
| **Randolph** | Mentor Backend |
| **VenomVu** | Mentor Frontend |
| **ThanhDT** | Frontend, quản trị Discord |

---

## 2. Chương trình dành cho ai

Chương trình hướng tới các bạn mong muốn **học hỏi thông qua việc phát triển sản phẩm thực tế**: mã nguồn của bạn sẽ được tích hợp trực tiếp vào bộ SDK có người dùng thật, vào công cụ vận hành node mạng, hoặc các tựa game trực tiếp trên nền tảng HydraOne.

**Quyền lợi của bạn:**

- Được mentor trực tiếp từ đội ngũ core DevX, review chi tiết từng pull request.
- Tham gia các buổi seminar chuyên sâu về blockchain, Cardano, Hydra (chiều thứ 6, theo lịch).
- Tham gia Demo Day hàng tháng — trình bày giải pháp và sản phẩm của mình trước cộng đồng.
- Trải nghiệm quy trình phát triển DApp chuẩn mực: quản trị issue, PR review, CI/CD, chu kỳ sprint.
- Cơ hội được mời gia nhập đội ngũ core DevX.

**Lưu ý quan trọng trước khi tham gia:**

- Chương trình hoàn toàn **tự nguyện, không có thù lao**. Đây không phải là hợp đồng lao động hay chương trình thực tập công ty.
- Mọi đóng góp của bạn đều được ghi nhận minh bạch. Chứng nhận, thưởng nhiệm vụ (bounty) hay các quyền lợi bổ sung **có thể** được xem xét trong tương lai, nhưng không phải cam kết bắt buộc của tổ chức.
- Chương trình hướng đến sự đồng hành **lâu dài**. Thời gian đóng góp tối thiểu đề xuất: **5 giờ/tuần**.

> *Lưu ý:* Sổ tay này quy định chi tiết lộ trình cho các track kỹ thuật (X2, X1). Với bậc **X3 (Tester)** và **Content**, quy trình và nhiệm vụ sẽ được kích hoạt theo thông báo riêng của từng đợt huy động.

---

## 3. Thang bậc

| Bậc | Nội dung công việc | Quyền truy cập | Thỏa thuận cần ký |
| --- | ------------------ | -------------- | ----------------- |
| **X3 — Tester** | Tham gia các đợt test game alpha, SDK Playground; báo cáo lỗi | Tạo issue trên repo public; role Discord theo đợt test | — |
| **X2 — Contributor** | Giải quyết issue trên các repo mã nguồn mở | Quyền Triage trên repo public; làm việc qua fork + pull request | Ký giấy CLA tại văn phòng |
| **X1 — Builder** | Xây dựng game DApp cho HydraOne hoặc phát triển Hexcore thế hệ mới theo squad | Quyền đọc SDK nội bộ và game mẫu; quyền Write trên repo private được giao | Ký giấy CLA + NDA tại văn phòng |
| **DevX-Intern** | Đóng góp trực tiếp vào SDK hoặc lõi HydraOne cùng đội ngũ core | Theo phân công chi tiết của core | Ký giấy CLA + NDA tại văn phòng |
| **DevX** | Đội ngũ nòng cốt (core team) | Toàn quyền quản trị | — |
| **Content** | Biên tập bài viết, tổng hợp seminar, hỗ trợ quản trị cộng đồng | Phân quyền Discord | — |

**Hai track phát triển của X1:**

- **Track Game:** Xây dựng tựa game mới vận hành trên HydraOne, phát triển dựa trên game mẫu chuẩn (`hydra-mines`) để nắm nhanh quy trình tích hợp Hydra.
- **Track Hexcore:** Phát triển công cụ vận hành node `hexcore-v2` (NestJS, Docker, Nuxt).

**Vị trí DevX-Intern:** Chỉ duy trì **tối đa 1 người** tại một thời điểm để đảm bảo đội ngũ core có đủ thời gian kèm cặp, hướng dẫn chuyên sâu.

**Phân định quyền hạn với vùng hạ tầng và mã nguồn nhạy cảm:**

- **Chỉ đội ngũ core DevX phụ trách:** Hạ tầng máy chủ, hệ thống domain, CI/CD deployment, secret keys, đăng ký game mới vào registry backend của HydraOne, publish gói npm, và quyền merge vào nhánh `release`.
- **Ngoại lệ có kiểm soát của DevX-Intern:** Được phép viết code liên quan đến ký giao dịch, ví, khoá, dependency, hoặc cấu hình CI **chỉ khi có issue được giao việc rõ ràng**. Pull request bắt buộc phải có **2 thành viên DevX duyệt** (trong đó bắt buộc có **Ania** hoặc **Randolph**). DevX-Intern **không** được tự merge PR high-risk, không được truy cập secret hay hạ tầng máy chủ thực tế (Coolify, Cloudflare, server), không được merge vào `release` hay tự ý deploy.

---

## 4. Hành trình của bạn

```
Đăng ký ──► Xét hồ sơ ──► Ký giấy CLA/NDA ──► Thử việc 4 tuần ──► X1 / X2 / Dừng
                                                 │
                             Tuần 1–2: Làm repo public (X2)
                             Tuần 3–4: Kích hoạt NDA, vào track Game hoặc Hexcore
                             Cuối tuần 4: Bài kiểm tra debug trực tiếp 45 phút
```

### Chi tiết thử việc 4 tuần

| Mốc thời gian | Hoạt động chính | Mục tiêu cần đạt |
| ------------- | --------------- | ---------------- |
| **Tuần 0** | Ký giấy CLA + NDA tại văn phòng; kích hoạt 2FA; vào Discord & GitHub; thiết lập môi trường | Sẵn sàng nhận issue đầu tiên |
| **Tuần 1–2** | Hoàn thành **1 issue `green 🤟`** và **1 issue `amber !`** trên repo public (Hydra SDK, Playground, tài liệu) | Làm quen quy trình làm việc và kiến thức Hydra v2 |
| **Cuối tuần 2** | Trao đổi đánh giá giữa kỳ (15 phút) cùng mentor | Nhận phản hồi và định hướng chọn track |
| **Tuần 3–4** | Kích hoạt quyền NDA; tham gia track Game hoặc Hexcore | Làm quen với codebase và mã nguồn thực tế của dự án |
| **Cuối tuần 4** | **Bài kiểm tra trực tiếp 45 phút:** Debug lỗi cài sẵn qua chia sẻ màn hình | Đánh giá tư duy độc lập và khả năng xử lý sự cố |

Sau thời gian thử việc sẽ có ba hướng đánh giá: **lên X1**, **tiếp tục rèn luyện tại X2** (đóng góp repo public, có thể xét lại sau), hoặc **dừng tham gia**. Mọi quyết định đều được mentor giải thích rõ lý do kỹ thuật.

**Gợi ý chọn issue trong Tuần 1–2:**

- **Định hướng Frontend:** Chọn các issue gắn nhãn `playground` hoặc `docs` trên repo [Hydra SDK](https://github.com/Vtechcom/hydra-sdk/issues).
- **Định hướng Backend:** Chọn các issue về bộ test fixture và connector trên Hydra SDK.
- **Tất cả thành viên:** Đọc kỹ tài liệu vòng đời Hydra Head **v2** — đây là kiến thức nền tảng bắt buộc cho mọi track.

---

## 5. Tuần đầu tiên

Checklist Tuần 0 cần hoàn thành trước buổi họp weekly đầu tiên:

**Ký thỏa thuận & Tài khoản**

- [ ] Lên văn phòng ký thỏa thuận giấy **CLA** và **NDA** (in 2 bản, mỗi bên giữ 1 bản; dưới 18 tuổi cần người giám hộ ký cùng).
- [ ] Bật **xác thực 2 lớp (2FA)** cho tài khoản GitHub — điều kiện bắt buộc trước khi được mời vào tổ chức.
- [ ] Bật 2FA cho tài khoản Discord.
- [ ] Tham gia [Discord VTechcom Labs](https://discord.gg/NPfH5gRbHC), hoàn tất quy trình onboarding và nhận vai trò ban đầu.
- [ ] Chấp nhận lời mời tham gia tổ chức `Vtechcom` trên GitHub (lời mời gửi sau khi bạn đã ký giấy và được ghi nhận vào sổ contributor).

**Nghiên cứu tài liệu**

- [ ] Đọc kỹ Sổ tay này.
- [ ] Đọc [Contributing guide](https://github.com/Vtechcom/.github/blob/main/CONTRIBUTING.md) và [Code of Conduct](https://github.com/Vtechcom/.github/blob/main/CODE_OF_CONDUCT.md).
- [ ] Đọc README cùng tài liệu hướng dẫn agent (`CLAUDE.md` / `AGENTS.md`) của repo [Hydra SDK](https://github.com/Vtechcom/hydra-sdk).

**Thiết lập môi trường phát triển (Local Setup)**

- [ ] Cài đặt Node.js ≥ 22, pnpm, Git, Docker trên máy cá nhân.
- [ ] Fork và clone repo Hydra SDK; chạy thành công các lệnh `pnpm install`, `pnpm build:packages`, `pnpm test`.
- [ ] Tạo ví testnet và nhận tADA thử nghiệm theo hướng dẫn tại kênh `#start-here` trên Discord.

**Bắt đầu công việc**

- [ ] Đăng bài giới thiệu và standup đầu tiên tại diễn đàn `#standup`.
- [ ] Tìm một issue có nhãn `good first issue`, để lại bình luận xin nhận việc và chờ mentor assign.

---

## 6. Quy trình làm việc trên GitHub

### 6.1 Từ issue đến merge

1. **Chọn issue:** Ưu tiên bắt đầu từ nhãn `good first issue`, `green 🤟` (mức độ cơ bản), tiếp theo là `amber !` (mức độ trung bình). Chú ý nhãn `tier:*` để chọn đúng nhiệm vụ phù hợp với bậc của mình.
2. **Xin nhận issue:** Để lại comment xin nhận và chờ mentor chính thức assign. *Pull request mở ra mà không gắn với issue đã assign cho bạn sẽ bị đóng.*
3. **Tạo branch:** Đặt tên branch theo định dạng chuẩn: `<loại>/<số-issue>-<mô-tả-ngắn>` (ví dụ: `fix/58-bridge-docs`).
4. **Phát triển và kiểm thử local:** Thực hiện thay đổi và chạy kiểm tra đầy đủ trên máy cá nhân: lint, typecheck, build, test (xem chi tiết trong README của repo).
5. **Mở pull request:** Điền đầy đủ thông tin theo PR template. **Mọi mục trong template đều bắt buộc** — PR thiếu nội dung hoặc không khai báo AI sẽ bị đóng mà không review.
6. **Đảm bảo CI pass (xanh):** Mentor chỉ tiến hành review khi toàn bộ pipeline CI đã vượt qua kiểm tra.
7. **Review:** Mentor review định kỳ theo khung giờ mỗi ngày, ưu tiên theo thứ tự nộp PR (PR mở trước sẽ được duyệt trước).
8. **Bảo vệ PR:** Trình bày giải pháp nếu PR được chỉ định (xem mục 6.4).
9. **Merge mã nguồn:** Contributor **không tự ý merge**. Mentor sẽ trực tiếp merge sau khi PR được phê duyệt hoàn toàn.

Theo dõi tiến độ công việc tổng thể trên bảng quản lý [HydraOne Delivery](https://github.com/orgs/Vtechcom/projects/17).

### 6.2 Giới hạn khối lượng công việc (WIP Limits)

| Tiêu chí giới hạn | Bậc X2 | Bậc X1 |
| ------------------ | ------ | ------ |
| Số pull request mở cùng lúc | 1 PR | 2 PR |
| Số issue đang nhận cùng lúc | 2 issue | 2 issue |
| Dung lượng tối đa một pull request | ~400 dòng thay đổi | ~400 dòng thay đổi |

*Dung lượng thay đổi không tính các file lockfile, test fixtures hay mã nguồn sinh tự động.* Với các nhiệm vụ lớn, hãy chủ động trao đổi với mentor để chia nhỏ thành nhiều PR tuần tự. Giới hạn này giúp mentor review kỹ lưỡng, tránh tình trạng review lướt.

### 6.3 Quy chuẩn commit

Áp dụng nghiêm ngặt chuẩn [Conventional Commits](https://www.conventionalcommits.org/). Tiêu đề commit viết bằng tiếng Anh, rõ ràng, không gõ dấu:

```
fix(bridge): forward X-Api-Key in HexcoreConnector
docs: update bridge API reference for hydra-node v2
test(bridge): add fixture decode tests for snapshot tags
```

Phần mô tả chi tiết (commit body) có thể viết bằng tiếng Việt hoặc tiếng Anh.

### 6.4 Bảo vệ PR (Defense Session)

Các pull request được gắn nhãn `needs-defense` sẽ yêu cầu bạn giải thích trực tiếp giải pháp trong khoảng **5 phút** qua kênh voice Discord, hoặc trả lời 2–3 câu hỏi kỹ thuật chuyên sâu do mentor đặt ra ngay trên PR — **tuyệt đối không dùng AI trợ giúp trong lúc này**.

- **Bắt buộc:** Áp dụng với PR dung lượng lớn (`size:L`) hoặc các PR chạm vào khu vực nhạy cảm (`high-risk`).
- **Ngẫu nhiên:** Chọn ngẫu nhiên khoảng 1/5 (20%) số PR thông thường còn lại.

Mục tiêu không phải gây khó khăn mà để đảm bảo bạn nắm vững thay đổi do mình tạo ra: lý do lựa chọn giải pháp, các kịch bản đã kiểm thử, và những điểm bạn còn băn khoăn hay chưa chắc chắn.

### 6.5 Báo cáo lỗi (Issue Reporting)

- Sử dụng đúng biểu mẫu: **Bug report** cho lỗi chức năng thông thường; **Test report** cho lỗi phát hiện trong các đợt test tập trung.
- Thông tin bắt buộc: Các bước tái hiện chi tiết (reproduction steps), kết quả thực tế và kết quả mong muốn, phiên bản môi trường, mạng thử nghiệm.
- Lỗi phức tạp: Bắt buộc đính kèm ảnh chụp màn hình, video minh họa hoặc mã giao dịch (tx hash) liên quan.
- **Tuyệt đối không bao giờ** dán cụm từ khôi phục ví (seed phrase), mã bí mật (private key) hay khóa API vào issue, kể cả ví testnet.
- Báo cáo thiếu bước tái hiện sẽ được gắn nhãn `needs-repro` và tự động đóng sau 7 ngày nếu không bổ sung.
- **Lỗ hổng bảo mật:** Không tạo issue công khai — vui lòng làm theo hướng dẫn tại [Security policy](https://github.com/Vtechcom/.github/blob/main/SECURITY.md).

### 6.6 Vùng nhạy cảm (High-risk Areas)

Contributor bậc X1 và X2 **không được tự ý chỉnh sửa** các khu vực sau nếu chưa có chỉ định và phân công cụ thể từ core team:

- Logic ký giao dịch, quản lý khóa bảo mật, mnemonic, tương tác ví.
- Quản lý gói thư viện phụ thuộc (`package.json`, lockfile).
- Cấu hình CI/CD workflow, file deploy hệ thống, cấu hình biến môi trường và secret.

Mọi PR chạm vào các thành phần trên sẽ tự động gắn nhãn `high-risk`. Riêng với DevX-Intern, khi được giao việc ở vùng này, PR bắt buộc phải có đủ **2 thành viên DevX phê duyệt** (trong đó phải có **Ania** hoặc **Randolph**).

### 6.7 Bắt buộc tương thích Hydra v2

Hệ thống Hydra node v2 đã loại bỏ hoàn toàn giai đoạn commit thủ công cũ. Mọi đoạn mã còn chứa các trạng thái cũ như `Commit`, `HeadIsInitializing`, `Committed`, `Abort` đều thuộc chuẩn **v1** lỗi thời và PR sẽ bị từ chối ngay lập tức. Đây là sai sót các công cụ AI thường tạo ra nhất — hãy luôn đối chiếu với tài liệu v2 chính thức.

---

## 7. Dùng AI đúng cách

VTechcom Labs khuyến khích việc sử dụng AI để nâng cao hiệu suất làm việc. Đội ngũ core cũng sử dụng AI hàng ngày. Tuy nhiên, bạn cần tuân thủ 4 nguyên tắc cốt lõi:

1. **Minh bạch & Khai báo:** Ghi rõ mức độ áp dụng và công cụ AI đã dùng ngay trong phần khai báo của PR template.
2. **Chịu trách nhiệm 100%:** Câu trả lời "do AI tự sinh mã" không được chấp nhận. Nếu bạn không giải thích được một dòng code, vui lòng không đưa dòng code đó vào PR.
3. **Cảnh giác với kiến thức cũ:** Các mô hình AI thường tạo ra mã nguồn Hydra v1 rất mượt mà nhưng không còn giá trị sử dụng. Hãy luôn đối chiếu tài liệu v2 và file `MIGRATION-v2.md` trong repo Hydra SDK.
4. **Trung thực về bằng chứng:** Bạn có thể dùng AI để trau chuốt câu từ trong báo cáo lỗi, nhưng bằng chứng lỗi (ảnh, video, log, tx hash) phải là kết quả kiểm thử thực tế của bạn.

### Quy tắc sử dụng công cụ AI theo loại Repository

| Loại Repository | Công cụ AI ĐƯỢC PHÉP dùng | Công cụ AI CẤM SỬ DỤNG |
| --------------- | ------------------------- | ---------------------- |
| **Repo Private** *(Sau khi ký NDA: `hydraone-sdk`, game mới, `hexcore-v2`)* | - Claude, ChatGPT/Codex, Gemini (bản trả phí hoặc qua API).<br>- GitHub Copilot, Cursor ở chế độ riêng tư (Privacy Mode).<br>- Các mô hình LLM chạy hoàn toàn offline tại local máy tính.<br>*Bắt buộc phải tắt tính năng chia sẻ dữ liệu cho mục đích huấn luyện (data training).* | Mọi công cụ hoặc mô hình AI **không có tùy chọn tắt** việc thu thập dữ liệu huấn luyện, hoặc mặc định ghi log nội dung mã nguồn của người dùng. |
| **Repo Open Source** *(Theo giấy phép Apache 2.0: `hydra-sdk`, `hydra-hexcore`)* | Mọi công cụ AI, bao gồm cả các gói dịch vụ miễn phí có điều khoản chia sẻ dữ liệu. | — *(Vẫn tuyệt đối cấm đưa secret, private key, token vào prompt).* |

> [!WARNING]
> **Cảnh báo về các dịch vụ và mô hình AI miễn phí:**
> Nhiều nền tảng và mô hình miễn phí hiện nay mặc định hoặc bắt buộc sử dụng dữ liệu người dùng (prompt, context, code) để huấn luyện mô hình hoặc cải thiện dịch vụ. Các công cụ này **chỉ được phép sử dụng với repo open source**.
> 
> Đối với repo private, nếu bạn không chắc chắn một công cụ có huấn luyện trên dữ liệu của mình hay không, **hãy mặc định là CÓ và không sử dụng công cụ đó**. Kể cả với repo open source, **tuyệt đối không bao giờ dán secret, `.env`, khóa API hay private key vào bất kỳ công cụ AI nào**.

#### Danh sách nhận diện các nhóm công cụ miễn phí dùng dữ liệu để huấn luyện:

1. **Mô hình miễn phí qua API hoặc Playground:**
   - Điển hình là gói miễn phí (Free Tier) của **Google AI Studio** (Gemini, Gemma): Theo điều khoản sử dụng, dữ liệu prompt và nội dung sinh ra có thể được Google ghi nhận và sử dụng bởi các chuyên viên đánh giá nhằm cải thiện sản phẩm và huấn luyện mô hình.
2. **Mô hình miễn phí trên các cổng tổng hợp (Aggregator Gateways):**
   - Các mô hình có hậu tố `:free` trên **OpenRouter**, các model thuộc free-tier trên **opencode** hoặc các cổng proxy trung gian tương tự. Đơn vị cung cấp hạ tầng phía sau thường ghi log toàn bộ nội dung hoặc khai thác dữ liệu để phục vụ việc tinh chỉnh (fine-tuning) mô hình.
3. **Chatbot và ứng dụng AI bản miễn phí của các hãng công nghệ:**
   - **Meta AI** (bao gồm cả Llama, Muse), **Grok** (xAI), **Microsoft Copilot** bản người dùng cá nhân (consumer) chưa bật chính sách bảo vệ dữ liệu thương mại, **Gemini web app** bản miễn phí khi chưa tắt tính năng lưu trữ hoạt động (*Gemini Apps Activity*).
4. **API hoặc ứng dụng lưu trữ dữ liệu tại nước ngoài có điều khoản cải thiện dịch vụ:**
   - **DeepSeek**, **Qwen** (Alibaba), **Kimi** (Moonshot), **GLM** (Zhipu AI)... khi sử dụng qua website, app hoặc endpoint API công cộng có điều khoản cho phép nhà cung cấp tận dụng dữ liệu người dùng để tối ưu hóa chất lượng hệ thống.
5. **Extension hỗ trợ lập trình (AI Coding) miễn phí hoặc không rõ nguồn gốc:**
   - **Windsurf** / **Codeium** gói cá nhân miễn phí, tiện ích **Continue** hoặc **Cline** khi cấu hình trỏ tới các endpoint/mô hình miễn phí, cùng các extension "AI Assistant" trôi nổi trên marketplace của VS Code / JetBrains.
6. **Bất kỳ công cụ nào không có tùy chọn tắt chia sẻ dữ liệu:**
   - Trong phần cài đặt (Settings / Privacy), nếu bạn **không tìm thấy nút tắt** tùy chọn *"Dùng dữ liệu để huấn luyện"* (*Allow data to be used to train models* / *Training opt-out*), công cụ đó tuyệt đối **không được phép** tiếp cận mã nguồn repo private.

**Kinh nghiệm thực tế:** Mỗi repo của tổ chức đều cung cấp sẵn file `AGENTS.md` / `CLAUDE.md` tóm tắt kiến trúc, bộ lệnh và quy ước code. Bạn nên nạp file này vào ngữ cảnh cho AI đọc trước để kết quả sinh mã tuân thủ đúng chuẩn ngay từ đầu.

---

## 8. Nhịp làm việc

Chương trình vận hành theo chu kỳ sprint **1 tuần**, bắt đầu từ thứ Hai:

| Thời gian | Hoạt động | Hình thức tổ chức |
| --------- | --------- | ----------------- |
| **Thứ 2, buổi tối** | Họp Weekly (45 phút): Tổng kết sprint cũ, thống nhất kế hoạch sprint mới | Voice trên Discord |
| **Hàng ngày** | Standup bất đồng bộ: *Đã làm hôm qua · Dự kiến hôm nay · Vấn đề đang vướng* | Đăng bài tại forum `#standup` |
| **Thứ 3 & Thứ 5, buổi tối** | Họp nhanh squad (sync 15 phút) — *chỉ áp dụng trong 4 tuần đầu* | Voice riêng theo từng squad |
| **Thứ 6** | Seminar kỹ thuật (theo lịch thông báo) | Discord Stage, có ghi hình lưu trữ |
| **Thứ 6 cuối tháng** | **Demo Day:** Mỗi squad trình bày sản phẩm trong 10 phút | Discord Stage, mở cho cộng đồng |

*Khung giờ họp cụ thể sẽ được ấn định dựa trên thời gian rảnh của đa số thành viên đăng ký và thông báo qua tính năng Discord Events.*

**Trường hợp vắng mặt:** Vui lòng để lại tin nhắn xin phép trước tại diễn đàn `#standup`. Nội dung các buổi Weekly và Demo Day đều được ghi chép tóm tắt hoặc lưu video.

---

## 9. Giao tiếp

### Bố trí kênh trao đổi

| Nội dung công việc | Kênh tiếp nhận |
| ------------------ | -------------- |
| Thảo luận kỹ thuật về code, báo cáo lỗi, đề xuất tính năng | **GitHub** (thông qua issue và pull request) |
| Thắc mắc, giải đáp kỹ thuật chung | Forum `#help` trên Discord |
| Đề xuất ý tưởng mới | Forum `#ideas` trên Discord (tối đa 2 ý tưởng/tuần) hoặc issue template **Idea** |
| Báo cáo tiến độ hàng ngày (Standup) | Forum `#standup` trên Discord |
| Trao đổi nội bộ giữa các thành viên cùng nhóm | Kênh riêng `#squad-<tên-game>` |
| Thông báo chung từ ban tổ chức | Kênh `#announcements` |

**Discord là nền tảng liên lạc chính.** Để đảm bảo tính minh bạch và lưu vết thông tin, đội ngũ không sử dụng Zalo, Telegram hay tin nhắn riêng để giải quyết công việc chung — các nội dung trao đổi ngoài GitHub hoặc Discord sẽ không được ghi nhận.

### Quy định ngôn ngữ

- **Trên GitHub:** Tiêu đề issue/PR, tiêu đề commit, code và comment trong code dùng tiếng Anh. Nội dung mô tả issue/PR, phần body của commit và trao đổi trong review **được phép dùng tiếng Việt**.
- **Kênh chung trên Discord:** Tiếng Anh là ngôn ngữ chính; sử dụng kênh `#vn-general` cho các trao đổi bằng tiếng Việt.
- **Trong nội bộ squad:** Thoải mái sử dụng tiếng Việt để trao đổi nhanh.
- **Hệ thống tài liệu:** Repo Hydra SDK duy trì song song 3 ngôn ngữ EN / VI / JA — khi chỉnh sửa tài liệu, bạn cần cập nhật đồng bộ cả ba.

### Cách đặt câu hỏi hiệu quả

1. Dành 15–30 phút chủ động tìm kiếm câu trả lời trước trong README, tài liệu hướng dẫn và các issue đã đóng.
2. Đặt câu hỏi công khai tại kênh `#help`, tránh nhắn tin riêng cho mentor.
3. Cung cấp đầy đủ ngữ cảnh: bạn đang xử lý issue nào, mong muốn đạt kết quả gì, đã thử những cách nào và thông tin lỗi chi tiết (kèm log, ảnh chụp màn hình).

---

## 10. Ghi nhận và lên bậc

### Thang điểm đóng góp

| Hoạt động được ghi nhận | Điểm số |
| ----------------------- | :-----: |
| Pull request được merge thành công — nhãn `size:S` | +1 |
| Pull request được merge thành công — nhãn `size:M` | +3 |
| Pull request được merge thành công — nhãn `size:L` | +5 |
| Pull request phải sửa đổi nhiều hơn 2 vòng review | Điểm PR × 0.5 |
| Báo cáo lỗi được xác nhận (`confirmed`) | +1 *(lỗi nghiêm trọng: +3)* |
| Đề xuất ý tưởng được duyệt đưa vào backlog | +2 |
| Đóng góp review có chất lượng (mang tính xây dựng/phát hiện vấn đề) cho PR của thành viên khác | +1 |
| Vượt qua phần bảo vệ PR | +1 |
| Tham gia thuyết trình tại Seminar hoặc Demo Day | +3 |
| Pull request bị đóng do không điền template hoặc vi phạm giới hạn kích thước | -1 |

Điểm số tập trung đánh giá **chất lượng công việc thực tế**. Việc nộp nhiều PR nhỏ lẻ không mang lại giá trị hoặc đưa ra các ý tưởng sơ sài sẽ không giúp bạn thăng bậc nhanh hơn.

### Tiêu chuẩn lên bậc

| Lộ trình | Điều kiện xét duyệt |
| -------- | ------------------- |
| **X3 → X2** | Có ít nhất 1 báo cáo lỗi hợp lệ được xác nhận, hoặc có 1 PR được merge thành công. |
| **X2 → X1** | Đạt ~10 điểm tích lũy trong 4 tuần; tối thiểu 2 PR được merge; vượt qua bài kiểm tra debug trực tiếp; được mentor đồng thuận; đã hoàn tất ký NDA. |
| **X1 → DevX-Intern** | Do đội ngũ core DevX trực tiếp đề cử dựa trên năng lực và thái độ làm việc thực tế (tối đa duy trì 1 vị trí). |

Đợt xét bậc định kỳ diễn ra trong buổi họp Weekly **đầu mỗi tháng**.

### Quy định trạng thái ngừng hoạt động (Inactive)

Nếu bạn không có bất kỳ tương tác nào trên GitHub hoặc Discord trong **30 ngày liên tục**, tài khoản sẽ chuyển sang trạng thái `inactive` và quyền Write trên các repo sẽ tạm thời được thu hồi. Khi sắp xếp được thời gian quay trở lại, bạn chỉ cần liên hệ với mentor để kích hoạt lại quyền hạn.

---

## 11. Pháp lý và bảo mật

### Hai thỏa thuận pháp lý

| Tiêu chí | Thỏa thuận Đóng góp Mã nguồn (CLA) | Thỏa thuận Bảo mật Thông tin (NDA) |
| -------- | ---------------------------------- | ---------------------------------- |
| **Thời điểm ký** | Ký trực tiếp tại văn phòng ở Tuần 0 | Ký trực tiếp tại văn phòng ở Tuần 0 |
| **Thời điểm có hiệu lực** | Có hiệu lực ngay khi ký | Kích hoạt hiệu lực khi được cấp quyền truy cập repo private (thường từ Tuần 3) |
| **Phạm vi áp dụng** | Áp dụng cho mọi đóng góp mã nguồn | Áp dụng cho các repo private và thông tin nội bộ |
| **Quyền sở hữu trí tuệ** | Bạn **cấp quyền sử dụng** mã nguồn cho VTechcom Labs (theo chuẩn Apache 2.0) | Bạn **chuyển nhượng quyền tài sản** đối với sản phẩm cho VTechcom Labs; bạn vẫn giữ nguyên quyền nhân thân (đứng tên tác giả) |
| **Quyền công bố** | Mã nguồn được phát hành public theo giấy phép Apache 2.0 | Bạn được phép mô tả kinh nghiệm công việc trong CV cá nhân; tuyệt đối không công khai mã nguồn private |

**Quy trình ký thỏa thuận:**
- Ký giấy trực tiếp tại văn phòng VTechcom Labs trong tuần 0 (in 2 bản, mỗi bên giữ 1 bản).
- Người tham gia dưới 18 tuổi bắt buộc phải có chữ ký đồng ý của cha mẹ hoặc người giám hộ hợp pháp.
- Người phụ trách ghi nhận thông tin vào sổ theo dõi contributor (ngày ký, mã bản hợp đồng, GitHub username). Sau khi ghi sổ, tổ chức mới gửi lời mời gia nhập GitHub org.
- *Trường hợp ngoại lệ (ở xa không thể đến văn phòng):* In tài liệu, ký tay trực tiếp, scan hoặc chụp rõ nét gửi về email `haipham@vtechcom.org`, sau đó nộp lại bản gốc khi có dịp thuận tiện.

### Quy tắc an toàn bảo mật bắt buộc

- Bật xác thực 2 lớp (2FA) cho cả GitHub và Discord; tuyệt đối không chia sẻ tài khoản cho người khác.
- **Bảo mật mã nguồn private:** Tuyệt đối không fork về tài khoản cá nhân, không đẩy lên repo bên ngoài, không dán mã vào các trang pastebin, gist công khai hay nạp vào các công cụ AI không được phép.
- **Quản lý thông tin nhạy cảm:** Tuyệt đối không commit các file cấu hình `.env`, secret key, private key, auth token vào git — kể cả thông tin mạng testnet.
- Nếu nghi ngờ hoặc phát hiện sự cố rò rỉ thông tin (kể cả do bản thân sơ suất), bạn cần chủ động thông báo cho đội ngũ core trong vòng **24 giờ**. Sự trung thực và kịp thời luôn được đánh giá cao để khắc phục sự cố.

---

## 12. Quy tắc và kỷ luật

Chương trình tuân thủ nghiêm ngặt [Bộ quy tắc ứng xử (Code of Conduct)](https://github.com/Vtechcom/.github/blob/main/CODE_OF_CONDUCT.md) và **xử lý nghiêm** mọi hành vi vi phạm:

| Mức độ chế tài | Các hành vi vi phạm áp dụng |
| -------------- | --------------------------- |
| 🔴 **Thu hồi quyền ngay lập tức (không cảnh cáo)** | Làm rò rỉ mã nguồn hoặc thông tin bảo mật nội bộ; cố tình truy cập secret hoặc hạ tầng ngoài phạm vi cho phép; sử dụng mã nguồn private sai quy định NDA (bao gồm việc nạp vào công cụ AI cấm); có hành vi quấy rối hoặc vi phạm nghiêm trọng quy tắc ứng xử. |
| 🟠 **Cảnh cáo 1 lần, sau đó hạ bậc** | Cố tình push thẳng vào các nhánh chính (`main` / `master` / `release`); đóng góp mã nguồn khi chưa ký thỏa thuận; nhận issue rồi bỏ dở quá 7 ngày mà không thông báo lý do; không thể giải thích được nội dung mã nguồn của mình khi tham gia bảo vệ PR. |
| ⚪ **Chuyển trạng thái Inactive** | Không có hoạt động đóng góp hay tương tác nào trong vòng 30 ngày liên tục. |

### Quy định hạ bậc chi tiết

- **Đối với thành viên X2 vi phạm mức 🟠:**
  - Bị hạ bậc về **X3 (Tester)**: Thu hồi quyền khỏi team `x2`, không được nhận issue viết code, nhưng vẫn được tham gia test sản phẩm và báo cáo lỗi.
  - Điều kiện quay lại X2: Sau tối thiểu **30 ngày**, phải có ít nhất 1 báo cáo lỗi hợp lệ được xác nhận (`confirmed`) và được mentor phê duyệt.
  - Nếu tiếp tục tái phạm khi đang ở bậc X3: Thu hồi toàn bộ quyền tham gia chương trình.
- **Đối với thành viên X1 vi phạm mức 🟠:**
  - Bị hạ bậc về **X2**: Thu hồi quyền khỏi toàn bộ các repo private. Bạn có trách nhiệm xóa toàn bộ bản sao mã nguồn private trên máy cá nhân trong vòng **7 ngày**. Toàn bộ nghĩa vụ bảo mật theo thỏa thuận NDA đã ký vẫn giữ nguyên hiệu lực.
- **Vi phạm mức 🔴:** Áp dụng thu hồi quyền ngay lập tức đối với mọi cấp bậc.

Kênh tiếp nhận phản ánh vi phạm: Nhắn tin riêng cho các moderator Discord (**Tony**, **ThanhDT**) hoặc gửi email bảo mật tới `haipham@vtechcom.org`. Mọi thông tin phản ánh đều được cam kết giữ kín danh tính.

---

## 13. Khi bạn cần dừng lại

Việc bạn bận việc học tập, thay đổi công việc hoặc đơn giản là muốn tạm dừng đồng hành đều là điều bình thường. Hãy thực hiện quy trình bàn giao văn minh:

1. **Thông báo trước:** Gửi thông báo ngắn gọn tại diễn đàn `#standup` hoặc nhắn tin cho mentor phụ trách.
2. **Bàn giao nhiệm vụ:** Để lại bình luận tóm tắt tiến độ những phần đã làm trên issue đang nhận và chủ động bấm unassign bản thân.
3. **Thực hiện nghĩa vụ NDA:** Nếu đã từng tham gia các repo private, vui lòng xóa toàn bộ bản sao mã nguồn dự án trên máy cá nhân trong vòng **7 ngày** và xác nhận hoàn tất với mentor.

Nếu bạn hoàn tất thủ tục bàn giao đúng quy trình, VTechcom Labs luôn chào đón bạn quay trở lại bất cứ lúc nào. Các quyền bạn đã cấp phép hoặc chuyển nhượng đối với những đóng góp trước đó vẫn tiếp tục duy trì hiệu lực theo đúng thỏa thuận pháp lý.

---

## 14. Câu hỏi thường gặp

**Tôi chưa có kinh nghiệm về blockchain thì có tham gia được không?**  
Hoàn toàn được. Tuần 1–2 bắt đầu từ việc nghiên cứu tài liệu và hoàn thiện các bài test trên Hydra SDK mà không đòi hỏi kiến thức blockchain chuyên sâu. Các buổi seminar và sự hướng dẫn của mentor sẽ giúp bạn tích lũy kiến thức từng bước.

**Nếu mỗi tuần tôi chỉ sắp xếp được khoảng 3–4 giờ thì sao?**  
Bạn vẫn có thể tham gia đóng góp ở bậc X2 trên các repo open source hoặc tham gia các đợt test ở bậc X3. Đối với bậc X1, do làm việc phối hợp theo squad phát triển sản phẩm nên bạn cần cam kết tối thiểu từ 5 giờ/tuần trở lên để không ảnh hưởng đến tiến độ chung của nhóm.

**Tôi có thể ghi nhận các dự án này vào hồ sơ/CV cá nhân không?**  
Có. Đối với repo open source, bạn có thể dẫn đường link đóng góp trực tiếp. Đối với repo private, bạn được phép mô tả vai trò, công nghệ sử dụng và những bài toán kỹ thuật mình đã giải quyết, nhưng tuyệt đối không công khai mã nguồn dự án.

**Tôi phải làm gì nếu pull request chờ review quá lâu?**  
Hãy kiểm tra xem pipeline CI đã pass và bản mô tả PR đã điền đầy đủ các mục theo template hay chưa. Nếu đã quá 48 giờ làm việc mà chưa nhận được phản hồi, bạn hãy nhắn tin nhắc nhở tại kênh `#help` kèm theo đường link PR.

**Tôi có ý tưởng game mới rất thú vị thì đề xuất thế nào?**  
Hãy tạo issue mới theo template **Idea** trên GitHub hoặc chia sẻ tại diễn đàn `#ideas` trên Discord: nêu rõ ý tưởng, lý do phù hợp với nền tảng HydraOne và ước lượng công sức thực hiện. Ý tưởng được duyệt sẽ đưa vào backlog phát triển và được cộng điểm đóng góp.

**Dùng AI hỗ trợ viết phần lớn mã nguồn thì có bị trừ điểm không?**  
Không bị trừ điểm, với điều kiện bạn phải khai báo minh bạch, hiểu rõ từng dòng code và vượt qua buổi bảo vệ PR nếu được chỉ định. Việc che giấu dùng AI hoặc nộp mã nguồn mà không thể giải thích được giải pháp mới là hành vi bị xử lý kỷ luật.

**Nếu tôi vô tình commit nhầm secret/khóa bí mật thì xử lý thế nào?**  
Hãy báo ngay lập tức cho đội ngũ core tại kênh `#help` hoặc nhắn tin riêng cho mentor. **Tuyệt đối không tự ý dùng lệnh git force-push để xóa commit** — các khóa bí mật bị lộ cần được thu hồi (revoke) và cấp mới ngay trên hệ thống máy chủ, việc này sẽ do đội ngũ core trực tiếp xử lý.

---

## 15. Liên hệ

| Vấn đề cần hỗ trợ | Đầu mối liên hệ |
| ----------------- | --------------- |
| Câu hỏi và trao đổi kỹ thuật | Diễn đàn `#help` trên Discord |
| Quản lý công việc trong squad, issue, review PR | Mentor phụ trách trực tiếp của bạn |
| Phản ánh vi phạm quy tắc ứng xử | Moderator Discord (Tony, ThanhDT) hoặc qua email `haipham@vtechcom.org` |
| Báo cáo lỗ hổng bảo mật | Xem hướng dẫn tại [Security policy](https://github.com/Vtechcom/.github/blob/main/SECURITY.md) hoặc gửi email trực tiếp tới `haipham@vtechcom.org` |

---

*Sổ tay được cập nhật định kỳ theo từng đợt hoạt động. Mọi đóng góp chỉnh sửa vui lòng mở issue tại repo [`Vtechcom/.github`](https://github.com/Vtechcom/.github).*