# Test Case Report

**Layihə:** Cars API

**Modul:** POST `/cars`

## Mühit (Environment)

- **Alət:** Swagger UI
- **Brauzer:** Chrome 126
- **Əməliyyat sistemi:** Windows 11
- **Build:** 1.0.8

---

# Test Case 1 – Positive

**Test ID:** TC-001

**Başlıq:** Düzgün məlumatlarla yeni avtomobilin uğurla yaradılmasının yoxlanılması

## İlkin şərtlər (Preconditions)

- Swagger UI əlçatandır.
- POST `/cars` endpoint-i işlək vəziyyətdədir.
- İstifadə ediləcək `id` sistemdə mövcud deyil.

## Test Məlumatları (Test Data)

```json
{
  "brand": "mercedes",
  "id": 55,
  "model": "model",
  "year": 1998
}
```

## Təkrar etmək üçün addımlar (Steps to Reproduce)

1. Swagger UI-ni aç.
2. POST `/cars` endpoint-ni seç.
3. Request body-ni daxil et.
4. **Execute** düyməsini kliklə.

## Gözlənilən nəticə (Expected Result)

- API **201 Created** status kodu qaytarmalıdır.
- Yeni avtomobil uğurla yaradılmalıdır.
- Response body göndərilən məlumatlarla uyğun olmalıdır.

## Faktiki nəticə (Actual Result)

- API **201 Created** status kodu qaytardı.
- Yeni avtomobil uğurla yaradıldı.
- Response body göndərilən məlumatlarla tam uyğun gəldi.

## Təkrarlanma dərəcəsi (Reproducibility)

**100% — 5/5 dəfə təkrar olunub.**

## Status

**Passed ✅**

---

# Test Case 2 – Negative

**Test ID:** TC-002

**Başlıq:** Təkrarlanan `id` ilə yeni avtomobil yaradılmasının yoxlanılması

## İlkin şərtlər (Preconditions)

- Swagger UI əlçatandır.
- `id = 55` olan avtomobil artıq sistemdə mövcuddur.

## Test Məlumatları (Test Data)

```json
{
  "brand": "mercedes",
  "id": 55,
  "model": "model",
  "year": 1998
}
```

## Təkrar etmək üçün addımlar (Steps to Reproduce)

1. Swagger UI-ni aç.
2. POST `/cars` endpoint-ni seç.
3. Yuxarıdakı request body-ni daxil et.
4. **Execute** düyməsini kliklə.

## Gözlənilən nəticə (Expected Result)

- API **409 Conflict** status kodu qaytarmalıdır.
- Avtomobil yaradılmamalıdır.
- `id` dəyərinin artıq mövcud olduğunu bildirən xəta mesajı göstərilməlidir.

## Faktiki nəticə (Actual Result)

- API **409 Conflict** status kodu qaytardı.
- Response body-də aşağıdakı mesaj göstərildi:

```text
Key (id)=(55) already exists.
```

- Yeni avtomobil yaradılmadı.

## Təkrarlanma dərəcəsi (Reproducibility)

**100% — 5/5 dəfə təkrar olunub.**

## Status

**Passed ✅**
