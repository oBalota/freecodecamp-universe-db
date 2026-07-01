# 🌌 Celestial Bodies Database (Universe)

[English](#english) | [Türkçe](#türkçe)

---

## English

### 📝 Project Overview
This project was developed as part of the **freeCodeCamp - Relational Database Certification**. The goal was to design and populate a relational database named `universe` using PostgreSQL, ensuring that it meets strict database normalization rules, foreign key constraints, and specific data requirements.

### 🚀 Features & Technical Requirements
*   **Database Engine:** PostgreSQL
*   **Total Tables:** 5 (`galaxy`, `star`, `planet`, `moon`, and `space_mission`)
*   **Key Constraints:**
    *   Every table uses an automatically incrementing Primary Key (`SERIAL`) following the `table_name_id` convention.
    *   Strict Foreign Key references mapping the hierarchy: `galaxy` ➔ `star` ➔ `planet` ➔ `moon`.
    *   Enforced data integrity with `NOT NULL` and `UNIQUE` constraints where required.
*   **Data Types Used:** `VARCHAR`, `INT`, `NUMERIC`, `TEXT`, and `BOOLEAN`.
*   **Data Scale:** Contains over 40+ carefully structured rows including 6 galaxies, 6 stars, 12 planets, and 20 moons.

### 🛠️ How to Use
To restore this database locally, run the following commands in your PostgreSQL terminal:

`CREATE DATABASE universe;`

## Türkçe
### 📝 Proje Özeti
Bu proje, freeCodeCamp - Relational Database Certification (İlişkisel Veritabanı Sertifikası) kapsamında geliştirilmiştir. Amaç, PostgreSQL kullanarak universe adında ilişkisel bir veritabanı tasarlamak, tablolar arası ilişkileri (Foreign Keys) kurmak ve veritabanı normalizasyon kurallarına uygun bir yapı inşa etmekti.

### 🚀 Özellikler ve Teknik Gereksinimler
**Veritabanı Yönetim Sistemi:** PostgreSQL

**Toplam Tablo Sayısı:** 5 adet (`galaxy`, `star`, `planet`, `moon` ve `space_mission`)

**Kısıtlamalar & Kurallar:**

* Her tablo, `table_name_id` kuralına uygun, otomatik artan (`SERIAL`) bir Birincil Anahtara (Primary Key) sahiptir.

* Hiyerarşik düzen Foreign Key'ler ile korunmuştur: `galaxy` ➔ `star` ➔ `planet` ➔ `moon`.

* `NOT NULL` ve `UNIQUE` kısıtlamaları ile veri tutarlılığı sağlanmıştır.

**Kullanılan Veri Tipleri:** `VARCHAR`, `INT`, `NUMERIC`, `TEXT` ve `BOOLEAN`.

**Veri Hacmi:** 6 galaksi, 6 yıldız, 12 gezegen ve 20 ay olmak üzere toplamda 40'tan fazla satır veri işlenmiştir.

### 🛠️ Nasıl Çalıştırılır?
Bu veritabanını kendi yerel ortamınızda ayağa kaldırmak için PostgreSQL terminalinde şu komutu çalıştırın:

` CREATE DATABASE universe;`

Ardından yedek dosyasını içeri aktarın:

` psql -U postgres -d universe < universe.sql `

