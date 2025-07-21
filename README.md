
# 📚 Chatbot Legal RAG sobre el Reglamento de Solicitud de Refugio en Guatemala

Este proyecto implementa un sistema de **Recuperación Aumentada por Generación (RAG)** aplicado al texto completo del *Reglamento para la Determinación de la Condición de Refugiado en Guatemala*. Su objetivo es responder de manera precisa y explicativa a preguntas sobre el proceso de solicitud de refugio, utilizando inteligencia artificial generativa multilingüe.

---

## 🧠 ¿Qué hace este proyecto?

- ✅ Procesa el reglamento legal en formato `.txt`, segmentándolo en fragmentos semánticos.
- ✅ Genera **embeddings** de los artículos con modelos de `sentence-transformers`.
- ✅ Indexa el contenido usando **FAISS** para búsquedas rápidas.
- ✅ Integra dos opciones de respuesta:
  - **Extractiva** con `XLM-RoBERTa` fine-tuned en SQuAD2.
  - **Generativa** con `Mistral-7B-Instruct`, capaz de redactar respuestas legales naturales.
- ✅ Responde a preguntas sobre plazos, derechos, instituciones responsables y procedimientos clave.

---

## ⚙️ Tecnologías utilizadas

- 🧩 [LangChain](https://www.langchain.com/)
- 🤗 [Transformers](https://huggingface.co/docs/transformers/index)
- 🔍 [FAISS](https://github.com/facebookresearch/faiss)
- 🧠 [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1)
- 🧠 `sentence-transformers/all-MiniLM-L6-v2`
- 🐍 Python 3.10+

---

## 🚀 Cómo ejecutarlo

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/chatbot-rag-refugio-guatemala.git
   cd chatbot-rag-refugio-guatemala
   ```

2. Crea un entorno virtual e instala dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Ejecuta el notebook `RAG.ipynb` en Jupyter.

4. Opcional: agrega tu token de Hugging Face como variable de entorno:
   ```bash
   export HF_TOKEN=tu_token
   ```

---

## 📝 Ejemplos de preguntas respondidas

| Pregunta | Respuesta generada |
|---------|--------------------|
| ¿Cuántos días puede tardar la resolución de una solicitud? | Hasta 30 días según CONARE, aunque puede extenderse. |
| ¿Qué documento se presenta para extender el estatus de refugiado? | El Documento Personal de Identidad Especial. |
| ¿Ante qué autoridad se puede solicitar asilo? | Ante la Subdirección de Protección del Instituto Guatemalteco de Migración o en puestos fronterizos. |

---

## 📎 Archivos incluidos

- `RAG.ipynb`: Notebook principal con implementación paso a paso.
- `reglamento_solicitud_refugio_Guatemala.txt`: Texto base legal procesado.
- `Piloto Chatbot con IA.docx`: Idea conceptual y justificación del piloto.

---

## 💡 Posibilidades de ampliación

- Agregar otros cuerpos normativos (Ley de Migración, Constitución).
- Implementar una interfaz web con Gradio o Streamlit.
- Evaluar precisión con un conjunto de preguntas de prueba.
- Integrar validación legal por expertos.

---

## 👤 Autor

**José Marcelo Jara Vera**  
Especialista en análisis de datos y sistemas de protección internacional  
Guatemala / Ecuador  
[LinkedIn](https://www.linkedin.com/in/marcelojara25/) · marcelojara25@yahoo.com
