# 🔧 n8n Workshop — Hybridge

> Repositorio del taller universitario de automatización con n8n. Contiene materiales teóricos, prácticas, ejercicios resueltos y flujos exportados para cada sesión.

[![n8n](https://img.shields.io/badge/n8n-Self--Hosted-orange)](https://n8n.io)
[![Node.js](https://img.shields.io/badge/Node.js-v22-green)](https://nodejs.org)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

---

## 📁 Estructura del repositorio

```
n8n-workshop/
├── README.md                          # Este archivo
├── LICENSE
├── .gitignore
│
├── sesion-01-introduccion/
│   ├── README.md                      # Resumen de la sesión
│   ├── docs/
│   │   ├── Hybridge_Sesion1_n8n.docx  # Material teórico completo
│   │   └── notas-clase.md             # Notas adicionales de clase
│   ├── workflows/
│   │   ├── hello-world-pokemon.json   # Workflow importable: Pokémon API
│   │   └── date-time-reto.json        # Reto flash: Date & Time
│   ├── practicas/
│   │   ├── AutoFlow_Lead_Qualification.docx   # Práctica: reglas de negocio
│   │   ├── AutoFlow_Pipeline_Infographic.html # Infográfico del flujo
│   │   └── lead-qualification-flow.json       # Workflow n8n (cuando lo implementes)
│   └── assets/
│       └── screenshots/               # Capturas de pantalla de la sesión
│
├── sesion-02-{nombre}/                # Misma estructura para cada sesión
│   ├── README.md
│   ├── docs/
│   ├── workflows/
│   ├── practicas/
│   └── assets/
│
├── recursos/
│   ├── glosario-bilingue.md           # Glosario acumulativo EN/ES
│   ├── cheatsheet-n8n.md              # Referencia rápida de nodos
│   └── security-checklist.md          # Checklist de seguridad para workflows
│
└── scripts/
    └── utils/                         # Scripts auxiliares si los necesitas
```

---

## 🚀 Quick Start

### Prerrequisitos

```bash
# Verificar Node.js
node -v   # Debe ser v18.17+, v20, o v22

# Si no tienes Node.js
nvm install 22
nvm use 22
```

### Instalación de n8n

```bash
npm install n8n -g
n8n start --tunnel
# Abrir: http://localhost:5678/
```

### Clonar este repositorio

```bash
git clone https://github.com/BENMP0902/n8n-workshop.git
cd n8n-workshop
```

---

## 📋 Sesiones

| # | Sesión | Estado | Temas clave |
|---|--------|--------|-------------|
| 01 | Introducción a n8n | ✅ Completa | Workflows, nodes, triggers, self-hosted, instalación |
| 02 | TBD | 🔜 Próxima | — |

---

## 🤝 Convenciones del repositorio

### Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(sesion-01): add lead qualification practice
docs(sesion-01): update session notes with class discussion
fix(sesion-01): correct webhook trigger configuration
chore: update .gitignore for n8n temp files
```

### Branches

- `main` — Material revisado y completo
- `sesion-XX-draft` — Trabajo en progreso de cada sesión

### Workflows exportados

Los archivos `.json` en `/workflows/` son exportaciones directas de n8n. Para importarlos:

1. Abrir n8n → New Workflow
2. Menú `⋮` → Import from File
3. Seleccionar el `.json`

---

## 🔒 Notas de seguridad

- **NUNCA** subas credenciales, API keys o tokens al repositorio
- Los archivos `.json` de n8n **pueden contener credenciales** — revisa antes de hacer commit
- Usa el `.gitignore` incluido que excluye archivos sensibles

---

## 📚 Recursos adicionales

- [Documentación oficial n8n](https://docs.n8n.io/)
- [n8n Community](https://community.n8n.io/)
- [n8n Node Reference](https://docs.n8n.io/integrations/)

---

*Parte del proyecto [Hybridge](https://github.com/BENMP0902) — Curriculum integral de ingeniería de software.*