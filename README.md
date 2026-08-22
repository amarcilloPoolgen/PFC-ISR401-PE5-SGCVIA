# PFC-ISR401-PE5-SGCVIA

Práctica Experimental Unidad V (PE5) — Ingeniería de Requisitos (ISR-401), UTEQ, 2026-2027 PPA.
Integración, métricas y defensa del Proyecto Integrador: **Sistema de Gestión para Clínicas Veterinarias con Inteligencia Artificial (SGCV-IA)**.

**Repositorio:** [https://github.com/<usuario>/PFC-ISR401-PE5-SGCVIA](https://github.com/amarcilloPoolgen/PFC-ISR401-PE5-SGCVIA)

## Equipo

| Integrante | Criterio(s) a cargo |
|---|---|
| Amagua | C1 — Auditoría de calidad ERS |
| Marcillo (Jean) | C2 — Trazabilidad end-to-end |
| Vera | C3 — Requisitos de IA |
| Mesías | C4 — ERS/SRS final integrado + C7 — Fundamento teórico y referencias |
| Barrionuevo | C6 — Estructura del informe/conclusiones + C8 — Gestión y evidencia Git |

## Compilación del informe (`main.tex`)

**Compilador:** `pdflatex` (o `latexmk`), con al menos 2 pasadas para resolver referencias cruzadas e índice.

```bash
git clone https://github.com/<usuario>/PFC-ISR401-PE5-SGCVIA.git
cd PFC-ISR401-PE5-SGCVIA
pdflatex main.tex
pdflatex main.tex
```

O, si tienes `latexmk` instalado (recomendado, resuelve automáticamente el número de pasadas):

```bash
latexmk -pdf main.tex
```

**Archivo principal:** `main.tex` (en la raíz del repositorio).

**Dependencias (paquetes LaTeX):** distribución `texlive-full` o `MiKTeX` con soporte para `longtable`, `graphicx`, `hyperref`, `booktabs`. No se requieren paquetes fuera de una instalación estándar de TeX Live.

## Estructura del repositorio

```
PFC-ISR401-PE5-SGCVIA/
├── README.md
├── main.tex
├── portada.tex
├── capitulos/
│   ├── 01_introduccion.tex
│   ├── 02_metodologia_ir.tex
│   ├── 03_ers_srs_final.tex
│   ├── 04_modelos_uml.tex
│   ├── 05_validacion.tex
│   ├── 06_gestion_trazabilidad.tex      ← Marcillo (C2)
│   ├── 07_requisitos_ia.tex             ← Vera (C3)
│   ├── 08_metricas_calidad.tex          ← Amagua (C1)
│   ├── 09_retrospectiva.tex             ← Barrionuevo (C8)
│   └── 10_conclusiones.tex              ← Barrionuevo (C6)
├── anexos/
│   ├── anexoA_instrumento_auditoria.tex ← Amagua (C1)
│   ├── anexoB_preguntas_tribunal.tex
│   ├── anexoC_aporte_individual.tex
│   ├── anexoD_retrospectiva.tex         ← Barrionuevo (C8)
│   └── anexoE_referencias_ia.tex        ← Mesías (C7)
├── 03_Modelado/
│   └── Diagramas_UML/
│       ├── DIAGRAMA DE CLASES REFINADOS.pdf        (histórico)
│       └── DIAGRAMA DE CLASES REFINADOS v3.1.pdf   (vigente)
├── matriz/
│   └── matriz_trazabilidad_final.xlsx   ← Marcillo (C2)
├── referencias/
│   └── referencias.bib
└── presentacion/
    └── defensa_PE5_SGCVIA.pptx
```

## Entregables de esta práctica

1. ERS/SRS final versionado (`main.tex` → `main.pdf`)
2. Informe final en PDF (≥40 páginas de contenido)
3. Matriz de trazabilidad final (`matriz/matriz_trazabilidad_final.xlsx`)
4. Presentación de defensa (`presentacion/`)
5. Este repositorio, público, con este README

## Versión vigente

Ver historial de commits para el detalle de correcciones aplicadas en la auditoría de trazabilidad (criterio C2): modelo de dominio v3.1, catálogo de requisitos legales, matriz de trazabilidad final y sincronización backlog↔ERS (100%, verificado contra `Trello_Import_SGCV_IA.csv`).
