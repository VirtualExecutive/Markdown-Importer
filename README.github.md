
[ @import "docs/api/readme.md" başlangıcı İÇ İÇE İMPORT]
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
# 🔐 Kimlik Doğrulama API'si

Bu dokümantasyon, kimlik doğrulama (authentication) API endpoint'lerini açıklar.

## 📝 Genel Bakış

Kimlik doğrulama API'si aşağıdaki temel işlevleri sağlar:

- Kullanıcı kaydı (Register)
- Giriş yapma (Login) 
- Şifre sıfırlama (Password Reset)
- Token yenileme (Token Refresh)

## 🔑 Endpoint'ler

### 1. Kullanıcı Kaydı

**Endpoint:** `POST /api/auth/register`

**İstek Gövdesi:**

[ @import "docs/api/auth/readme.md" bitişi]


[ @import "docs/api/readme.md" bitişi]

[ @import "docs/vscode/readme.md" başlangıcı TEK İMPORT]
# 🐛 VSCode Debug Yapılandırması

## 📋 Genel Bakış
VSCode üzerinden Python uygulamasını debug etmek için gerekli yapılandırma ayarları.

## 📝 Dosya Konumu
`.vscode/launch.json`

## ⚙️ Yapılandırma Parametreleri

| Parametre | Değer | Açıklama |
|-----------|-------|-----------|
| name | "Python Debug: run.py" | Debug yapılandırmasının adı |
| type | "debugpy" | Debug için kullanılacak araç |
| request | "launch" | Debug başlatma modu |
| program | "run.py" | Çalıştırılacak Python dosyası |
| console | "integratedTerminal" | Konsol tipi |

## 📝 Örnek Yapılandırma
```json
{
    "configurations": [
        {
            "name": "Python Debug: run.py",
            "type": "debugpy",
            "request": "launch",
            "program": "run.py",
            "console": "integratedTerminal"
        }
    ]
}
```

## 🛠️ Kullanım
1. F5'e basarak debug moduna geçebilirsiniz.
2. Sadece `name` değiştirilebilirsiniz.

## 💡 Önemli Özellik
- Bu yapılandırma sayesinde, çalışma alanındaki hangi `.py` dosyasında olursanız olun, F5'e bastığınızda otomatik olarak `run.py` çalıştırılır. Bu özellik, farklı dosyalarda çalışırken bile ana uygulamayı hızlıca debug etmenizi sağlar.

## ⚠️ Gereksinimler
1. Python eklentisi yüklü olmalı
2. debugpy paketi yüklü olmalı (`pip install debugpy`)
3. Workspace klasöründe `.vscode` dizini olmalı

[ @import "docs/vscode/readme.md" bitişi]


[Dosya yok]
<!-- @import "docs/no/readme.md" [Missing File] -->

[Boşluk var / True]
<!--@import "dosya.md"-->
<!-- @import "dosya.md" [Missing File] -->
<!-- @import "dosya.md" [Missing File] -->
<!-- @import "dosya.md" [Missing File] -->

