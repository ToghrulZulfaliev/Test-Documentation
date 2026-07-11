# Test Plan – Smplifai Tələbə Qeydiyyatı və Sənəd Avtomatlaşdırılması Platforması

## 1. Objective

Bu test planın məqsədi **Smplifai** platformasının funksional tələblərə, biznes qaydalarına və təhlükəsizlik tələblərinə uyğun işlədiyini yoxlamaqdır.

---

## 2. Scope

### In Scope

- Tələbə qeydiyyatı
- Email və şifrə ilə giriş
- Google OAuth ilə giriş
- Documentlərin upload olunması
- Şəxsi məlumatların idarə olunması
- Yeni tələbə profilinin yaradılması
- Faylların silinməsi
- Məlumatların saxlanılması
- Məcburi sənədlərin yoxlanılması
- Email və sistem bildirişləri
- Profil məlumatlarının avtomatik doldurulması
- Təkrarlanan Student ID yoxlanılması
- Validasiya mesajları
- Xəta mesajları
- API testləri
- Təhlükəsizlik testləri
- Bildirişlərin yoxlanılması

### Out of Scope

- Admin Panel
- Server infrastrukturu və performans testləri
- Billing System

---

## 3. Test Types

| Test Type | Description |
|------------|-------------|
| Functional Testing | Biznes tələblərinin düzgün işləməsinin yoxlanılması |
| UI Testing | Dizayn, düymələr, formalar və mesajların yoxlanılması |
| Negative Testing | Yanlış məlumatlarla sistemin davranışı |
| Regression Testing | Yeni dəyişikliklərdən sonra mövcud funksiyaların yoxlanılması |
| Cross-browser Testing | Chrome, Firefox və Edge brauzerlərində yoxlama |
| API Testing | Backend API-lərin yoxlanılması |
| Smoke Testing | Yeni build-in əsas funksiyalarının işləməsinin yoxlanılması |

---

## 4. Test Environment

| Item | Details |
|------|---------|
| OS | Windows 11 |
| Browsers | Chrome, Firefox, Edge |
| Backend | QA Mühiti |
| Database | QA Database |

---

## 5. Entry Criteria

Testing can start when:

- Biznes tələbləri təsdiqlənib.
- QA mühiti hazırdır.
- Son build deploy olunub.
- API-lər işlək vəziyyətdədir.
- Test istifadəçiləri yaradılıb.
- Test sənədləri hazırlanıb.
- AI servisi işləyir.
- Smoke Test uğurla keçib.

---

## 6. Exit Criteria

Testing can finish when:

- Planlaşdırılmış bütün test case-lər icra olunub.
- Critical və High prioritetli açıq bug qalmayıb.
- Uğursuz testlər yenidən yoxlanılıb.
- Regression Test tamamlanıb.
- Test hesabatı hazırlanıb.
- Product Owner buraxılışı təsdiqləyib.

---

## 7. Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| Applications are not displayed | Tələbə müraciətləri görünmür və test ssenarilərinin icrası bloklanır. | Testdən əvvəl tətbiqlərin yaradıldığını, API və Database məlumatlarının düzgün yükləndiyini yoxlamaq, problem olduqda development komandası ilə əlaqə saxlamaq. |
| Billing (ödəniş) prosesinin düzgün işləməməsi | Ödəniş ssenarilərinin test edilməsi mümkün olmaya bilər və istifadəçilər ödənişlərini uğurla tamamlaya bilməzlər. | Testə başlamazdan əvvəl Billing xidmətinin işlək vəziyyətdə olduğunu yoxlamaq, test/mock ödəniş mühitindən istifadə etmək və problem aşkar edildikdə development komandasını məlumatlandırmaq. |

---

## 8. Deliverables

- Test Plan
- Test Ssenariləri
- Test Case-lər
- Test Məlumatları
- API Test Collection
- Bug Report
- Test Execution Report
- Regression Report
- Test Summary Report
