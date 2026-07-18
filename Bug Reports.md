# Bug Report

## Bug ID: BUG-001

**Başlıq:** Notifications səhifəsində Application silinərkən tətbiq silinmir və **"Not Found Applications"** bildirişi göstərilir

**Layihə:** Smplifai

**Modul:** Notifications – Applications

## Mühit (Environment)

- **Brauzer:** Chrome 126
- **Əməliyyat sistemi:** Windows 11
- **Build:** 1.0.8

## Severity

**Critical**

## Priority

**High**

## İlkin şərtlər (Preconditions)

- İstifadəçi sistemə uğurla daxil olub.
- Notifications səhifəsinə giriş imkanı var.
- Applications siyahısında ən azı bir tətbiq mövcuddur.

## Təkrar etmək üçün addımlar (Steps to Reproduce)

1. Smplifai sistemini aç.
2. Etibarlı istifadəçi məlumatları ilə daxil ol.
3. **Notifications** səhifəsinə keç.
4. Hər hansı bir **Application** üçün **Delete** düyməsini kliklə.

## Faktiki nəticə (Actual Result)

Seçilmiş Application silinmir və ekranda **"Not Found Applications"** pop-up bildirişi görünür.

## Gözlənilən nəticə (Expected Result)

Seçilmiş Application uğurla silinməli, siyahıdan yoxa çıxmalı və istifadəçiyə uğurlu silinmə haqqında məlumat göstərilməlidir. **"Not Found Applications"** bildirişi göstərilməməlidir.

## Əlavələr (Attachments)

- Screenshot
- Video qeydi
- Console logları

## Təkrarlanma dərəcəsi (Reproducibility)

**100% — 5/5 dəfə təkrar olunub.**

## Status

**Open**

---

## Bug ID: BUG-002

**Başlıq:** Notifications səhifəsində **Delete All** düyməsi ilə silinən bildirişlər səhifə yeniləndikdən sonra yenidən görünür

**Layihə:** Smplifai

**Modul:** Notifications

## Mühit (Environment)

- **Brauzer:** Chrome 126
- **Əməliyyat sistemi:** Windows 11
- **Build:** 1.0.8

## Severity

**Major**

## Priority

**High**

## İlkin şərtlər (Preconditions)

- İstifadəçi sistemə uğurla daxil olub.
- Notifications səhifəsində bir və ya bir neçə bildiriş mövcuddur.

## Təkrar etmək üçün addımlar (Steps to Reproduce)

1. Smplifai sistemini aç.
2. Etibarlı istifadəçi məlumatları ilə daxil ol.
3. **Notifications** səhifəsinə keç.
4. **Delete All** düyməsini kliklə.
5. Bildirişlərin siyahıdan silindiyini yoxla.
6. Səhifəni **Refresh (F5)** et.

## Faktiki nəticə (Actual Result)

**Delete All** düyməsi ilə silinən bildirişlər səhifə yeniləndikdən sonra yenidən görünür.

## Gözlənilən nəticə (Expected Result)

**Delete All** düyməsi klikləndikdən sonra bütün bildirişlər daimi olaraq silinməli və səhifə yeniləndikdən sonra da yenidən görünməməlidir.

## Əlavələr (Attachments)

- Screenshot
- Video qeydi
- Browser Console logları

## Təkrarlanma dərəcəsi (Reproducibility)

**100% — 5/5 dəfə təkrar olunub.**

## Status

**Open**
