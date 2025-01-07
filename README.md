![](https://github.com/viajatech/SuperAgente/blob/main/image%20(76).png)
---

# Agente Autónomo by David Ruiz (@viajatech)

![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-Enabled-brightgreen)
![Gradio](https://img.shields.io/badge/Gradio-Integrated-orange)

---

## 📚 **Descripción**

Bienvenido a **Agente Autónomo**, la herramienta de inteligencia artificial de última generación diseñada para transformar la manera en que interactúas con tu entorno digital. Inspirado por los personajes de ciencia ficción de la novela de David Ruiz, este agente autónomo convierte ideas imaginativas en realidad tecnológica, integrando múltiples modelos de IA para ofrecer una experiencia sin precedentes en automatización y productividad.

---

## 🚀 **Características Principales**

### **🧠 Integración Multimodal con IA**

- **Compatibilidad Universal:** Conecta y comunica con una amplia gama de modelos de IA, incluyendo LM Studio (Llama 3.1/3.2/3.3), Mistral, Qwen, Deepseek V3 y próximamente Llama 4.(entre otros)
- Inteligencia Mejorada: Utiliza estrategias avanzadas de Test-Time Compute para que cualquier modelo de IA pueda "pensar" más y ofrecer respuestas más inteligentes y coherentes.
- **pestaña de Configuración**, encontrarás un **Radio** con: **Simple**: Emula un razonamiento interno (chain-of-thought) con la profundidad especificada.  **Best-of-N** y **Weighted Best-of-N**: Generan varias respuestas y eligen la mejor según un reward (dummy).  
- **Beam Search** y **DVTS**: Implementaciones simplificadas de búsquedas más elaboradas que optimizan la salida del modelo en el test-time.  

Estas estrategias **no requieren** entrenamiento adicional; se basan en llamar varias veces al mismo modelo, con la diferencia de cómo se escogen las respuestas y cuántas iteraciones se ejecutan.ia Mejorada:** Emplea estrategias avanzadas de Test-Time Compute para potenciar cualquier modelo de IA, haciendo que piensen y respondan de manera más inteligente.

- **Flexibilidad Total:** Cambia entre diferentes modelos de IA sin esfuerzo, adaptándose a tus necesidades y preferencias en tiempo real.

### **🖥️ Automatización de Aplicaciones de Escritorio**

- **Control Completo:** Abre y gestiona aplicaciones como Microsoft Word, Excel y Notepad con simples comandos de voz o texto.
- **Escritura Automática:** Dicta tus ideas y deja que **Agente Autónomo** las escriba directamente en tus documentos, con autoguardado para máxima seguridad y eficiencia.
- **Fórmulas en Excel:** Introduce fórmulas específicas en celdas de Excel con facilidad, optimizando tu flujo de trabajo.

### **🌐 Automatización de Navegadores Web**

- **Búsquedas Inteligentes:** Realiza búsquedas optimizadas en Google, YouTube, Vimeo, Maps y Spotify, eliminando frases innecesarias para obtener resultados precisos.
- **Secciones Específicas:** Navega directamente a secciones como Imágenes, Videos, Shopping, Noticias, Maps y Libros con comandos sencillos.
- **Compatibilidad con Chrome y Firefox:** Controla tus navegadores favoritos desde una única interfaz, asegurando una experiencia fluida y sin interrupciones.

### **🎤 Interacción con Servicios de Voz**

- **Reconocimiento de Voz (STT):** Transcribe tu voz a texto con precisión utilizando `speech_recognition`.
- **Texto a Voz (TTS):** Escucha respuestas generadas por IA mediante servicios de Azure Cognitive Services.
- **Interfaz Conversacional:** Interactúa con tu agente autónomo de manera natural y conversacional, mejorando la accesibilidad y facilidad de uso.

### **🖌️ Interfaz de Usuario de Vanguardia**

- **Interfaz Gráfica Intuitiva:** Diseñada con Tkinter para una navegación fácil y accesible, con múltiples pestañas para gestionar diferentes funcionalidades.
- **Interfaz Web con Gradio:** Accede a tu agente desde cualquier dispositivo mediante Gradio, con enlaces locales y compartidos para una conectividad sin límites.
- **Experiencia de Usuario Superior:** Diseñada para ser elegante y funcional, asegurando que cada interacción sea fluida y agradable.

### **📈 Gestión de Concurrencia y Rendimiento**

- **Threading Avanzado:** Maneja múltiples tareas simultáneamente para mantener la aplicación responsiva, incluso durante operaciones intensivas.
- **Optimización de Recursos:** Asegura un rendimiento eficiente, maximizando el uso de la memoria y la CPU para una experiencia sin retrasos.

### **🔒 Manejo de Errores y Seguridad**

- **Logging Detallado:** Facilita la depuración y el monitoreo del funcionamiento del agente mediante un sistema de registro robusto.
- **Manejo de Excepciones:** Aumenta la robustez y confiabilidad de la aplicación mediante un manejo cuidadoso de errores en diversas partes críticas del código.

---

## 🛠️ **Instalación Rápida**

### 📋 **Requisitos Previos**

- **Sistema Operativo:** Windows
- **Python:** Versión 3.8 o superior
- **Gradio** para la interfaz de usuario.  
- **SpeechRecognition** para convertir voz a texto.  
- **Azure Cognitive Services** para convertir texto en voz.  
- **OpenAI API** apuntando a [LM Studio](https://github.com/lmstudio-ai) (configurado como servidor local).  

### 📥 **Instalación de Dependencias**

Ejecuta los siguientes comandos en tu terminal para instalar las bibliotecas necesarias:

```bash
pip install gradio
pip install openai
pip install azure-cognitiveservices-speech
pip install speechrecognition
pip install TTS
pip install selenium
pip install webdriver-manager
pip install pyperclip
pip install psutil
pip install pywin32
python -m pywin32_postinstall
```

---

## 💡 **Cómo Usar Agente Autónomo** 💡

### 🏁 **Iniciar el Agente Autónomo**

1. **Ejecuta el Script Principal:**
   Inicia la interfaz gráfica y el agente chatbot ejecutando el script principal en tu entorno Python.

### 📜 **Instrucciones de Uso para el Agente Chatbot**

Interactúa con el agente utilizando comandos de texto para automatizar tareas específicas. A continuación, se presentan ejemplos de uso para maximizar tu productividad:

#### **Para Word/Excel/Notepad:**

- **Abrir Word y escribir una  historia:**
  ```plaintext
  abre word y escribe una breve historia sobre un capibara
  ```
- **Abrir Excel y escribir múltiples líneas:**
  ```plaintext
  abre excel y escribe
  manzana
  pera
  uva
  ```
- **Abrir Bloc de Notas y escribir un cuento:**
  ```plaintext
  abre bloc de notas y escribe un cuento
  ```
- **Aplicar una fórmula en Excel:**
  - Introduce “A1” y “=1+1” en la sección “Aplicar Fórmula” de la pestaña Excel.

#### **Para Buscar en Maps:**

- **Buscar en Google Maps usando Chrome:**
  ```plaintext
  abre chrome y busca en maps hoteles para perritos
  ```
  Esto buscará "hoteles+para+perritos" eliminando "en" sobrante.
  
- **Buscar en Google Maps usando Firefox:**
  ```plaintext
  abre firefox y busca en maps veterinarias
  ```
  Esto abrirá Google Maps con "veterinarias".

#### **Para Videos en YouTube/Vimeo:**

- **Buscar videos en YouTube usando Firefox:**
  ```plaintext
  abre firefox y busca videos en youtube de gatitos
  ```
  Esto eliminará "de" y buscará "gatitos".
  
- **Buscar videos en Vimeo usando Chrome:**
  ```plaintext
  abre chrome y busca videos en vimeo de tutoriales de python
  ```
  Esto eliminará "de" y buscará "tutoriales de python".

#### **Para Spotify:**

- **Abrir Spotify en Chrome:**
  ```plaintext
  abre spotify en chrome
  ```
  Esto abrirá [https://open.spotify.com](https://open.spotify.com).
  
- **Abrir Spotify en Firefox:**
  ```plaintext
  abre spotify en firefox
  ```

#### **Redes Sociales (Placeholder):**

- **Automatizar una publicación en una red social:**
  ```plaintext
  abre la red social x en firefox, mi usuario es pepito, contraseña 123, escribe "Hola" y publica.
  ```

### 🌐 **Configuración de Gradio para Acceso Externo** 🌐

Permite el acceso al agente chatbot desde cualquier dispositivo (como celulares) configurando el túnel de Gradio:

- **Acceso Local (equipo local):**
  ```python
  demo.launch(share=False)
  ```

- **Acceso Externo (equipos externos):**
  ```python
  demo.launch(share=True)
  ```
  Esto generará dos enlaces:
  1. **Local:** Acceso desde tu PC/Laptop.
  2. **Compartido:** Un enlace para compartir que estará disponible por 72 horas, permitiendo el acceso desde celulares y otros equipos.

#### 📝 **Resumen de Configuración de Gradio:**

- **Equipos locales:**
  ```python
  share=False
  ```

- **Equipos externos:**
  ```python
  share=True
  ```

---

## 🧑‍🤝‍🧑 **Contribuciones** 🧑‍🤝‍🧑

¡La comunidad es el corazón de este proyecto! Si deseas contribuir, sigue estos pasos:

1. **Fork** este repositorio.
2. **Crea una nueva rama** (`git checkout -b feature/nueva-funcionalidad`).
3. **Haz tus cambios** y asegúrate de que el código funcione correctamente.
4. **Confirma tus cambios** (`git commit -m 'Añadir nueva funcionalidad'`).
5. **Push** a la rama (`git push origin feature/nueva-funcionalidad`).
6. **Abre una Pull Request**.

---

## 💖 **Apoya el Proyecto** 💖

Tu apoyo es crucial para continuar desarrollando **Agente Autónomo** y mantenerlo como una herramienta de código abierto. Considera realizar una donación para ayudarnos a seguir innovando y mejorando.

[💳 **Donaciones al proyecto aquí**](https://github.com/sponsors/viajatech)

---

## 📜 **Licencia** 📜

Este proyecto está licenciado bajo la Licencia **Apache 2.0**. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

## 📫 **Contacto** 📫

Para más información o soporte, visita el repositorio en GitHub o contacta a [David Ruiz](https://github.com/viajatech).

---

🌐 **Descubre el Futuro de la Automatización con Agente Autónomo. ¡Únete a la Revolución de la Inteligencia Artificial Hoy!** 🌐

---

