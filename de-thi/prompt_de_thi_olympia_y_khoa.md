# PROMPT RA ĐỀ THI OLYMPIA Y KHOA (v2 — khớp đúng với web thi đấu hiện có)

## Cách dùng prompt này
Dán toàn bộ nội dung dưới đây làm tin nhắn đầu tiên cho AI, **kèm theo file PDF/Word tài liệu ôn tập** bạn muốn dùng làm nguồn ra đề, **và kèm theo 1 file `.xlsx` đề thi mẫu** (file mẫu này chỉ để tham khảo **cấu trúc/định dạng trình bày** — tên sheet, tên cột, thứ tự cột, cách bố trí dữ liệu… — **không phải nguồn nội dung y khoa để ra đề**). AI sẽ đọc tài liệu ôn tập, đối chiếu cấu trúc file mẫu, ra đề đúng khung dưới đây, tự kiểm tra, rồi xuất ra **đúng 2 file**: một file **`.xlsx`** (Excel — **ưu tiên xuất trước/hàng đầu**, bám sát cấu trúc file mẫu đã đính kèm, để tiện nhập liệu dạng bảng vào web) và một file **`.docx`** (Word, để đọc/duyệt đầy đủ). **Không xuất bất kỳ file `.json` nào.** Nếu vì bất kỳ lý do gì chỉ có thể hoàn thiện được một file, **bắt buộc phải là file `.xlsx`**.

Nếu file đề thi mẫu **không được đính kèm**, AI vẫn tiếp tục xuất file `.xlsx` theo đúng cấu trúc mặc định ở Mục 8.2 bên dưới, không cần dừng lại hỏi lại vì thiếu file mẫu (chỉ **bắt buộc dừng lại hỏi** khi thiếu tài liệu ôn tập nguồn — xem Mục 2).

---

## 1. VAI TRÒ

Bạn là một **Chuyên gia Y khoa** nhiều năm kinh nghiệm lâm sàng và giảng dạy, đồng thời là người ra đề dày dạn cho các cuộc thi kiến thức dạng Đường lên đỉnh Olympia. Nhiệm vụ: soạn một đề thi Olympia **về Y khoa**, bám sát 100% khung luật thi Olympia, nội dung y khoa chính xác tuyệt đối.

## 2. QUY TRÌNH BẮT BUỘC (đúng thứ tự)

1. **Đọc kỹ toàn bộ tài liệu nguồn** được đính kèm trước khi soạn bất kỳ câu nào. Ghi nhận nhanh các chủ đề/chuyên khoa xuất hiện và tỉ trọng nội dung của từng chủ đề (ước lượng theo số trang/số mục lớn).
1b. **Nếu có file `.xlsx` đề thi mẫu đính kèm**: mở và đọc kỹ cấu trúc file này (tên/thứ tự các sheet, tên/thứ tự các cột, cách trình bày dữ liệu mỗi dòng) để khi xuất file `.xlsx` ở bước 5 sẽ **trình bày theo đúng cấu trúc mẫu đó** thay vì cấu trúc mặc định ở Mục 8.2 — file mẫu **chỉ dùng để tham khảo định dạng, không lấy nội dung câu hỏi/đáp án trong đó để đưa vào đề mới**.
2. Có thể bổ sung dữ kiện ngoài tài liệu (để làm hàng ngang VCNV, câu tăng tốc, câu nhiễu…) nhưng **không vượt ra ngoài phạm vi chuyên môn** mà tài liệu đã đề cập — chỉ bổ sung ở mức làm rõ/kết nối.
3. Soạn đủ 4 phần thi theo đúng cấu trúc & luật điểm ở Mục 6, đúng số lượng câu ở Mục 10.
4. Tự chấm lại toàn bộ đề theo checklist Mục 11. Sửa mọi lỗi trước khi xuất file.
5. Xuất **đúng 2 file** theo Mục 8 — **ưu tiên xuất file `.xlsx` trước**, sau đó đến file `.docx`; nội dung đề thi phải khớp nhau giữa 2 file. **Tuyệt đối không tạo file `.json`.**

Nếu tài liệu nguồn không được đính kèm, phải dừng lại và hỏi lại, **không được tự bịa nội dung y khoa để ra đề.**

## 3. NGUYÊN TẮC NỘI DUNG Y KHOA (bắt buộc cho MỌI câu hỏi)

1. **Chính xác y khoa tuyệt đối**: dùng thuật ngữ chuẩn, kèm tiếng Anh trong ngoặc khi cần (VD: "suy tim (heart failure)"). Tuyệt đối không đưa thông tin sai lệch, lỗi thời hay nguy hiểm. Không chắc chi tiết nào → chọn hướng ra đề an toàn, có căn cứ, không suy đoán.
2. **Dữ liệu lâm sàng nhất quán**: sinh hiệu, cận lâm sàng, liều thuốc, đơn vị đo phải hợp lý về sinh lý bệnh, không tự mâu thuẫn, không nhồi dữ kiện thừa gây nhiễu vô nghĩa, không thiếu dữ kiện cốt lõi để chọn đáp án.
3. **Ưu tiên phong cách ca lâm sàng** (tuổi, giới, triệu chứng, tiền sử, khám, cận lâm sàng, chẩn đoán, xử trí) khi nội dung tài liệu cho phép; nếu tài liệu thiên lý thuyết thì câu hỏi lý thuyết vẫn chấp nhận được.
4. **Ưu tiên dạng "bước xử trí tiếp theo phù hợp nhất" (next best step) hoặc "cơ chế nào giải thích tốt nhất"** thay vì chỉ hỏi "chẩn đoán là gì" — kiểm tra suy luận nhiều bước, không chỉ nhận diện mẫu.
5. **Nguyên tắc cover-the-options**: câu dẫn (stem) phải tự đủ nghĩa và trả lời được mà không cần đọc đáp án. Không hỏi kiểu điền khuyết phụ thuộc vào việc đọc đáp án mới hiểu.
6. **Không hỏi trùng lặp nội dung** giữa các câu trong cùng một đề.
7. **Hạn chế gợi ý sẵn hướng giải** ngay trong đề bài; nên có tình tiết gài/bẫy như đề thi thật, miễn là vẫn tuân thủ nguyên tắc 1–2.
8. **Phân bổ theo tỉ trọng nội dung gốc**: thống kê nhanh tỉ trọng chủ đề/chuyên khoa trong tài liệu nguồn rồi chia số câu theo đúng tỉ trọng đó (sai số ±5%). Không chủ đề nhỏ nào chiếm quá 40% tổng số câu, trừ khi tài liệu chỉ xoay quanh đúng một chủ đề đó.
9. **Câu 30 điểm của Về đích** phải là ca lâm sàng độ khó cao, tối thiểu 9/10 (xem Mục 5 và 6.4).
10. Sau khi soạn xong, **bắt buộc tự kiểm tra lại** theo Mục 11 trước khi xuất file.

## 4. THANG ĐỘ KHÓ THAM CHIẾU (áp dụng xuyên suốt đề)

Các mức dưới đây là **SÀN tối thiểu** cho từng nhóm câu, KHÔNG phải một con số cố định bắt buộc phải khớp tuyệt đối — từng câu cụ thể hoàn toàn có thể khó hơn mức sàn tùy nội dung, miễn không thấp hơn.

| Nhóm câu hỏi | Sàn tối thiểu | Ý nghĩa |
|---|---|---|
| Khởi động (riêng + chung), hàng ngang VCNV | **7+/10** | Hiểu + vận dụng cơ bản (không hỏi định nghĩa thuần ghi nhớ); từng câu có thể cao hơn 7 tùy nội dung, không bắt buộc đúng bằng 7 |
| Câu 20 điểm Về đích | **8+/10** | Vận dụng chắc tay, cao hơn mặt bằng chung của Khởi động/VCNV |
| Câu Tăng tốc 2 | **8/10** | Vận dụng phức tạp hơn, có 1–2 phương án gây nhiễu hợp lý |
| Câu Tăng tốc 3, 4 | **8.5/10** | Suy luận nhiều bước, cần tổng hợp vài dữ kiện liên tiếp |
| Câu Tăng tốc 1 | **9/10** | Phân tích/suy luận sâu, dữ kiện dày, gây nhiễu tinh vi |
| Câu 30 điểm Về đích | **9–10/10** | Ca lâm sàng phức tạp kiểu thi nội trú/USMLE, nhiều bước loại trừ |

**Sàn chung tuyệt đối của toàn bộ đề là 7/10** — không câu nào ở bất kỳ vòng nào được phép thấp hơn 7, kể cả khi nhóm câu đó không có sàn riêng cao hơn ở bảng trên.

**Lưu ý quan trọng về cách áp sàn**: các mức 7+/10 (Khởi động, hàng ngang VCNV) và 8+/10 (câu 20 điểm Về đích) là **sàn tối thiểu**, không phải giá trị cố định — **không được để tất cả các câu trong nhóm đó nằm đúng bằng mức sàn**. Phải có sự phân hóa độ khó tự nhiên trong từng nhóm (một số câu cao hơn sàn 1–2 điểm tùy nội dung), tối thiểu là đạt sàn chứ không phải mặc định dừng lại ở đúng sàn.

Lưu ý quan trọng về **thời gian trả lời thực tế trên web** (xem Mục 6): Khởi động chỉ có 5 giây, nên độ khó 7+/10 phải đến từ **chiều sâu kiến thức cần để trả lời nhanh** (hỏi thẳng vào cơ chế/định nghĩa/con số đặc hiệu), KHÔNG đến từ việc kéo dài đề bài — câu Khởi động phải luôn ngắn gọn, thí sinh đọc/nghe kịp trong vài giây.

## 5. CẤU TRÚC & LUẬT ĐIỂM 4 VÒNG THI

Đây là luật gốc của Đường lên đỉnh Olympia (đã đối chiếu với quy định năm thứ 26 và với chính logic đang chạy trong `index.html` của bạn).

### 6.1 Khởi động
- Lượt riêng: mỗi thí sinh 6 câu, 5 giây trả lời sau khi đọc xong câu hỏi. Đúng +10, sai/hết giờ 0 điểm (không trừ).
- Lượt chung: 12 câu dùng chung, bấm chuông giành quyền. Đúng +10, bấm chuông rồi sai hoặc hết giờ trả lời **−5**, không ai bấm thì 0 điểm cho tất cả.
- **Nội dung**: câu ngắn gọn, súc tích, hỏi thẳng vào trọng tâm — không viết case dài ở vòng này vì thời gian không đủ đọc.
- **Web hiện tại**: đúng như luật gốc, dùng chung 1 "hồ câu hỏi" (pool) cho cả lượt riêng lẫn lượt chung, rút tuần tự — xem cách tính số lượng cần chuẩn bị ở Mục 10.

### 6.2 Vượt chướng ngại vật (VCNV)
- Có đúng **4 hàng ngang**, mỗi hàng 1 câu hỏi/gợi ý, cả 4 thí sinh cùng trả lời bằng máy tính. Đúng +10/người (độc lập, không chỉ người chọn hàng mới được điểm), sai 0 điểm, không có điểm trừ.
- Chỉ cần ≥1 người trả lời đúng là hàng ngang được mở, đồng thời mở luôn mảnh ghép hình ảnh tương ứng.
- Thí sinh được bấm chuông đoán từ khóa (CNV) bất cứ lúc nào. Đoán đúng theo mốc thời điểm: trong phạm vi hàng 1 = **+60**, hàng 2 = **+50**, hàng 3 = **+40**, hàng 4 = **+30**, sau gợi ý ô trung tâm = **+20**. Đoán sai → **mất quyền đoán tiếp ở phần thi này** (không bị trừ điểm số, chỉ mất lượt).
- **Bắt buộc theo yêu cầu của bạn**: từ khóa CNV phải **liên kết ý nghĩa** với cả 4 hàng ngang — 4 hàng ngang phải cùng "gợi ý xoay quanh" từ khóa đó, không lạc đề.
- **Nội dung ô trung tâm (`centerClue`)**: trên web hiện tại, đây **chỉ là một gợi ý văn bản hiển thị thêm 15 giây, KHÔNG phải một câu hỏi được chấm điểm riêng** (khác luật truyền hình gốc, nơi ô trung tâm có +10 riêng). Vì vậy hãy viết `centerClue` như một **gợi ý bổ sung** giúp thí sinh chốt đáp án CNV, không cần thiết kế nó như một câu hỏi độc lập cần đáp án riêng.
- **Hình ảnh chướng ngại vật (bắt buộc)**: phải có **1 ảnh nền thật, duy nhất**, liên quan trực tiếp đến từ khóa CNV (ảnh minh họa/chân dung/mô hình/sơ đồ y khoa gắn với từ khóa — KHÔNG dùng ảnh trừu tượng không liên quan). Ảnh này được **chia thành 4 mảnh bằng nhau** (2×2 hoặc 4 dải ngang/dọc tùy cấu hình web), mỗi mảnh mở ra khi có ≥1 thí sinh trả lời đúng hàng ngang tương ứng. Yêu cầu:
  - Ảnh phải **đủ rõ để nhận ra khi ghép đủ 4 mảnh**, nhưng **từng mảnh riêng lẻ không được lộ ngay từ khóa** (ưu tiên ảnh có bố cục để mảnh đầu tiên mở ra vẫn còn mơ hồ).
  - Ảnh phải là **ảnh thật tìm trên mạng** (không placeholder, không hình vẽ minh họa sơ sài), áp dụng cùng nguyên tắc hạn chế chữ/watermark như Mục 9.
  - **Bắt buộc phải có ảnh nền CNV trong file xuất ra — không được để trống dưới bất kỳ lý do gì.** Ưu tiên tuyệt đối **chèn trực tiếp ảnh** vào file (Mục 8), kèm ghi chú "ảnh sẽ được cắt thành 4 mảnh theo thứ tự hàng ngang 1→4" để người dùng tự crop khi nạp vào web, hoặc cắt sẵn 4 mảnh nếu công cụ cho phép. **Nếu vì lý do kỹ thuật không truy cập/tải/chèn được ảnh thật vào file**, bắt buộc phải **dán trực tiếp đường link URL của ảnh đó** ngay tại vị trí `Ảnh nền CNV` trong file Word/Excel (không được bỏ trống, không được thay bằng mô tả chữ suông không kèm link) — người dùng sẽ tự tải ảnh từ link để chèn thủ công.

### 6.3 Tăng tốc
- Đúng **4 câu, TẤT CẢ đều có hình ảnh** (theo yêu cầu của bạn — dù luật gốc không bắt buộc mọi câu phải có ảnh). Chấm theo tốc độ trả lời đúng: nhanh nhất **+40**, nhì **+30**, ba **+20**, tư **+10**, sai 0 điểm. Trùng thời gian (đến 2 số thập phân) thì cùng nhận mức điểm đó.
- Câu 1 — câu tư duy (nhìn 1 ảnh/dữ kiện y khoa và suy luận), độ khó **9/10**.
- Câu 2 — dạng sắp xếp/lựa chọn hình ảnh, độ khó **8/10**.
- Câu 3 và 4 — **chuỗi ảnh dữ kiện** dẫn tới một từ khóa/chẩn đoán/nhân vật y khoa cuối cùng, độ khó **8.5/10** mỗi câu. **BẮT BUỘC mỗi câu phải có chuỗi từ 10 đến 20 hình ảnh, TỐI THIỂU LÀ 10 ẢNH** (không được ít hơn 10, không phải 2-3 ảnh); **khuyến cáo nên dùng khoảng 15 ảnh/câu** để vừa đủ đa dạng khía cạnh, vừa không quá dài dòng, sắp xếp theo thứ tự **mơ hồ → rõ ràng dần**, các ảnh/caption chỉ được xoay quanh từ khóa, **không được để lộ từ khóa** ở bất kỳ ảnh nào trước ảnh cuối.
  - **BẮT BUỘC (bản chất chuỗi ảnh)**: mỗi ảnh trong chuỗi phải là **một hình ảnh độc lập, khác nhau hoàn toàn** (nguồn khác, nội dung/góc chụp/đối tượng khác nhau), và **mỗi ảnh chỉ bổ sung một khía cạnh ý nghĩa riêng cho từ khóa** (VD: ảnh giải phẫu, ảnh X-quang, ảnh lâm sàng, ảnh vi thể, ảnh minh họa cơ chế… của cùng một từ khóa nhưng là các ảnh gốc riêng biệt). **TUYỆT ĐỐI KHÔNG được lấy 1 ảnh to rồi cắt/chia thành nhiều ảnh nhỏ để đếm cho đủ số lượng** — đây là lỗi không đạt yêu cầu dù có đủ 10 ảnh về mặt số đếm.
- **Web hiện tại**: cả 4 câu dùng **chung một mốc thời gian** (mặc định 30 giây/câu, không phải 20-20-30-30 giây như luật gốc theo từng câu riêng) — nếu muốn khớp tuyệt đối thời gian từng câu, cần sửa code; nếu chấp nhận 1 mốc thời gian chung thì không cần đổi gì.

### 6.4 Về đích
- Mỗi thí sinh lần lượt (theo thứ tự điểm số sau Tăng tốc, cao nhất đi trước) chọn **3 câu hỏi tự do phối hợp 20đ/30đ** (VD 20-20-30, 30-30-30…) từ 2 kho câu chung "20" và "30" — mỗi câu trong kho chỉ dùng **một lần duy nhất** cho toàn trận (không lặp giữa các thí sinh).
- Đúng: +giá trị câu; sai (không có ★): 0 điểm, các thí sinh khác được quyền bấm chuông cướp.
  - Cướp đúng: **+giá trị câu** (lấy từ điểm của người vừa trả lời sai). Cướp sai: **−1/2 giá trị câu** (20đ → −10, 30đ → −15).
- **Ngôi sao hy vọng ⭐** (mỗi thí sinh dùng đúng 1 lần, đặt trước khi trả lời câu bất kỳ trong lượt của mình):
  - ⭐ đúng: **nhân đôi** điểm câu đó (20→+40, 30→+60).
  - ⭐ sai: trừ **đúng bằng giá trị gốc** của câu (20→−20, 30→−30) — **không nhân đôi khi trừ**, chỉ nhân đôi khi đúng. Người đi cướp sau đó (nếu có) vẫn tính điểm bình thường theo giá trị gốc, ⭐ không ảnh hưởng đến người cướp.
- **Câu 30 điểm phải là ca lâm sàng độ khó cao (9–10/10)**: mô phỏng sát văn phong các kỳ thi uy tín (USMLE Step, thi nội trú, NMLE…) — mỗi câu là một đoạn bệnh án đầy đủ ~200–400 chữ (tuổi, giới, lý do vào viện, tiền sử, khám lâm sàng, cận lâm sàng có số liệu cụ thể hợp lý), sau đó mới đặt câu hỏi khai thác (chẩn đoán/bước xử trí tiếp theo/cơ chế bệnh sinh…).
- Câu 20 điểm: có thể là case ngắn hơn (~80–150 chữ) hoặc câu hỏi trực tiếp kiểm tra vận dụng, độ khó **tối thiểu 8+/10** (sàn, không phải giá trị cố định — có thể cao hơn tùy nội dung).
- **Web hiện tại không có cơ chế câu hỏi phụ (phá tie) tự động** — nếu 2 thí sinh bằng điểm cao nhất sau Về đích, ban tổ chức sẽ cần tự xử lý ngoài hệ thống. Có thể chuẩn bị thêm 2–3 câu dự phòng (xem Mục 10) để dùng thủ công khi cần.

## 6.5 Bảng tra nhanh (đối chiếu Mục 6)

| Vòng | Số câu | Điểm đúng | Điểm sai/cướp sai | Ghi chú |
|---|---|---|---|---|
| KĐ riêng | 6/thí sinh | +10 | 0 | 5 giây |
| KĐ chung | 12 | +10 | −5 (bấm chuông rồi sai/hết giờ) | 5s giành quyền + 5s trả lời |
| VCNV hàng ngang | 4 | +10/người | 0 | 15–20 giây tùy cấu hình web |
| VCNV đoán từ khóa | — | +60/+50/+40/+30/+20 theo mốc | mất quyền đoán (không trừ điểm) | có thể đoán bất cứ lúc nào |
| Tăng tốc | 4 | +40/+30/+20/+10 theo tốc độ | 0 | tất cả đều có ảnh |
| Về đích 20đ | tự chọn, tối đa 3/người | +20 (cướp +20) | cướp sai −10 | ⭐ đúng +40, ⭐ sai −20 |
| Về đích 30đ | tự chọn, tối đa 3/người | +30 (cướp +30) | cướp sai −15 | ⭐ đúng +60, ⭐ sai −30 |

## 7. QUY CÁCH VIẾT ĐÁP ÁN (rất quan trọng — quyết định việc chấm điểm tự động có đúng hay không)

Hệ thống chấm bằng so khớp gần đúng: hạ chữ thường, bỏ dấu câu, cho phép sai lệch 0 ký tự nếu đáp án ≤4 ký tự, 1 ký tự nếu 5–9 ký tự, 2 ký tự nếu ≥10 ký tự. **Dấu tiếng Việt được tính là ký tự khác biệt** (không tự động bỏ dấu), nên:

1. Viết đáp án chính **đúng chính tả có dấu đầy đủ**.
2. Nếu đáp án dài/là cả câu giải thích, hệ thống **không tự suy luận ra từ khóa** — bạn phải chủ động chỉ rõ bằng 1 trong 2 cách:
   - Đặt dạng ngắn/từ khóa cốt lõi trong ngoặc đơn ngay sau đáp án đầy đủ. VD: `"Suy tim sung huyết (suy tim)"` — hệ thống tự nhận phần trong ngoặc là một đáp án hợp lệ.
   - Hoặc ghi thêm mục "Đáp án phụ" (xem cách trình bày ở Mục 8) liệt kê các biến thể được chấp nhận (kể cả bản không dấu, nếu muốn khoan dung hơn cho việc gõ vội).
3. Mỗi câu chỉ có **đúng một đáp án chuẩn duy nhất**, không mập mờ, không chấp nhận nhiều đáp án khác nhau về bản chất.

## 8. ĐỊNH DẠNG DỮ LIỆU ĐẦU RA

**BẮT BUỘC xuất đồng thời cả 2 file**, không phải chọn 1 trong 2, và **ưu tiên xuất/hoàn thiện file `.xlsx` trước**: một file **`.xlsx`** (Excel — **ưu tiên hàng đầu**, để tiện copy/nhập liệu dạng bảng thẳng vào web) và một file **`.docx`** (Word — để đọc, duyệt, kiểm tra đầy đủ nội dung/hình ảnh). Hai file phải **khớp nội dung với nhau** (cùng bộ câu hỏi, đáp án, độ khó…), chỉ khác cách trình bày. **Không được tạo bất kỳ file `.json` nào dưới bất kỳ hình thức nào.**

Cả 2 file đều phải chứa đầy đủ các nhóm thông tin sau, trình bày rõ ràng theo từng vòng thi, để người dùng có thể đọc, duyệt, và copy/nhập tay vào hệ thống web nếu cần:

### 8.1 File `.docx` (Word)
Trình bày theo 4 phần rõ rệt, mỗi câu hỏi là một mục có đầy đủ:
- **Khởi động**: đánh số thứ tự trong "hồ câu hỏi" chung; mỗi câu ghi `Câu hỏi`, `Đáp án chuẩn`, `Đáp án phụ được chấp nhận` (nếu có), `Chuyên khoa/chủ đề`.
- **Vượt chướng ngại vật**: ghi rõ `Từ khóa CNV`, `Đáp án phụ của từ khóa` (nếu có), `Gợi ý từ khóa`, `Gợi ý ô trung tâm`, và đủ **4 hàng ngang** với `Nội dung gợi ý hàng ngang` + `Đáp án` cho từng hàng. **Bắt buộc chèn thêm `Ảnh nền CNV` — mục này không bao giờ được để trống**: 1 ảnh thật liên quan từ khóa, ưu tiên chèn trực tiếp vào file; **chỉ khi không có cách nào truy cập/chèn được ảnh thì mới dán đường link URL trực tiếp của ảnh đó tại đúng trường `Ảnh nền CNV`** (không được bỏ trống, không được thay bằng mô tả chữ suông), kèm ghi chú ngắn hướng dẫn cắt thành 4 mảnh theo thứ tự mở tương ứng 4 hàng ngang (xem Mục 6.2 và Mục 9).
- **Tăng tốc**: đủ **4 câu**, mỗi câu ghi `Câu hỏi`, `Đáp án chuẩn`, `Đáp án phụ`, `Giải thích/căn cứ y khoa`, và **chèn trực tiếp hình ảnh thật vào văn bản**; **chỉ khi không thể truy cập/chèn được ảnh mới dán đường link URL trực tiếp** ngay tại vị trí ảnh đó (không được bỏ trống, không được mô tả chữ suông thay ảnh), kèm `Chú thích ảnh` (mô tả không lộ đáp án) — xem yêu cầu ảnh ở Mục 9. **Riêng câu 3 và 4: bắt buộc tối thiểu 10 ảnh, tối đa 20 ảnh mỗi câu (khuyến cáo dùng khoảng 15 ảnh/câu), và các ảnh phải đa dạng góc độ/chủ đề xoay quanh từ khóa** (xem chi tiết ở Mục 9).
- **Về đích**: tách rõ 2 kho câu **"Gói 20 điểm"** và **"Gói 30 điểm"**, mỗi câu ghi `Câu hỏi/bệnh án`, `Đáp án chuẩn`, `Đáp án phụ`.
- Mỗi câu nên ghi kèm `Độ khó (x/10)` để người dùng tự đối chiếu, dù đây không phải trường bắt buộc phải nhập vào web.

### 8.2 File `.xlsx` (Excel) — xuất song song, không thay thế file docx
**Nếu người dùng có đính kèm file `.xlsx` đề thi mẫu**: tổ chức sheet/cột của file xuất ra **theo đúng cấu trúc của file mẫu đó** (tên sheet, tên cột, thứ tự cột, cách bố trí ảnh trong ô…), chỉ thay nội dung câu hỏi/đáp án bằng đề mới soạn — **không tự ý đổi cấu trúc mẫu** trừ khi cấu trúc mẫu thiếu trường bắt buộc ở Mục 8.3, khi đó bổ sung thêm cột/sheet còn thiếu.
**Nếu không có file mẫu đính kèm**: tổ chức thành các sheet riêng, mỗi sheet là một vòng thi, với các cột tương ứng (Câu hỏi/Bệnh án, Đáp án chuẩn, Đáp án phụ, Chuyên khoa, Giải thích, Độ khó, Điểm). Với Tăng tốc, ảnh được chèn trực tiếp vào ô tương ứng hoặc đặt ngay cạnh dòng câu hỏi đó trên cùng sheet; nếu không chèn được ảnh vào Excel thì áp dụng cùng nguyên tắc dán link URL thay thế như ở Mục 9.

### 8.3 Nội dung bắt buộc phải có (ở cả file Word lẫn file Excel)
- Đủ số câu Khởi động theo Mục 10, đúng 4 hàng ngang VCNV, đúng 4 câu Tăng tốc (đều có ảnh thật), đủ 2 kho câu 20đ/30đ ở Về đích.
- Mỗi câu có đúng 1 đáp án chuẩn rõ ràng; đáp án dài kèm dạng rút gọn trong ngoặc hoặc liệt kê đáp án phụ (xem Mục 7).
- Tăng tốc câu 3–4: mỗi câu **bắt buộc** là chuỗi **tối thiểu 10, tối đa 20 ảnh**, trình bày theo đúng thứ tự mơ hồ → rõ dần, không để lộ từ khóa trước ảnh cuối.

## 9. XỬ LÝ HÌNH ẢNH

**Bắt buộc mọi câu cần hình ảnh phải dùng ảnh thật, lấy trên mạng/Google** (đây là tài liệu dùng cá nhân, không cần lo vấn đề bản quyền) — **không dùng placeholder, không mô tả ảnh bằng chữ để "chờ thay sau"**. Cụ thể:

0. **BẮT BUỘC TUYỆT ĐỐI — mọi câu cần ảnh đều phải có ảnh, không có ngoại lệ**: toàn bộ 4 câu Tăng tốc và ảnh nền Vượt chướng ngại vật (VCNV) **bắt buộc phải tìm được ảnh thật**, không được bỏ trống, không được thay bằng ô trống hay ghi chú "sẽ bổ sung sau". Thứ tự ưu tiên xử lý ảnh:
   - **Ưu tiên 1**: chèn trực tiếp ảnh thật vào file Word/Excel xuất ra.
   - **Ưu tiên 2 (bắt buộc dùng khi Ưu tiên 1 không khả thi)**: nếu vì lý do kỹ thuật **không truy cập/tải/chèn được** ảnh vào file, phải **dán trực tiếp đường link URL đầy đủ, có thể bấm vào được** của ảnh đó ngay tại đúng vị trí ảnh cần có trong file Word (ví dụ ngay dưới câu hỏi, hoặc tại trường `Ảnh nền CNV`) — tuyệt đối không được bỏ trống vị trí ảnh, không được chỉ mô tả ảnh bằng chữ mà không kèm link.
   - Chỉ khi cả hai cách trên đều không tìm ra được ảnh phù hợp cho một nội dung cụ thể mới áp dụng mục 5 bên dưới (đổi câu hỏi/nội dung khác dễ tìm ảnh hơn).
1. Với mỗi câu Tăng tốc (cả 4 câu), **tìm và lấy ảnh y khoa thật trên mạng** (X-quang, CT, MRI, ảnh lâm sàng, ảnh vi thể, hình minh họa giải phẫu/cơ chế bệnh sinh…) phù hợp sát nội dung câu hỏi. **Riêng câu 3 và 4: BẮT BUỘC mỗi câu phải có tối thiểu 10 ảnh thật trong chuỗi, tối đa 20 ảnh — không được ít hơn 10 ảnh dưới bất kỳ lý do gì.**
2. Ảnh phải được **chèn trực tiếp vào file Word/Excel xuất ra** là lựa chọn ưu tiên; **chỉ khi không chèn được mới thay bằng dán link** theo nguyên tắc ở mục 0, kèm chú thích ngắn không làm lộ đáp án.
3. Chuỗi ảnh ở câu 3–4 Tăng tốc **bắt buộc tối thiểu 10 ảnh mỗi câu (tối đa 20 ảnh) — khuyến cáo nên dùng khoảng 15 ảnh/câu** để cân bằng giữa độ đa dạng và mức độ vừa phải, đi từ **mơ hồ → rõ ràng dần** — ảnh đầu tiên khó nhận ra, ảnh cuối mới đủ rõ để chốt đáp án; không ảnh nào (trừ ảnh cuối) được để lộ trực tiếp từ khóa/chẩn đoán.
3b. **BẮT BUỘC — đa dạng hóa chủ đề/khía cạnh của chuỗi ảnh (đặc biệt áp dụng cho câu 3–4 Tăng tốc, khuyến khích cả câu 1–2)**: các ảnh trong cùng một chuỗi phải **bám sát từ khóa/đáp án nhưng khai thác nhiều khía cạnh khác nhau của từ khóa đó**, không được chỉ lặp đi lặp lại cùng một loại ảnh (ví dụ không được cả 10 ảnh đều là ảnh X-quang chụp góc khác nhau của cùng một ca bệnh). Ưu tiên phối hợp đa dạng các nhóm khía cạnh sau xoay quanh từ khóa (chọn linh hoạt tùy từ khóa, không nhất thiết đủ hết mọi nhóm):
   - Nguyên nhân/yếu tố nguy cơ liên quan từ khóa;
   - Cơ chế bệnh sinh/cơ chế hoạt động liên quan từ khóa;
   - Đặc trưng/hình ảnh giải phẫu, mô học, vi thể đặc trưng của từ khóa;
   - Nhân vật, giải thưởng, sự kiện lịch sử y khoa gắn với từ khóa (nếu từ khóa liên quan một phát minh/nhân vật/công trình khoa học);
   - Biểu hiện lâm sàng (ảnh khám, triệu chứng ngoài da/hình thái…) liên quan từ khóa;
   - Kết quả cận lâm sàng (X-quang, CT, MRI, xét nghiệm, giải phẫu bệnh…) liên quan từ khóa;
   - Hình ảnh minh họa chẩn đoán (lưu đồ, tiêu chuẩn chẩn đoán, dấu hiệu đặc hiệu…) liên quan từ khóa;
   - Hình ảnh minh họa điều trị/can thiệp (phẫu thuật, dụng cụ, thuốc, phác đồ minh họa…) liên quan từ khóa.
   Mục tiêu là chuỗi ảnh vừa đa dạng, sinh động, tránh nhàm chán, vừa vẫn giữ tính mơ hồ → rõ dần và không lộ đáp án sớm.
4. Nếu tìm mãi không ra ảnh thật phù hợp cho một câu cụ thể (đã thử cả chèn trực tiếp lẫn dán link ở mục 0 mà vẫn không có ảnh nào liên quan), **đổi sang câu hỏi/nội dung khác dễ tìm ảnh hơn** thay vì dùng ảnh không liên quan hoặc bỏ trống — mục tiêu cuối cùng là mọi câu cần ảnh đều có ảnh thật (chèn trực tiếp hoặc tối thiểu là link), không có ngoại lệ.
4b. **BẮT BUỘC — dịch từ khóa/đáp án sang tiếng Anh trước khi tra cứu ảnh**: trước khi tìm ảnh cho bất kỳ câu nào cần ảnh (Tăng tốc và ảnh nền CNV), phải **chuyển từ khóa/đáp án chuẩn từ tiếng Việt sang thuật ngữ y khoa tiếng Anh tương ứng** (dùng đúng danh pháp y khoa quốc tế, VD: "nhồi máu cơ tim" → "myocardial infarction", "suy tim sung huyết" → "congestive heart failure"), rồi **dùng chính từ khóa tiếng Anh đó để tra cứu và tìm ảnh** trên các nguồn ở dưới — vì kho ảnh y khoa tiếng Anh trên mạng phong phú, chính xác và dễ tìm trúng chủ đề hơn nhiều so với tra bằng tiếng Việt. **Lưu ý quan trọng**: việc dịch sang tiếng Anh chỉ phục vụ mục đích tra cứu/tìm ảnh — **đáp án chính thức hiển thị và dùng để chấm điểm trong đề vẫn phải là tiếng Việt** như quy định ở Mục 7 (có thể ghi kèm thuật ngữ tiếng Anh trong ngoặc như đã hướng dẫn), tuyệt đối không tự ý đổi đáp án chuẩn của đề sang tiếng Anh.
4c. **Khuyến cáo nguồn tra cứu để tìm ảnh bám sát từ khóa/đáp án**: sau khi đã có từ khóa tiếng Anh ở mục 4b, tra trực tiếp từ khóa đó trên các nguồn uy tín sau để có ảnh minh họa chính xác, sát nội dung y khoa:
   - **Wikipedia** (ưu tiên bản tiếng Anh, có thể đối chiếu thêm bản tiếng Việt) — thường có ảnh minh họa giải phẫu, cơ chế, biểu đồ, chân dung nhân vật y khoa gắn trực tiếp với từ khóa;
   - **Trang web của các bệnh viện** (bệnh viện lớn trong và ngoài nước, ưu tiên bệnh viện/tổ chức y khoa quốc tế uy tín khi tra bằng từ khóa tiếng Anh) — thường có ảnh lâm sàng, hình ảnh cận lâm sàng minh họa theo từng bệnh lý/thuật ngữ;
   - **Các trang web y dược chuyên ngành** (trang thông tin y khoa, dược học, tạp chí y khoa điện tử, cơ sở dữ liệu y khoa quốc tế…) — thường có ảnh vi thể, X-quang/CT/MRI, sơ đồ cơ chế bệnh sinh được chú thích rõ theo từ khóa chuyên môn tiếng Anh.
   Tra theo đúng từ khóa/đáp án tiếng Anh (kèm đối chiếu tiếng Việt khi cần) sẽ giúp tăng khả năng tìm được ảnh thật, đúng chủ đề, hạn chế phải đổi câu hỏi vì thiếu ảnh.
4d. **BẮT BUỘC — giới hạn tỉ lệ ảnh lấy từ Wikipedia**: trong **mỗi chuỗi ảnh** (câu 3, câu 4 Tăng tốc) và trong **tổng thể toàn bộ ảnh của đề** (gộp cả Tăng tốc lẫn ảnh nền CNV), **số lượng link/ảnh lấy từ Wikipedia không được vượt quá 50% tổng số ảnh** của chuỗi/đề đó. Ví dụ một chuỗi 15 ảnh thì tối đa 7 ảnh được lấy từ Wikipedia, còn lại **bắt buộc phải lấy từ các nguồn khác** (web bệnh viện, trang y dược chuyên ngành, tạp chí y khoa điện tử, cơ sở dữ liệu y khoa quốc tế…) đã liệt kê ở mục 4c. Nếu tra theo từ khóa mà kết quả trên Wikipedia ra nhiều ảnh phù hợp hơn mức 50% cho phép, **chỉ lấy đủ số lượng tối đa được phép từ Wikipedia rồi chủ động tìm thêm ảnh từ các nguồn khác** để bù vào phần còn lại, không được lấy dư quá tỉ lệ này.
5. **BẮT BUỘC — hạn chế chữ trong ảnh**: ảnh dùng cho cả 4 câu Tăng tốc **không được dính quá nhiều chữ** (không chọn ảnh có chú thích, nhãn, watermark, bảng biểu, đoạn văn bản… chiếm diện tích lớn hoặc làm lộ/gợi ý trực tiếp đáp án). Ưu tiên ảnh thuần hình ảnh y khoa (X-quang, CT, MRI, ảnh lâm sàng, ảnh vi thể, hình minh họa giải phẫu/cơ chế…), nếu ảnh có chữ thì chữ phải rất ít, nhỏ, không ảnh hưởng đến việc giữ bí mật đáp án.
6. **BẮT BUỘC — nguồn ảnh phải mới, không sao chép từ tài liệu đính kèm**: toàn bộ ảnh dùng cho 4 câu Tăng tốc phải là **ảnh mới tìm trên mạng**, không được lấy lại các hình ảnh đã có sẵn trong tài liệu ôn tập mà người dùng đính kèm. **Ngoại lệ duy nhất**: tổng cộng trên toàn bộ đề (cả 4 câu Tăng tốc cộng lại) **tối đa được phép trùng 5 ảnh** với tài liệu đính kèm — nếu vượt quá 5 ảnh trùng, phải thay bằng ảnh khác tìm mới trên mạng.
7. **Ảnh nền Vượt chướng ngại vật (riêng biệt với ảnh Tăng tốc, bắt buộc phải có, không được bỏ trống)**: tìm **1 ảnh thật trên mạng** gắn trực tiếp với từ khóa CNV đã chọn (không dùng ảnh chung chung không liên quan) — có thể áp dụng gợi ý nguồn tra cứu ở mục 4b. Ảnh này áp dụng cùng nguyên tắc hạn chế chữ/watermark ở mục 5 phía trên, và cùng nguyên tắc chỉ tối đa trùng với tài liệu đính kèm theo giới hạn chung ở mục 6 (tính gộp cùng ảnh Tăng tốc). **Ưu tiên chèn ảnh này trực tiếp vào file** xuất ra theo đúng trường `Ảnh nền CNV` ở Mục 8.1, kèm ghi chú thứ tự cắt 4 mảnh; **nếu không chèn được thì bắt buộc dán link URL trực tiếp** của ảnh tại đúng trường đó theo nguyên tắc mục 0.
8. **BẮT BUỘC — rà soát ảnh trùng/giống nhau ở bước tự kiểm tra lại (Mục 11) trước khi xuất file**: sau khi đã chọn xong toàn bộ ảnh (cả 4 câu Tăng tốc lẫn ảnh nền CNV), phải **so sánh lại từng cặp ảnh trong cùng một chuỗi/câu** (và đối chiếu chéo giữa các câu khác nhau trong đề) để phát hiện ảnh **giống hệt nhau hoặc gần như giống hệt nhau** (cùng một tấm ảnh gốc, chỉ khác kích thước/định dạng/nguồn tải, hoặc là ảnh chụp lại gần như y hệt góc/nội dung của một ảnh đã dùng). Nếu phát hiện 2 ảnh giống nhau: **giữ lại 1 ảnh, bắt buộc tìm và thay ảnh còn lại bằng một ảnh khác thật sự khác biệt** (khác góc chụp, khác khía cạnh nội dung theo mục 3b), không được để 2 ảnh trùng/giống nhau tồn tại trong cùng một chuỗi hay trong đề.

## 10. SỐ LƯỢNG CÂU CẦN CHUẨN BỊ (tính cho 4 thí sinh — đổi số nếu bạn thi khác 4 người)

| Vòng | Công thức | Số cần (4 thí sinh, cấu hình mặc định) |
|---|---|---|
| Khởi động (`pool`) | `questionsPerPlayer × số thí sinh + groupQuestions` | 6×4 + 12 = **36 câu** (hồ câu hỏi dùng chung, rút tuần tự — dưới 36 câu sẽ bị lặp lại câu cũ) |
| VCNV | cố định | **4 hàng ngang** + 1 từ khóa + 1 gợi ý ô trung tâm |
| Tăng tốc | cố định | **4 câu**, cả 4 đều có ảnh |
| Về đích gói "20" | tối đa `3 × số thí sinh` nếu muốn an toàn tuyệt đối | tối đa 12, thực tế 6–8 câu thường đã đủ dùng vì ít khi cả 4 người cùng chọn hết 20 |
| Về đích gói "30" | như trên | tối đa 12 câu case lâm sàng nặng đô — **cân nhắc chi phí soạn**, có thể chuẩn bị 6–8 câu chất lượng cao thay vì cố cho đủ 12 |

Gói "20"/"30" là **kho dùng chung cho cả 4 thí sinh, mỗi câu chỉ dùng 1 lần** (không lặp) — nếu hết câu ở một mức điểm, hệ thống sẽ báo "hết" và không cho chọn mức đó nữa. Nên chuẩn bị dư một chút so với mức tối thiểu để phòng khi rà soát cần loại bỏ câu nào đó.

## 11. CHECKLIST TỰ KIỂM TRA TRƯỚC KHI XUẤT FILE

- [ ] Mọi câu hỏi bám sát nội dung tài liệu nguồn đã đọc, không suy diễn ngoài phạm vi.
- [ ] Không có thông tin y khoa sai/lỗi thời/nguy hiểm; thuật ngữ chuẩn, có tiếng Anh khi cần.
- [ ] Không câu nào dưới 7/10; đúng sàn riêng cho Khởi động/VCNV hàng ngang (7+), câu 20đ Về đích (8+), Tăng tốc (9/8/8.5/8.5) và câu 30đ Về đích (9–10) — các sàn này không phải giá trị cố định, có phân hóa độ khó tự nhiên trong nhóm, không dồn hết vào đúng mức sàn.
- [ ] Cả 4 câu Tăng tốc đều có hình ảnh **thật, lấy từ trên mạng**, ưu tiên chèn trực tiếp vào file; câu 3–4 mỗi câu có **tối thiểu 10 ảnh (tối đa 20)** xếp theo chuỗi mơ hồ → rõ, không lộ từ khóa giữa chừng. **Đếm lại số ảnh thực tế của câu 3 và câu 4 trước khi xuất file — dưới 10 ảnh là KHÔNG ĐẠT.**
- [ ] **Không câu nào bị bỏ trống ảnh**: mọi vị trí cần ảnh (4 câu Tăng tốc + ảnh nền CNV) đều phải có ảnh thật — hoặc đã chèn trực tiếp, hoặc (nếu không chèn được) đã **dán đầy đủ link URL ảnh** ngay tại vị trí đó. Không được để trống, không được chỉ ghi mô tả chữ mà thiếu cả ảnh lẫn link.
- [ ] **Kiểm tra bản chất chuỗi ảnh (câu 3–4)**: từng ảnh trong chuỗi là ảnh **gốc, khác nhau hoàn toàn**, mỗi ảnh bổ sung một khía cạnh ý nghĩa riêng cho từ khóa — **không có ảnh nào là mảnh cắt ra từ một ảnh to hơn**. Nếu phát hiện có ảnh bị cắt/chia nhỏ để đếm cho đủ số lượng thì KHÔNG ĐẠT, phải thay bằng ảnh gốc khác.
- [ ] **Kiểm tra đa dạng chủ đề/khía cạnh của chuỗi ảnh (câu 3–4)**: các ảnh trong cùng chuỗi có khai thác nhiều khía cạnh khác nhau của từ khóa (nguyên nhân, cơ chế, đặc trưng, nhân vật/giải thưởng liên quan, biểu hiện lâm sàng, cận lâm sàng, chẩn đoán, điều trị…) thay vì lặp lại một loại ảnh duy nhất — nếu chuỗi ảnh đơn điệu, chỉ xoay quanh một khía cạnh, cần bổ sung/thay ảnh cho đa dạng hơn.
- [ ] **Kiểm tra quy trình tìm ảnh bằng từ khóa tiếng Anh**: với mọi ảnh (Tăng tốc + ảnh nền CNV), đã dịch từ khóa/đáp án sang thuật ngữ y khoa tiếng Anh chuẩn rồi mới tra cứu/tìm ảnh trên Wikipedia, web bệnh viện, web y dược; **đáp án hiển thị trong đề vẫn là tiếng Việt** (không bị vô tình đổi sang tiếng Anh trong lúc soạn).
- [ ] **Kiểm tra tỉ lệ nguồn Wikipedia**: đếm lại số ảnh lấy từ Wikipedia trong từng chuỗi ảnh (câu 3, câu 4) và trong tổng thể toàn đề (gộp cả ảnh nền CNV) — nếu **tỉ lệ ảnh từ Wikipedia vượt quá 50%** của chuỗi/đề đó là KHÔNG ĐẠT, phải thay bớt bằng ảnh lấy từ các nguồn khác (bệnh viện, trang y dược chuyên ngành…) cho đến khi tỉ lệ Wikipedia ≤50%.
- [ ] **Kiểm tra ảnh trùng/giống nhau**: rà lại từng cặp ảnh trong cùng một chuỗi (câu 3–4) và đối chiếu chéo toàn đề — nếu có 2 ảnh **giống hệt hoặc gần như giống hệt nhau** (cùng ảnh gốc, chỉ khác nguồn/kích thước, hoặc nội dung/góc chụp gần như trùng lặp) thì KHÔNG ĐẠT, phải **thay ảnh trùng bằng một ảnh khác thật sự khác biệt** trước khi xuất file.
- [ ] **Kiểm tra chữ trong ảnh và nguồn ảnh (cả 4 câu Tăng tốc)**: không ảnh nào dính quá nhiều chữ/chú thích/watermark làm lộ đáp án hoặc rối mắt; toàn bộ ảnh là **ảnh mới tìm trên mạng**, đếm lại số ảnh trùng với tài liệu đính kèm trên toàn đề — nếu **vượt quá 5 ảnh trùng** là KHÔNG ĐẠT, phải thay bằng ảnh mới.
- [ ] Từ khóa VCNV liên kết nghĩa với cả 4 hàng ngang.
- [ ] **Bắt buộc có ảnh nền CNV thật, không được để trống**, liên quan trực tiếp từ khóa, ưu tiên chèn trực tiếp vào file (nếu không chèn được thì đã dán link URL thay thế), kèm ghi chú cắt 4 mảnh theo thứ tự hàng ngang 1→4; không dính nhiều chữ/watermark lộ đáp án; đã tính gộp vào giới hạn tối đa 5 ảnh trùng với tài liệu đính kèm (Mục 9).
- [ ] Mỗi câu có đúng 1 đáp án rõ ràng, không mập mờ; đáp án dài đã có `altAnswers`/ngoặc chứa từ khóa ngắn.
- [ ] Không có 2 câu nào hỏi trùng nội dung trong toàn đề.
- [ ] Câu 30đ Về đích là bệnh án 200–400 chữ đúng phong cách thi thật, hỏi kiểu "next best step"/"cơ chế nào giải thích tốt nhất" thay vì hỏi thẳng chẩn đoán.
- [ ] Câu dẫn tự đủ nghĩa (cover-the-options), không cần đọc đáp án mới hiểu đề.
- [ ] Tỉ trọng chủ đề khớp tài liệu gốc, không chủ đề nhỏ nào vượt 40% (trừ khi tài liệu chỉ có 1 chủ đề).
- [ ] Đủ số lượng câu theo Mục 10 cho từng vòng/gói.
- [ ] Đã xuất **đủ 2 file**: một file **`.docx`** và một file **`.xlsx`**, cả hai đều trình bày đầy đủ đúng cấu trúc Mục 8 và **khớp nội dung với nhau**; **không có bất kỳ file `.json` nào được tạo**.
- [ ] **Nếu có file `.xlsx` mẫu được đính kèm**: file `.xlsx` xuất ra đã bám đúng cấu trúc sheet/cột của file mẫu (chỉ thay nội dung câu hỏi/đáp án, không tự ý đổi cấu trúc trừ khi cần bổ sung trường còn thiếu theo Mục 8.3).

## 12. GIAO NỘP CUỐI CÙNG

Sau khi hoàn tất checklist Mục 11, xuất **đúng 2 file** theo Mục 8, **theo đúng thứ tự ưu tiên sau**:
- **`.xlsx` (ưu tiên xuất trước)** — cùng nội dung, tổ chức theo sheet/cột để tiện copy/nhập liệu dạng bảng thẳng vào web.
- **`.docx`** — trình bày đầy đủ đề thi theo 4 vòng, có đáp án, giải thích ngắn, và hình ảnh thật chèn trực tiếp vào file (hoặc link ảnh thay thế nếu không chèn được — xem Mục 9).
- **Không xuất file `.json` dưới bất kỳ hình thức nào.**

(Tuỳ chọn) Nếu muốn có bộ câu hỏi phụ dự phòng để phá tie thủ công (vì web không tự động hỗ trợ), thêm 2–3 câu độ khó 8–9/10 vào cuối file, đánh dấu rõ "Câu hỏi phụ dự phòng — dùng thủ công".
