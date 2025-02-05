# Markdown İmporter 📝

Bu araç, markdown dosyalarınızı modüler bir şekilde yönetmenizi sağlar. Markdown dosyalarınızı parçalara ayırıp, ana dosyanızda import edebilirsiniz.

## 📥 Kurulum

```bash
pip install markdown-importer
```

## 🚀 Özellikler

- Markdown dosyalarını modüler hale getirme
- Çoklu dil desteği (Türkçe/İngilizce)
- Eksik dosya kontrolü ve bildirimi
- Esnek import sözdizimi
- Otomatik senkronizasyon

## 🛠️ Kullanım

### 1. Markdown Dosyasını Hazırlama
Kaynak markdown dosyanızda import etmek istediğiniz dosyaları belirtin:
```markdown
<!-- @import "docs/api/auth/readme.md" -->
```

### 2. Çalıştırma

```bash
# Varsayılan ayarlarla
markdown-importer

# Özel parametrelerle
markdown-importer -e README.editor.md -g README.github.md -l tr
```

### 3. Parametreler

| Parametre | Kısa | Uzun | Varsayılan | Açıklama |
|-----------|------|------|------------|-----------|
| Kaynak Dosya | -e | --editor-file | README.editor.md | İmport direktiflerini içeren kaynak dosya |
| Hedef Dosya | -g | --github-file | README.github.md | Oluşturulacak sonuç dosyası |
| Temel Dizin | -b | --base-dir | . | İmport edilecek dosyaların aranacağı dizin |
| Dil | -l | --language | tr | Kullanılacak dil (tr: Türkçe, en: İngilizce) |

## 🌍 Dil Desteği

- 🇹🇷 Türkçe (`-l tr`)
- 🇬🇧 İngilizce (`-l en`)

## ⚠️ Hata Yönetimi

- Eksik dosyalar `[Missing File]` olarak işaretlenir
- Her hata detaylı olarak raporlanır
- İşlem sonucu özeti sunulur

---

# Markdown Importer 📝

This tool allows you to manage your markdown files in a modular way. You can split your markdown files into pieces and import them into your main file.

## 📥 Installation

```bash
pip install markdown-importer
```

## 🚀 Features

- Modular markdown file management
- Multi-language support (Turkish/English)
- Missing file checks and notifications
- Flexible import syntax
- Automatic synchronization

## 🛠️ Usage

### 1. Prepare Markdown File
Specify the files you want to import in your source markdown file:
```markdown
<!-- @import "docs/api/auth/readme.md" -->
```

### 2. Running

```bash
# With default settings
markdown-importer

# With custom parameters
markdown-importer -e README.editor.md -g README.github.md -l en
```

### 3. Parameters

| Parameter | Short | Long | Default | Description |
|-----------|-------|------|---------|-------------|
| Source File | -e | --editor-file | README.editor.md | Source file containing import directives |
| Target File | -g | --github-file | README.github.md | Result file to be created |
| Base Directory | -b | --base-dir | . | Directory to search for imported files |
| Language | -l | --language | tr | Language to use (tr: Turkish, en: English) |

## 🌍 Language Support

- 🇹🇷 Turkish (`-l tr`)
- 🇬🇧 English (`-l en`)

## ⚠️ Error Handling

- Missing files are marked as `[Missing File]`
- Each error is reported in detail
- Summary of process result is provided
