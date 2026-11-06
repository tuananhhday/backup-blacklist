# Blacklist Studio — backup

Kho này dành cho snapshot dữ liệu của Blacklist Studio. Chuyển repo sang **Private** trước khi bật backup trong app.

Render cần `GITHUB_BACKUP_REPO=tuananhhday/backup-blacklist`, `GITHUB_BACKUP_BRANCH=main` và secret `GITHUB_BACKUP_TOKEN` có quyền Contents read/write cho repo này. Không ghi token vào Git.

App tạo `snapshots/latest.sqlite3.gz` sau khi backup thành công. File này chứa database SQLite gồm dữ liệu, lịch sử nhãn và bản nháp. Mỗi lần cập nhật tạo commit để giữ lịch sử. Hiện README không chứa dữ liệu người dùng.

Hướng dẫn: https://github.com/tuananhhday/Blacklist/blob/main/BACKUP_SETUP.md
