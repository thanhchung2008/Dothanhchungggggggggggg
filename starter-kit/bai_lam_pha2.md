## 4.2. Trích xuất tin nhắn đặt vé ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "SVT",
    "ngay_su_kien": "2026-12-20",
    "nguoi_lon": 2,
    "tre_em": 1,
    "loai_ve": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "FZ",
    "ngay_su_kien": "2027-01-05",
    "nguoi_lon": 3,
    "tre_em": 0,
    "loai_ve": "thuong",
    "ghi_chu": "hỗ trợ xe lăn"
  },
  {
    "ma_goi": "VIP",
    "ngay_su_kien": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "loai_ve": "vip",
    "ghi_chu": "hỗ trợ tìm chỗ cho người khiếm thị"
  }
]
```

**Link trò chuyện:**https://share.gemini.google/sc7HoQTq4FNh

## 4.3. Báo giá vé bằng Chain-of-Thought

**KET QUA AI**

```text
1. Tiền người lớn:
Nhóm có 5 người lớn, giá gói SVT là 1.200.000 đồng/người lớn: 5 x 1.200.000 = 6.000.000đồng
2. Tiền trẻ em:Trẻ 8 tuổi và 10 tuổi (thuộc nhóm từ 5 đến 11 tuổi) tính 70% giá người lớn: 1.200.000 x 70\% = 840.000 đồng/trẻ em.Bé 3 tuổi (dưới 5 tuổi) được miễn phí (0 đồng).Tổng tiền trẻ em:2 x 840.000) + (1 x 0) = 1.680.000 đồng
3. Tiền vé:6.000.000 + 1.680.000 = 7.680.000 đồng
4. Giảm giá nhóm:
Nhóm có 5 người lớn (đạt điều kiện từ 5 người lớn trở lên) nên được giảm 5% trên tổng tiền vé:Số tiền được giảm: 7.680.000 x 5\% = 384.000 đồng .Tiền vé sau giảm: 7.680.000 - 384.000 = 7.296.000 đồng
5. Phụ thu:
Có 1 người lớn chọn khu ghế ưu tiên với mức phụ thu 300.000 đồng/người (không áp dụng giảm giá):1 x 300.000 = 300.000 đồng
6. Tổng tiền:7.296.000 + 300.000 = 7.596.000 đồng
[RESULT: 7.596.000 đồng]
```

**Link trò chuyện:**https://share.gemini.google/DxJxioifzASE

### b) Kiểm tra kết quả AI

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_khu_vuc",
  "so_khach": 2,
  "so_hiep_bi_anh_huong": 2,
  "tom_tat": "Khán giả mua vé có mái che nhưng bị xếp sang khu không mái trong 2 hiệp đầu gặp trời mưa."
}
```

**Link trò chuyện:**https://share.gemini.google/xrTcoKpkK5hP
