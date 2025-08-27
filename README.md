# LinkedIn-Job-Bot-
Bot avanzado de LinkedIn desarrollado en Node.js + Puppeteer. Automatiza la búsqueda de empleos y postulaciones con Easy Apply, aplicando filtros inteligentes, llenado de formularios, manejo de CAPTCHA y registros detallados. Pensado para profesionales y reclutadores que buscan eficiencia y escalabilidad.

# 🤖 LinkedIn Job Bot – Automatiza tus postulaciones con Node.js + Puppeteer

En un mercado laboral competitivo, la eficiencia marca la diferencia entre lograr una entrevista o quedarse en la lista de espera.  
Este bot avanzado automatiza la búsqueda y postulación en LinkedIn, pensado para **profesionales, reclutadores y desarrolladores** que desean optimizar su tiempo y aumentar sus oportunidades.

---

## 🚀 Capacidades clave

- 🔹 **Easy Apply**: aplica únicamente a empleos con postulación rápida.  
- 🔹 **Búsqueda inteligente**: filtra por ubicación, fecha de publicación, modalidad remota y palabras clave.  
- 🔹 **Llenado automático de formularios**: experiencia, expectativa salarial y preguntas frecuentes.  
- 🔹 **Manejo de CAPTCHA**: detección y pausa para verificación manual.  
- 🔹 **Evita duplicados**: omite ofertas ya aplicadas o que requieren aplicación externa.  
- 🔹 **Configuración centralizada**: todo se gestiona desde `config.json`.  
- 🔹 **Logging detallado**: registros de cada búsqueda y aplicación realizada.  
- 🔹 **Manejo de errores y selectores de respaldo**: más resiliencia ante cambios en la interfaz de LinkedIn.  

---

## 🛠️ Tecnologías utilizadas

- ⚡ **Node.js** → lógica principal del sistema.  
- 🌐 **Puppeteer** → automatización del navegador.  
- 🧩 **Patrón modular** → cada funcionalidad está separada por módulos (`login`, `searchJobs`, `apply`).  
- ⏳ **Timeouts configurables** → simulan comportamiento humano y evitan bloqueos.  
- 🔐 **Control de sesión** → persistencia de login y cookies.  

---

## 📂 Estructura del proyecto

```bash
linkedin-bot/
  ├─ src/
  │   ├─ modules/         # Scripts específicos (login, búsqueda, postulación)
  │   ├─ utils/           # Funciones de soporte (logs, delays, captcha)
  │   └─ index.js         # Entrada principal
  ├─ config.json          # Parámetros de configuración
  ├─ .env                 # Credenciales de LinkedIn
  ├─ package.json
  └─ README.md
