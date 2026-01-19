# Auth Supabase App

Aplikasi Flutter dengan autentikasi lengkap menggunakan Supabase (Sign Up, Login, dan Logout).

## Fitur

- ✅ Sign Up (Registrasi)
- ✅ Login (Masuk)
- ✅ Logout (Keluar)
- ✅ Validasi form
- ✅ UI yang modern dan responsif
- ✅ State management untuk autentikasi

## Setup

### 1. Install Dependencies

```bash
flutter pub get
```

### 2. Setup Supabase

1. Buat akun di [Supabase](https://supabase.com)
2. Buat project baru
3. Dapatkan URL dan anon key dari dashboard project Anda
4. Buka file `lib/config/supabase_config.dart` dan isi dengan kredensial Anda:

```dart
class SupabaseConfig {
  static const String supabaseUrl = 'https://your-project.supabase.co';
  static const String supabaseAnonKey = 'your-anon-key-here';
}
```

### 3. Jalankan Aplikasi

```bash
flutter run
```

## Struktur Project

```
lib/
├── config/
│   └── supabase_config.dart    # Konfigurasi Supabase
├── screens/
│   ├── login_screen.dart        # Halaman Login
│   ├── signup_screen.dart       # Halaman Sign Up
│   └── home_screen.dart         # Halaman Home dengan Logout
├── services/
│   └── auth_service.dart        # Service untuk autentikasi
└── main.dart                     # Entry point aplikasi
```

## Dependencies

- `supabase_flutter`: SDK Supabase untuk Flutter
- `flutter_secure_storage`: Untuk penyimpanan data aman (opsional)

## Catatan

Pastikan Anda sudah mengaktifkan Email Authentication di dashboard Supabase (Settings > Authentication > Providers > Email).
