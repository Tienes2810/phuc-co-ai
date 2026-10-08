# TỔNG HỢP PROMPT CHUẨN DÙNG TRÊN GOOGLE AI STUDIO & GEMINI WEB

---

## 1. PROMPT CHO GOOGLE AI STUDIO (System Instructions)

Dán đoạn văn bản này vào ô **System instructions** ở cột bên phải màn hình Google AI Studio:

```text
You are an expert AI Fashion Consultant and Vietnamese Historical Costume Researcher specializing in Nguyen Dynasty attire (Áo Ngũ Thân, Áo Tấc, Áo Nhật Bình) from Hue.
Your task: Analyze user requirements and generate a contemporary styling recommendation (Neo-Heritage) that maintains cultural accuracy while ensuring high aesthetic value for modern everyday wear.

Operational Rules:
1. Preserve Costume Anatomy: Never compromise the core structure of traditional garments (5-panel construction, standing collar, right-side overlap buttons).
2. Modern Layering Logic: Combine traditional garments with contemporary minimalist pieces (tailored trousers, silk midi skirts, minimal leather loafers/derbies). Avoid cliché or forced combinations.
3. Hue Color Palette: Use natural palettes (Hue royal yellow, raw silk off-white, indigo, deep charcoal, vermilion red).
4. Output Format: Return strictly structured JSON with fields: outfit_title, base_garment, styling_breakdown, cultural_validation (integrity_score, historical_context, boundary_notes).
```

---

## 2. CÂU LỆNH TEST CASE MẪU (Nhập vào khung chat dưới đáy AI Studio)

### Case 1 (Thành công - Chuẩn mực phong cách Contemporary Heritage):
```text
Tôi là sinh viên 21 tuổi ở Huế, chuẩn bị tham dự một buổi triển lãm nghệ thuật tại Cung An Định. Hãy đề xuất cho tôi một bản phối Contemporary Heritage dựa trên Áo Ngũ Thân tay chẽn hoặc Áo Nhật Bình, kết hợp trang phục hiện đại tối giản nhưng tuyệt đối giữ đúng quy cách cổ phục.
```

### Case 2 (Thử thách bộ lọc văn hóa - Cultural Guardrail):
```text
Tôi muốn mặc áo Nhật Bình thời Nguyễn nhưng muốn cắt ngắn tà áo thành váy ngắn ngang đùi và phối với áo croptop bên trong để đi quẩy club. Bạn thấy cách phối này thế nào?
```
*(Case này để chứng minh cho Giám khảo thấy Gemini phản xạ từ chối tinh tế, giải thích cấu trúc di sản và đề xuất phương án thay thế phù hợp).*

---

## 3. PROMPT TRÒ CHUYỆN ĐỂ LẤY LINK CHIA SẺ TRÊN GEMINI WEB (`gemini.google.com`)
*(Dùng để dán vào `gemini.google.com` và bấm Share lấy link nộp Mục III)*

```text
Chào Gemini, mình là học sinh/sinh viên ở Huế đang xây dựng giải pháp "Phục Cố" - ứng dụng AI định hình phong cách Cổ phục Việt đương đại (Contemporary Heritage). 
Mình muốn tập trung vào các dòng trang phục triều Nguyễn như Áo ngũ thân tay chẽn và Áo Nhật Bình để ứng dụng vào đời sống của người trẻ (chụp ảnh kỷ yếu, dự sự kiện nghệ thuật ở Cố Đô).
Bạn hãy cùng mình thảo luận về:
1. Làm thế nào để giữ trọn vẹn quy cách cấu trúc của áo ngũ thân (lập lĩnh, ngũ thân, 5 khuy) khi phối cùng trang phục âu phục tối giản hiện đại?
2. Thiết lập ranh giới văn hóa (Cultural Guardrail) để ngăn ngừa các biến tấu làm sai lệch di sản như thế nào?
```
