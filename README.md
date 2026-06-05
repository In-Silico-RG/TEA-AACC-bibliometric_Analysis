# TEA + Altas Capacidades en Academia — Análisis Bibliométrico

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)

## Descripción

Repositorio de datos, código y documentación del análisis bibliométrico sobre la intersección entre el **Trastorno del Espectro Autista (TEA)** y las **Altas Capacidades Intelectuales (AACC)** en investigadores y académicos profesionales, con énfasis en los contextos latinoamericano y colombiano.

**Fuente de datos:** [Lens.org](https://lens.org) — exportaciones BibTeX y CSV, junio 2026  
**Período analizado:** 1834–2026  
**Corpus maestro:** 3.966 registros únicos (BibTeX) / 1.869 registros con datos extendidos (CSV)

## Estructura del repositorio

```
tea-aacc-bibliometria/
├── data/
│   ├── raw/                    # Archivos originales de Lens.org
│   │   ├── string-1.csv        # S1 — Amplio
│   │   ├── string-2.csv        # S2 — Adultos profesionales
│   │   ├── string-3.csv        # S3 — Diagnóstico tardío
│   │   ├── string-4.csv        # S4 — Neurodiversidad laboral
│   │   ├── string-5.csv        # S5 — Español/Latinoamérica
│   │   ├── string-1-amplio.bib
│   │   ├── string-2-foco-adultos-profesionales.bib
│   │   ├── string-3-foco-diagnostico-tardio-enmascaramiento.bib
│   │   ├── string-4-neurodiversidad-entornos-academicos-laborales.bib
│   │   └── string-5-espanol-literatura-latinoamericana.bib
│   └── processed/
│       ├── corpus_maestro_enriched.csv      # Corpus deduplicado con citas
│       └── subcorpus_TEA_AACC_relevante.csv # Sub-corpus TEA+AACC filtrado
├── notebooks/
│   └── bibliometria_TEA_AACC_v2.ipynb      # Análisis completo reproducible
├── paper/
│   ├── paper_TEA_AACC_bibliometrico.tex     # Artículo principal (LaTeX)
│   ├── seccion_critica_metodologias_unisucre.tex
│   └── referencias.bib
├── figures/                                 # Todas las figuras generadas
├── protocol/
│   └── protocolo_autoexploracion_TEA.md    # Protocolo de autoexploración
└── docs/
    └── search_strings.md                   # Strings de búsqueda documentados
```

## Reproducibilidad

### Requisitos

```bash
pip install pandas matplotlib seaborn wordcloud networkx bibtexparser
# O con conda:
conda install pandas matplotlib seaborn networkx
pip install wordcloud bibtexparser
```

### Ejecución

```bash
git clone https://github.com/nsiico/tea-aacc-bibliometria.git
cd tea-aacc-bibliometria
jupyter notebook notebooks/bibliometria_TEA_AACC_v2.ipynb
```

Los archivos CSV y BibTeX deben estar en `data/raw/`. Actualizar las rutas en la celda §2 si es necesario.

## Resultados principales

| Indicador | Valor |
|-----------|-------|
| Corpus maestro (BibTeX dedup) | 3.966 registros |
| Corpus maestro (CSV extendido) | 1.869 registros |
| Sub-corpus TEA+AACC relevante | 341 registros |
| Total citas (corpus extendido) | 33.596 |
| h-index corpus completo | 85 |
| h-index sub-corpus TEA+AACC | 32 |
| % Open Access | 88,4% |
| Registros con mención a Colombia | 8 |
| CAGR 2010–2020 | +16,4%/año |

## Cita

Si usas este repositorio, por favor cita:

```bibtex
@misc{nsiico2026,
  author  = {[Autores]},
  title   = {Análisis Bibliométrico sobre TEA y Altas Capacidades en Academia},
  year    = {2026},
  doi     = {10.5281/zenodo.XXXXXXX},
  url     = {https://github.com/nsiico/tea-aacc-bibliometria}
}
```

## Licencia

Los datos derivados y el código están bajo licencia [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).  
Los datos originales de Lens.org están sujetos a sus propios términos de uso.

## Contacto

**Repositorio mantenido por:** @In-Silico-RG
**Afiliación:** Universidad de Sucre (Unisucre), Colombia
