# Transcriptor Multi-IA v17.0 — UAS / VOSH Integration

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![R](https://img.shields.io/badge/R-%3E%3D%204.0.0-blue.svg)](https://www.r-project.org/)
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)

[Español](#español) | [English](#english)

---

## Español

Sistema interactivo desarrollado en **R (Shiny)** por la **Universidad Autónoma de Sinaloa (UAS)** para la auditoría, digitalización y transcripción automatizada de formatos médicos universales utilizando Modelos de Lenguaje de Visión (VLM) a través de OpenRouter.

La arquitectura del script utiliza un sistema de **Buffer Secuencial indexado estilo C** para optimizar la gestión de memoria RAM, procesando los archivos PDF página por página sin comprometer los recursos del servidor en lotes masivos.

### 🚀 Características Clave
* **Módulo VOSH:** Extracción estructurada basada en un contrato estricto de variables mapeadas desde diccionarios analíticos de Excel.
* **Módulo DIF Sinaloa:** Normalización de datos clínicos (edades, géneros, graduaciones ópticas).
* **Auto-Healer JSON:** Algoritmos internos de minería de texto (*thought-mining*) capaces de rescatar estructuras JSON corruptas o truncadas desde los tokens de razonamiento de la IA.
* **Proceso Aislado:** Migración de dependencias críticas a Ghostscript via `system2()`, evitando fallos de segmentación nativos en arquitecturas ARM64/Poppler.

### 📄 Cómo Citar este Trabajo
Si utilizas este software o parte de su arquitectura para tu investigación, por favor cita nuestro artículo científico:
> *Terán, E. et al. (2026). Transcripción Automatizada y Auditoría de Hojas Clínicas Optométricas mediante Modelos de Lenguaje de Visión. Revista de Investigación UAS.*

### 🤝 Colaboración e Integración al Equipo
¡Este es un proyecto de **Ciencia Abierta**! Invitamos a desarrolladores, científicos de datos y profesionales de la salud visual a colaborar.
* Si encuentras un error o quieres proponer una mejora, abre un **Issue** o envía un **Pull Request**.
* Si deseas integrarte formalmente al equipo de investigación de la UAS para el desarrollo de nuevos módulos clínicos, por favor revisa las pautas en [CONTRIBUTING.md](CONTRIBUTING.md).

---

## English

Interactive **R (Shiny)** system developed by the **Universidad Autónoma de Sinaloa (UAS)** for the automated auditing, digitization, and transcription of universal medical forms using Vision Language Models (VLMs) via OpenRouter.

The script's architecture employs a **C-style indexed Sequential Buffer** to optimize RAM management, processing PDF files page by page without draining server resources during massive batch uploads.

### 🚀 Key Features
* **VOSH Module:** Structured extraction based on a strict variable contract mapped directly from analytical Excel dictionaries.
* **DIF Sinaloa Module:** Standardized clinical data normalization (age, gender, optical prescriptions).
* **JSON Auto-Healer:** Internal text-mining algorithms (*thought-mining*) capable of rescuing corrupted or truncated JSON objects directly from the AI's reasoning tokens.
* **Isolated Processing:** Decoupled critical dependencies to Ghostscript via `system2()`, eliminating native segmentation faults on ARM64/Poppler architectures.

### 📄 How to Cite
If you use this software or any part of its architecture in your research, please cite our paper:
> *Terán, E. et al. (2026). Automated Transcription and Auditing of Optometric Clinical Forms Using Vision Language Models. UAS Research Journal.*

### 🤝 Contributing & Joining the Team
This is an **Open Science** project! We welcome developers, data scientists, and eye-care professionals to collaborate.
* To report bugs or suggest enhancements, please open an **Issue** or submit a **Pull Request**.
* To formally join the UAS research team for future clinical module developments, please check the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).
