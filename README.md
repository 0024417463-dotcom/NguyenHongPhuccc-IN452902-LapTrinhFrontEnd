# EduHub Web — Ch02: CSS hiện đại & Responsive

Bài thực hành chương 2 môn **IN4529 — Lập trình Front End** (Nguyễn Hồng Phúc, Trường Đại học Đồng Tháp).
Tạo kiểu cho 4 trang EduHub Web bằng **CSS thuần**: design token, `@layer`, mobile-first, Grid/Flexbox, nesting, `:has()`, `:user-invalid`, dark mode.

## Chạy

Mở `index.html` bằng Live Server của VS Code, hoặc `npx -y http-server . -p 8080`.

## Cấu trúc

| Tệp | Nội dung |
|---|---|
| `css/main.css` | `@layer tokens, base, layout, components;` + `@import` 4 tệp |
| `css/tokens.css` | Token màu/chữ (`clamp()`)/khoảng cách/bo góc/bóng, dark mode |
| `css/base.css` | Reset, `:where()`, focus-visible, `prefers-reduced-motion` |
| `css/layout.css` | Container, header sticky, footer, hero, `.card-grid`, `.detail` (`grid-template-areas`) |
| `css/components.css` | Nút, card (`:has(.badge--hot)`), FAQ, bảng cuộn ngang, form |

Breakpoint mobile-first: `width >= 40rem` và `width >= 64rem`.

## Kiểm tra đã chạy

- `html-validate "*.html"`: 0 lỗi.
- 4 trang × 375/768/1280 px × sáng/tối: không cuộn ngang.

> Phần challenge ch2-T7 (Tailwind v4) chưa làm.
