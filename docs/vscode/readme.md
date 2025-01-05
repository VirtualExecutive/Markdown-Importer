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
