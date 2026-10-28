# NusaCore Admin Panel Template

NusaCore adalah template admin panel statis berbasis HTML, CSS, dan JavaScript yang dirancang untuk kebutuhan dashboard internal, backoffice, panel operasional, dan prototipe aplikasi web dengan tampilan modern.

## Gambaran Umum

Project ini berisi kumpulan halaman siap pakai untuk kebutuhan admin panel, seperti:

- Dashboard overview
- Manajemen user dan role
- Produk, order, transaksi, billing
- Notifikasi dan audit log
- Settings dan profile
- UI components dan layout variants
- Auth pages, onboarding, error pages
- Dokumentasi komponen template

Template ini cocok untuk:

- Pembuatan prototype cepat
- Landing struktur admin sebelum integrasi backend
- Dasar pengembangan panel internal perusahaan
- Referensi UI dashboard modern

## Struktur Project

```text
.
├── advanced-forms.html
├── api-integrations.html
├── audit.html
├── auth.html
├── billing.html
├── components.html
├── dashboard.html
├── datatables.html
├── details.html
├── docs.html
├── error-pages.html
├── file-manager.html
├── index.html
├── layouts.html
├── login.html
├── modals.html
├── notifications.html
├── onboarding.html
├── orders.html
├── permission-preview.html
├── products.html
├── profile.html
├── reports.html
├── roles.html
├── settings.html
├── states.html
├── transactions.html
├── users.html
├── css/
│   └── style.css
├── js/
│   └── app.js
└── README.md
```

## Teknologi yang Digunakan

Template ini menggunakan:

- **HTML5** untuk struktur halaman
- **CSS3** untuk styling utama
- **JavaScript vanilla** untuk interaksi UI
- **Google Fonts (Inter)** untuk tipografi
- **Font Awesome** untuk ikon
- **Chart.js** untuk visualisasi chart pada halaman tertentu

Beberapa halaman dokumentasi juga menampilkan integrasi atau gaya untuk library tambahan seperti DataTables, Dropzone, dan Quill.

## Cara Penggunaan

### 1. Jalankan secara langsung

Karena ini adalah template statis, Anda bisa langsung membuka file HTML di browser.

Contoh:

- `index.html`
- `dashboard.html`
- `login.html`

Namun untuk pengalaman yang lebih stabil, disarankan menjalankan dengan local server.

### 2. Menjalankan dengan local server

#### Opsi Python

```bash
python3 -m http.server 8000
```

Lalu buka:

```text
http://localhost:8000
```

#### Opsi VS Code Live Server

Jika menggunakan VS Code:

1. Install extension **Live Server**
2. Klik kanan `index.html`
3. Pilih **Open with Live Server**

### 3. Halaman awal

Gunakan salah satu halaman berikut sebagai entry point:

- `index.html` — alias dashboard utama
- `dashboard.html` — halaman dashboard eksplisit
- `docs.html` — dokumentasi komponen template

## Cara Kustomisasi

### Ubah branding

Brand utama saat ini menggunakan nama **NusaCore**. Anda bisa mengubah:

- Judul halaman pada tag `<title>`
- Nama brand di sidebar
- Logo teks atau inisial ikon brand

### Ubah warna utama

Buka file berikut:

- `css/style.css`

Lalu ubah variabel CSS di bagian `:root`, misalnya:

```css
--primary:#2563eb;
--primary-hover:#1d4ed8;
--primary-light:#eff6ff;
```

### Ubah data dummy

Sebagian isi tabel, statistik, notifikasi, dan preview disimpan di:

- `js/app.js`

Contoh data yang bisa diubah:

- daftar users
- transaksi
- audit log
- permission
- command palette
- template error page
- template auth preview

### Tambah halaman baru

Untuk menambah halaman baru:

1. Duplikasi salah satu file HTML yang paling mirip
2. Ubah judul halaman
3. Sesuaikan menu sidebar/top navigation
4. Tambahkan section atau komponen yang dibutuhkan
5. Jika perlu interaksi baru, tambahkan fungsi di `js/app.js`

## Fitur Utama Template

- Layout sidebar modern
- Dukungan dark mode
- Layout top navigation dan collapsed sidebar
- Responsive untuk desktop dan mobile
- Command palette sederhana
- Modal dan toast notification
- Preview auth flow
- Error state dan loading state
- Komponen statistik, tabel, card, form, badge, tabs, dan lainnya

## Filosofi Template

### 1. Cepat dipakai

NusaCore dibuat agar developer dapat langsung memakai template tanpa setup build tools yang rumit. File dapat dibuka langsung, dipelajari cepat, lalu diintegrasikan bertahap.

### 2. Mudah dimodifikasi

Struktur project sengaja dibuat sederhana:

- HTML per halaman
- satu file CSS utama
- satu file JavaScript utama

Pendekatan ini memudahkan tim kecil, freelancer, atau developer yang ingin bergerak cepat tanpa terikat framework tertentu.

### 3. Fokus pada kebutuhan admin nyata

Komponen dan halaman di template ini tidak hanya dekoratif, tetapi diarahkan untuk kebutuhan umum panel admin, seperti:

- monitoring data
- pengelolaan user
- transaksi dan billing
- audit dan notifikasi
- onboarding dan error handling

### 4. UI modern, namun tetap familiar

Template ini mencoba menjaga keseimbangan antara:

- tampilan modern
- keterbacaan tinggi
- navigasi yang jelas
- interaksi yang familiar bagi user backoffice

Tujuannya bukan sekadar “cantik”, tetapi membantu user bekerja lebih cepat.

### 5. Agnostic terhadap backend

NusaCore tidak bergantung pada stack backend tertentu. Anda bisa menghubungkannya ke:

- Laravel
- CodeIgniter
- Node.js / Express
- Django
- Rails
- API internal perusahaan
- atau sistem backend lain

Dengan begitu, template ini bisa menjadi lapisan presentasi yang fleksibel.

## Rekomendasi Pengembangan Lanjutan

Jika ingin mengembangkan template ini menjadi produk yang lebih siap produksi, Anda bisa menambahkan:

- sistem templating/partials untuk sidebar dan topbar
- integrasi API nyata
- autentikasi dan otorisasi backend
- asset bundler
- komponen reusable
- form validation yang lebih lengkap
- state management bila diporting ke framework

## Catatan

- Data pada beberapa halaman masih berupa **dummy/mock data**
- Sebagian fitur adalah **UI simulation** untuk kebutuhan demo
- Template ini ideal sebagai **fondasi UI**, lalu disambungkan ke logic aplikasi Anda

## Saran Alur Pakai

1. Mulai dari `index.html` atau `dashboard.html`
2. Sesuaikan branding menjadi identitas organisasi Anda
3. Rapikan menu sesuai modul yang benar-benar dipakai
4. Ganti data mock dengan data backend
5. Pecah komponen umum jika project makin besar

Dibuat sebagai template admin panel modern yang ringan, fleksibel, dan mudah diadaptasi untuk banyak kebutuhan operasional digital.
