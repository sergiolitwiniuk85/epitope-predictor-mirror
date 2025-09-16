# epitope-predictor-mirror

# Epitope Predictor Mirror

<p align="center">
  <a href="https://huggingface.co/spaces/sergiolitwiniuk/epitope-predictor">
    <img src="https://img.shields.io/badge/Hugging%20Face%20Space-Deployed-blue?style=for-the-badge&logo=huggingface" alt="Hugging Face Space">
  </a>
  <a href="https://huggingface.co/sergiolitwiniuk/adapter-esm2-150M">
    <img src="https://img.shields.io/badge/Hugging%20Face%20Model-Adapter-orange?style=for-the-badge&logo=huggingface" alt="Hugging Face Model">
  </a>
</p>

---

## 🧐 Sobre este proyecto

Este repositorio sirve como un "mirror" (réplica) del proyecto **Epitope Predictor**, un modelo de lenguaje biológico ajustado para la predicción de epítopos. El modelo utiliza un adaptador de `Esm2-150M` para identificar las secuencias de aminoácidos que probablemente formen un epítopo, es decir, la parte de una molécula que es reconocida por el sistema inmunológico.

El objetivo de este repositorio es proporcionar una copia de seguridad y un acceso alternativo al modelo y los scripts asociados, asegurando que el proyecto sea accesible y fácil de replicar.

## 🚀 Recursos y enlaces

Todos los componentes principales del proyecto están disponibles en la plataforma de Hugging Face:

- **Hugging Face Space (Demo interactiva)**: Puedes interactuar con el modelo directamente a través de la interfaz web en el siguiente enlace:
  - [**sergiolitwiniuk/epitope-predictor**](https://huggingface.co/spaces/sergiolitwiniuk/epitope-predictor)

- **Modelo Adaptador (Adapter)**: El modelo fine-tuneado (`adapter-esm2-150M`) está alojado en el Hub de Hugging Face, desde donde puede ser descargado y utilizado en tus propios proyectos:
  - [**sergiolitwiniuk/adapter-esm2-150M**](https://huggingface.co/sergiolitwiniuk/adapter-esm2-150M)

## 💻 Uso local

Para utilizar el modelo localmente, clona este repositorio y asegúrate de tener las dependencias necesarias.

### 1. Clonar el repositorio

```bash
git clone [https://github.com/tu_usuario/epitope-predictor-mirror.git](https://github.com/tu_usuario/epitope-predictor-mirror.git)
cd epitope-predictor-mirror
