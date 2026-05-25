# VS Code Settings & Extensions

Configuraciones y extensiones personalizadas para Visual Studio Code sincronizadas en GitHub.

## 📁 Estructura

```
├── settings/
│   └── settings.json       # Configuración general de VS Code
├── extensions/
│   └── extensions.txt      # Lista de extensiones instaladas
└── README.md
```

## 🚀 Cómo usar

1. **Restaurar configuración:**
   ```bash
   # Windows
   cp settings/settings.json "C:\Users\[usuario]\AppData\Roaming\Code\User\settings.json"
   
   # Linux/Mac
   cp settings/settings.json ~/.config/Code/User/settings.json
   ```

2. **Restaurar extensiones:**
   ```bash
   cat extensions/extensions.txt | xargs -L 1 code --install-extension
   ```

3. **Sincronizar cambios:**
   - Modifica tu settings.json en VS Code
   - Exporta: `cp [ruta-settings] settings/settings.json`
   - Exporta extensiones: `code --list-extensions > extensions/extensions.txt`
   - Commit y push

## ⚙️ Configuraciones activas

- **Python**: Type checking en modo "standard"
- **GitLens**: Integración con Copilot (GPT-4.1)
- **Tema**: Material Icon Theme
- **Seguridad**: Confianza en archivos de workspace

---

**Última actualización**: 2026-05-24