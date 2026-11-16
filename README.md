<p align="center">
  <img src="assets/app-icon/hicolor/256x256/apps/ai.storyteller.craft-anything.png" width="128" height="128" alt="Icon ZAC: chữ Z màu cam giữa cặp ngoặc code trên nền xanh đậm">
</p>

<h1 align="center">ZAC – Tái tạo phần mềm</h1>

<p align="center">
  <b>Xem bất kỳ website, ứng dụng hay trò chơi nào hoạt động ra sao, rồi để AI dựng phiên bản của riêng bạn.</b><br>
  Bộ máy mã nguồn mở viết bằng Rust, làm theo nguyên tắc "phòng sạch" (clean-room).
</p>

<p align="center">
  <img alt="100% Rust" src="https://img.shields.io/badge/100%25-Rust-b7410e?style=flat-square&logo=rust">
  <img alt="macOS · Windows · Linux" src="https://img.shields.io/badge/macOS%20%C2%B7%20Windows%20%C2%B7%20Linux-native-2d81ff?style=flat-square">
  <img alt="Giấy phép: MIT hoặc Apache-2.0" src="https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-3a3a3a?style=flat-square">
</p>

> [!NOTE]
> **ZAC – Tái tạo phần mềm** là bản phái sinh (fork) do **zacaiplatform** duy trì, dựa trên
> [Craft Anything](https://github.com/storytold/craft-anything) của đội ngũ ArtCraft.
> Bản này **không** do đội ngũ ArtCraft làm ra, tài trợ hay xác nhận.

## Công dụng

- **Nghiên cứu phần mềm:** website, ứng dụng desktop, ứng dụng điện thoại, trò chơi và tệp tin. Công cụ kiểm tra thật cho biết chúng được dựng ra sao, kèm bằng chứng cho từng câu trả lời.
- **Tự dựng bản của bạn:** nói điều bạn muốn (ví dụ "Tái tạo giao diện website này bằng React"), một coding agent như Claude Code sẽ dựng dự án mới bằng công nghệ bạn chọn.
- **So sánh và sửa dần:** bản dựng được kiểm tra lại với bản gốc, rồi tinh chỉnh tới khi giống.
- **Hai chế độ:**
  - *Clean room* (mặc định): chỉ quan sát từ bên ngoài, như người dùng bình thường.
  - *Deep*: phân tích sâu bên trong file, có thể dùng thêm Ghidra.
- **Chạy được 3 cách:** ứng dụng desktop, dòng lệnh (CLI), và máy chủ MCP để nối với Claude Code / Codex.

## Dùng đúng mục đích

Chỉ phân tích phần mềm **bạn sở hữu hoặc được phép phân tích**. Dùng để học cách một sản phẩm hoạt động và tự viết bản của riêng mình. **Không** dùng để sao chép mã, tài nguyên hay thương hiệu của người khác, và không vượt bản quyền, DRM hay khoá giấy phép.

## Cài đặt

Bản build sẵn và hướng dẫn chi tiết (tiếng Anh) xem tại repo gốc:
https://github.com/storytold/craft-anything#readme

Tự build từ mã nguồn (cần Rust):

```sh
cargo build --release -p craft-anything -p craft-anything-cli
```

## Giấy phép và ghi công

Mã nguồn dùng giấy phép kép [MIT](LICENSE-MIT) hoặc [Apache-2.0](LICENSE-APACHE), tuỳ bạn chọn.
Copyright (c) 2026 ArtCraft Team và những người đóng góp cho Craft Anything ([CONTRIBUTORS.md](CONTRIBUTORS.md)).
Các thông báo bắt buộc nằm trong [NOTICE](NOTICE). Font, icon và tài nguyên đi kèm giữ giấy phép riêng, liệt kê trong [ATTRIBUTION.md](ATTRIBUTION.md).

Bản ZAC dựa trên Craft Anything của đội ngũ ArtCraft. Tên, wordmark và logo ArtCraft là thương hiệu của ArtCraft Team và đã được gỡ khỏi bản fork này.
