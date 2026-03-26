# Tách Lớp & Họ Tên — Streamlit App

Công cụ xử lý file Excel: tách cột **Họ và tên** (dạng `12A01-Phạm Vũ Trường An`) thành 2 cột riêng **Họ tên 1** và **Lớp 1**, đồng thời chuẩn hóa mã lớp (bỏ số 0 dẫn đầu sau chữ cái).

## Chức năng
- Upload file `.xlsx` có sheet `Data`
- Tự động tìm cột `Họ và tên`
- Insert 2 cột mới ngay sau cột đó:
  - **Họ tên 1**: phần họ tên (sau dấu `-`)
  - **Lớp 1**: mã lớp đã chuẩn hóa (`12A09` → `12A9`)
- Tải về file output với tên `<tên_file_gốc>_đã tách lớp.xlsx`

## Deploy lên Streamlit Cloud

1. Fork/clone repo này lên GitHub
2. Vào [share.streamlit.io](https://share.streamlit.io) → **New app**
3. Chọn repo, branch `main`, main file: `app.py`
4. Nhấn **Deploy!**

## Chạy local

```bash
pip install -r requirements.txt
streamlit run app.py
```
