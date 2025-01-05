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
