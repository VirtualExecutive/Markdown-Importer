# API Çalışma Prensibi 📚

Bu dokümantasyon, API'nin nasıl çalıştığını ve temel yapısını açıklar.

## 🔄 API Çalışma Hiyerarşisi

### 📥 API Akışı

```
┌─────────────────────────┐
│ 1. İstek API Endpoint'e │
└──────────┬──────────────┘
           ↓
┌─────────────────────────┐
│ 2. Güvenlik Kontrolleri │
└──────────┬──────────────┘
           ↓
┌─────────────────────────┐
│ 3. İstek Kabulü         │
└──────────┬──────────────┘
           ↓
┌─────────────────────────┐
│ 4. Veri Alanları        │
│    Kontrolü             │
└──────────┬──────────────┘
           ↓
┌─────────────────────────┐     ┌───────────────────────┐
│ 5. Servis Katmanı       │ ←→  │ Repository & Services │
└──────────┬──────────────┘     └───────────────────────┘
           ↓
┌─────────────────────────┐
│ 6. İstemciye Yanıt      │
│    Döndürme             │
└─────────────────────────┘
```

[ @import "docs/api/auth/readme.md" başlangıcı]
<!-- @import "docs/api/auth/readme.md" -->
[ @import "docs/api/auth/readme.md" bitişi]

