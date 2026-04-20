# 🎓 Examen Complexivo MBA — Simulador Interactivo

Simulador de evaluación para el Examen Complexivo de la Maestría en Administración de Empresas (MBA).

## ✨ Características

- 🎲 **40 preguntas aleatorias** seleccionadas del banco completo de 517 preguntas
- 📚 **3 opciones por pregunta** (1 correcta + 2 distractores generados automáticamente)
- ✅ **Retroalimentación inmediata** con explicación de la respuesta correcta
- 📊 **Calificación al 100%** con desglose por módulo
- 🏅 **Informe de desempeño** — identifica tus fortalezas y áreas de mejora
- 📱 **Diseño responsive** optimizado para móvil, tablet y escritorio

## 📦 Módulos incluidos

| # | Módulo | Preguntas |
|---|--------|-----------|
| 1 | Dirección y Organización de la Empresa | 60 |
| 2 | Dirección Estratégica de la Empresa | 58 |
| 3 | Dirección de Marketing y Gestión Comercial | 59 |
| 4 | Dirección de Recursos Humanos | 40 |
| 5 | Marketing Digital | 57 |
| 6 | Dirección Financiera | 34 |
| 7 | Logística de Cadena de Suministro | 59 |
| 8 | Creación de Empresas | 55 |
| 9 | Habilidades Directivas | 47 |
| 10 | Trabajo de Titulación | 48 |
| **Total** | | **517** |

## 🚀 Despliegue en GitHub Pages

### Opción A — Desde la interfaz web de GitHub

1. Crea un nuevo repositorio en GitHub (ej: `quiz-mba`)
2. Sube los dos archivos: `index.html` y `questions.json`
3. Ve a **Settings → Pages**
4. En "Source" selecciona **Deploy from a branch**
5. Selecciona la rama `main` y carpeta `/root`
6. Haz clic en **Save**
7. En 1-2 minutos tu sitio estará en: `https://[tu-usuario].github.io/quiz-mba`

### Opción B — Con Git por terminal

```bash
git init
git add .
git commit -m "Quiz MBA inicial"
git branch -M main
git remote add origin https://github.com/[tu-usuario]/quiz-mba.git
git push -u origin main
```
Luego activa GitHub Pages desde Settings.

### Opción C — Prueba local

```bash
python3 -m http.server 8080
# Abre: http://localhost:8080
```
> ⚠️ No abras el `index.html` directamente como archivo — necesitas un servidor web para que `fetch('questions.json')` funcione.

## 🗂️ Estructura del proyecto

```
quiz-mba/
├── index.html        ← Aplicación completa (HTML + CSS + JS)
├── questions.json    ← Banco de 517 preguntas (generado automáticamente)
└── README.md         ← Este archivo
```

## 📋 Importar preguntas a Google Sheets

El archivo `PREGUNTAS_COMPLEXIVO.csv` (entregado por separado) contiene todas las preguntas con formato:
`ID | MÓDULO | PREGUNTA | RESPUESTA`

Para importarlo:
1. Abre el Google Sheets indicado
2. Ve a **Archivo → Importar**
3. Sube el CSV y selecciona "Reemplazar hoja actual"

---
*Generado automáticamente a partir del banco oficial de preguntas del MBA.*
