# 🤖 Awesome AI Agent Skills & Toolkits

Bộ sưu tập các kho lưu trữ **Agent Skills** chuyên sâu dành cho các AI Coding Agent (Cursor, Claude Code, Codex, Copilot, Kiro...). Danh sách này bao gồm các bộ kỹ năng tiêu chuẩn từ dựng hình 3D, phát triển Game, Mobile & Engineering Lifecycle cho đến các workflow chuẩn hóa của các kỹ sư hàng đầu.

---

## 📑 Danh Sách Repositories

| Dự án | Lĩnh vực | Mô tả ngắn |
| :--- | :--- | :--- |
| [Blender Skills](#1-blender-skills) | 3D & Technical Art | Bộ kỹ năng tích hợp Blender qua MCP cho AI Agent |
| [GameDev Agent Skills](#2-gamedev-agent-skills) | Game Development | Thư viện 70+ kỹ năng đa engine có auto-router |
| [Android / Full-Lifecycle Skills Library](#3-android--engineering-skills-library) | Android & Software Lifecycle | Thư viện curated skills chuẩn hóa và kiểm duyệt an toàn |
| [Matt Pocock Skills](#4-matt-pocock-skills) | Real Engineering & Architecture | Quy trình TDD, spec-to-tickets, code review cho dev |
| [Addy Osmani Agent Skills](#5-addy-osmani-agent-skills) | Web Performance & Best Practices | Bộ kỹ năng chuẩn hóa quy trình kỹ thuật, audit và web perf |

---

### 1. Blender Skills
* **Tác giả / Repo:** [`arjun988/blender-skills`](https://github.com/arjun988/blender-skills)
* **Lĩnh vực:** Đồ họa 3D, Blender, Technical Art Pipeline
* **Giới thiệu:**
  * Cung cấp gần 100 kỹ năng Blender chuyên sâu kết hợp với giao thức **MCP (Model Context Protocol)**.
  * Hỗ trợ AI Agent can thiệp trực tiếp vào Blender: từ giai đoạn blockout, dựng model, bọc UV, rigging, thiết lập ánh sáng/chất liệu đến tối ưu xuất file (export) sang Unity, Unreal Engine, Godot.
  * Phù hợp khi bạn muốn AI đóng vai trò như một 3D Technical Artist trong đội ngũ.

---

### 2. GameDev Agent Skills
* **Tác giả / Repo:** [`gamedev-skills/awesome-gamedev-agent-skills`](https://github.com/gamedev-skills/awesome-gamedev-agent-skills)
* **Lĩnh vực:** Lập trình Game (Đa nền tảng / Đa Engine)
* **Giới thiệu:**
  * Tập hợp hơn 70 kỹ năng phát triển trò chơi định dạng `SKILL.md` (chuẩn Claude Skills / AI Agent).
  * Điểm nổi bật là có **Master Router**: tự động phân tích file dự án để nhận diện engine (Godot, Unity, Unreal, Phaser, Defold, Raylib, Bevy, v.v.) và bài toán (UI, shader, gameplay mechanics, save system, game feel) để chỉ nạp đúng kỹ năng cần thiết mà không làm quá tải Context Window.
* **Cài đặt nhanh:**
  ```bash
  npx skills add gamedev-skills/awesome-gamedev-agent-skills
  ```

---

### 3. Android & Engineering Skills Library
* **Tác giả / Repo:** [`gptnius/skills-library`](https://github.com/gptnius/skills-library)
* **Lĩnh vực:** Android Development & General Software Lifecycle
* **Giới thiệu:**
  * Kho lưu trữ các bộ skill được chọn lọc cẩn thận (curated layer), kiểm định bảo mật (security-reviewed) phục vụ toàn bộ vòng đời phát triển phần mềm, trong đó có mảng Native Mobile / Android.
  * Giữ nguyên attribution từ tác giả gốc (upstream), tối ưu hóa cấu trúc context và câu lệnh để agent thực thi tác vụ mobile, build và refactor mã nguồn chuẩn xác.

---

### 4. Matt Pocock Skills
* **Tác giả / Repo:** [`mattpocock/skills`](https://github.com/mattpocock/skills)
* **Lĩnh vực:** Software Engineering Discipline, Architecture, TDD
* **Giới thiệu:**
  * Bộ kỹ năng nổi tiếng của Matt Pocock (tác giả Total TypeScript) hướng tới triết lý **"Real Engineering, Not Vibe Coding"**.
  * Chứa các workflow chuẩn mực:
    * `/grill-me`: Phỏng vấn kỹ lưỡng để làm rõ ý tưởng trước khi code.
    * `/to-spec` & `/to-tickets`: Chuyển thảo luận thành đặc tả (spec) và chia nhỏ thành các ticket vừa vặn với Context Window (dưới 140K token "smart zone").
    * `/tdd`: Áp dụng quy trình Red-Green-Refactor nghiêm ngặt.
    * Git guardrails: Ngăn agent tự ý chạy các lệnh nguy hiểm (`git push --force`, `reset --hard`,...).
* **Cài đặt nhanh:**
  ```bash
  npx skills@latest add mattpocock/skills
  ```

---

### 5. Addy Osmani Agent Skills
* **Tác giả / Repo:** [`addyosmani/agent-skills`](https://github.com/addyosmani/agent-skills)
* **Lĩnh vực:** Web Performance, API Design, Code Quality
* **Giới thiệu:**
  * Bộ kỹ năng được thiết kế bởi Addy Osmani (Engineering Lead tại Google Chrome), tập trung vào chất lượng công nghệ web và quy trình chuẩn mực.
  * Các tính năng cốt lõi:
    * **Anti-rationalization Tables:** Bộ quy tắc phản biện các lý do thoái thác của AI (ví dụ: né tránh viết test, bỏ qua spec).
    * Kỹ năng chuyên môn sâu: Tối ưu Web Vitals (`/webperf`), thiết kế REST/GraphQL API (`api-and-interface-design`), dọn dẹp mã nguồn (`/code-simplify`), và quy trình 5 bước gỡ lỗi (`debugging-and-error-recovery`).

---

## 🚀 Cách Sử Dụng Chung

Hầu hết các bộ kỹ năng đều tuân theo chuẩn Agent Skills mở (`SKILL.md`). Bạn có thể tích hợp bằng một trong các cách sau:

1. **Sử dụng CLI `skills`**:
   ```bash
   npx skills add <owner>/<repo>
   ```
2. **Cài đặt Plugin Claude Code**:
   ```bash
   claude plugin install <plugin-name>
   ```
3. **Thủ công (Manual)**: Copy thư mục kỹ năng tương ứng vào thư mục `.agent/skills/` hoặc `.claude/skills/` trong dự án của bạn.

---

## 📄 License
Tất cả các kho lưu trữ trên đều tuân theo giấy phép mã nguồn mở của các tác giả tương ứng. Vui lòng kiểm tra file `LICENSE` tại repo gốc trước khi sử dụng cho môi trường thương mại.
