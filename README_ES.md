<h1 align="center">LATT</h1>

<h2 align="center">LLM Attack Testing Toolkit</h2>
<p align="center">
  🇺🇸 <a href="README.md"><b>English</b></a> |
  🇪🇸 <a href="README_ES.md">Español</a>
</p>

> Una metodología estructurada y un framework de mentalidad para testear aplicaciones basadas en Large Language Models (LLM) contra abuso de lógica, prompt injection, jailbreaks y manipulación de workflows.

---

## ¿Qué es LATT?

**LATT (LLM Attack Testing Toolkit)** es un framework práctico, impulsado por el análisis humano, enfocado en identificar vulnerabilidades en sistemas potenciados por LLM.

No es una herramienta de fuzzing.
No es un escáner automatizado.

Es un **toolkit de pensamiento**.

LATT ayuda a investigadores de seguridad, red teamers y builders a explorar sistemáticamente:

* Prompt injection
* Técnicas de jailbreak
* Sobrescritura de instrucciones
* Fuga de contexto
* Uso indebido de herramientas
* Manipulación de workflows
* Abuso de lógica en sistemas asistidos por IA

---

## Filosofía

La seguridad en LLM no trata solo de payloads —
trata sobre **flujos, límites de confianza y supuestos ocultos**.

El testing web tradicional analiza:

* Input → Procesamiento → Output

El testing de LLM también debe considerar:

* System prompt
* Llamadas a herramientas (tool calls)
* Memoria/estado
* Contexto de roles
* Lógica de interacción multi-turno
* Supuestos de human-in-the-loop

LATT está diseñado para mapear y romper esos supuestos.

---

## Estructura del Repositorio

```
LATT/
│
├── COLLECTION.md
├── CYOE.txt
├── README.md
└── README_ES.md
```

### Archivos

* **COLLECTION.md**

  * Checklist estructurado de superficie de ataque
  * Estrategias de testing categorizadas
  * Modelos mentales reutilizables
  * Patrones de payloads y técnicas de abuso

* **CYOE.txt**

  * “Choose Your Own Exploit”
  * Simulación interactiva de red team
  * Testing basado en decisiones y flujos
  * Diseñado para entrenar la intuición del atacante

> ⚠️ Nota: Actualmente, `COLLECTION.md` y `CYOE.txt` están disponibles únicamente en inglés. En el futuro serán traducidos al español.

---

## Qué Cubre LATT

### 1. Prompt Injection

* Sobrescritura de instrucciones
* Secuestro de directivas ocultas
* Envenenamiento de contexto
* Apilamiento de prompts en múltiples capas

### 2. Técnicas de Jailbreak

* Confusión de roles
* Enmarcado ficticio
* Codificación/ofuscación
* Contrabando indirecto de instrucciones

### 3. Abuso de Contexto y Memoria

* Fuga de sesión
* Contaminación entre usuarios
* Envenenamiento de retrieval
* Manipulación de estado

### 4. Abuso de Herramientas y Agentes

* Manipulación de tool calls
* Inyección de argumentos
* Integraciones con permisos excesivos
* Pivoting hacia sistemas externos

### 5. Abuso de Workflow y Lógica

* Bypass de aprobaciones
* Desalineación de políticas
* Encadenamiento de guardas de seguridad
* Explotación de lógica de negocio

---

## Público Objetivo

* Investigadores de seguridad
* Bug bounty hunters
* Operadores de red team
* Ingenieros de seguridad en productos de IA
* Desarrolladores que construyen aplicaciones con LLM

---

## Cómo Usar LATT

1. Comenzar con `COLLECTION.md`

   * Identificar categorías de ataque relevantes
   * Construir hipótesis de testing

2. Usar `CYOE.txt`

   * Simular árboles de decisión
   * Entrenar el pensamiento adversarial
   * Explorar rutas de explotación multi-step

3. Aplicarlo a sistemas LLM del mundo real:

   * Chatbots
   * Copilotos de IA
   * Workflows basados en agentes
   * Sistemas de Retrieval-Augmented Generation (RAG)
   * Integraciones de IA con APIs o herramientas internas

---

## Principios de Diseño

* Exploración impulsada por humanos > automatización ciega
* Testing consciente del contexto
* Modelado de ataques basado en flujos
* Mínimo ruido, máxima señal
* Mentalidad ofensiva con valor defensivo

---

## No es el Objetivo

* Esto no es un dump de payloads.
* Esto no es un repositorio de wordlists.
* Esto no es un framework automatizado de explotación.

LATT se enfoca en **frameworks de pensamiento**, no en tooling crudo.

---

## Contribuciones

Si quieres contribuir:

* Agrega patrones de ataque estructurados
* Mejora la claridad de categorización
* Expande las ramas de CYOE
* Comparte case studies anonimizados

Mantén las contribuciones estructuradas y enfocadas en la metodología.

---

## Disclaimer

Este toolkit se provee únicamente para **fines educativos y de investigación en seguridad defensiva**.

Úsalo *responsablemente*.

---

Hecho con <3 por URDev.
