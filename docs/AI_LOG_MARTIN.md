# Log de prompts a las IAs

**Obligatorio registrar cada prompt siguiendo este formato, empezando desde el más reciente hasta el más antiguo. Se puede pedir a la misma IA que entregue el log.**

* Nombre de integrante - Prompt # (# de prompt)
* IA utilizada
* Prompt del integrante completo
* Respuesta de la IA completa
* Qué se aceptó
* Qué se denegó
* Qué se modificó

---

Martin Contreras - Prompt #1

### IA utilizada: Claude

**Prompt del integrante completo:**
> Te voy a dar acceso a una carpeta que contiene 4 proyectos en total. Detalle de los proyectos: 
>3 proyectos de SensorHub: Son implementaciones de una API (una versión es mía y las otras dos son de mis compañeros de equipo).
>1 proyecto llamado EDSIA-BEYOND: Este es un proyecto nuevo que vamos a desarrollar en conjunto. Para este caso en particular, aún no tenemos las métricas definidas, pero nuestro objetivo actual es empezar a estructurar las partes del sistema que queremos automatizar.
>Instrucción estricta: Por ahora, tu única tarea es leer, analizar y comprender la arquitectura y relación entre estos repositorios. No quiero que realices, propongas ni apliques ningún cambio al código ni a la estructura.
>Solo confirma que has procesado el contexto de los 4 proyectos y dime que estás listo para mis siguientes instrucciones.

**Respuesta de la IA completa:**

```bash
Ya tengo el contexto de los 4 proyectos. Resumen consolidado:

Los 3 SensorHub (mismo dominio, implementaciones independientes)

Los tres son APIs REST en Python + FastAPI + SQLAlchemy 2.x + Alembic, con PostgreSQL en producción y SQLite en local/tests, dockerizadas y desplegadas en Render. Comparten el mismo dominio: Sensor → Reading → Alert (sensores que emiten lecturas, que disparan alertas por umbral con máquina de estados open → acknowledged → resolved), y arquitectura en capas (routers/services/repositories/models) documentada con ADRs. Todo apunta a que nace del mismo curso (SDLC/electrónica) resuelto por cada integrante por separado.

EDSIA-BEYOND

Repositorio en puro scaffolding: casi todo vacío (pyproject.toml, requirements.txt sin contenido), sin código ni arquitectura definida aún. Es Python por convención (.gitignore), sin framework elegido. Lo único con sustancia es CONTRIBUTING.md (en la rama dev remota): flujo main protegido + dev de integración, 2 revisores obligatorios, cobertura mínima 90%, y regla de que todo el código vive en src/. El AI_LOG.md de esa misma rama confirma que la intención explícita del equipo es analizar los 3 SensorHub existentes para repartir roles de cara a EDSIA-BEYOND — es decir, este nuevo proyecto probablemente reutilizará patrones/aprendizajes de esas tres implementaciones (posiblemente una consolidación o evolución del mismo dominio de sensores, aunque eso aún no está definido).

He procesado y entendido la arquitectura y relación entre los 4 proyectos. No realicé ni propuse ningún cambio. Listo para tus siguientes instrucciones.

```
**Qué se aceptó:** N/A

**Qué se denegó:** N/A

**Qué se modificó:** N/A

---

Martin Contreras - Prompt #2

### IA utilizada: Claude

**Prompt del integrante completo:**
> Te voy a dar acceso a una carpeta que contiene 4 proyectos en total. Detalle de los proyectos: 
>3 proyectos de SensorHub: Son implementaciones de una API (una versión es mía y las otras dos son de mis compañeros de equipo).
>1 proyecto llamado EDSIA-BEYOND: Este es un proyecto nuevo que vamos a desarrollar en conjunto. Para este caso en particular, aún no tenemos las métricas definidas, pero nuestro objetivo actual es empezar a estructurar las partes del sistema que queremos automatizar.
>Instrucción estricta: Por ahora, tu única tarea es leer, analizar y comprender la arquitectura y relación entre estos repositorios. No quiero que realices, propongas ni apliques ningún cambio al código ni a la estructura.
>Solo confirma que has procesado el contexto de los 4 proyectos y dime que estás listo para mis siguientes instrucciones.

**Respuesta de la IA completa:**

```bash
Ya tengo el contexto de los 4 proyectos. Resumen consolidado:

Los 3 SensorHub (mismo dominio, implementaciones independientes)

Los tres son APIs REST en Python + FastAPI + SQLAlchemy 2.x + Alembic, con PostgreSQL en producción y SQLite en local/tests, dockerizadas y desplegadas en Render. Comparten el mismo dominio: Sensor → Reading → Alert (sensores que emiten lecturas, que disparan alertas por umbral con máquina de estados open → acknowledged → resolved), y arquitectura en capas (routers/services/repositories/models) documentada con ADRs. Todo apunta a que nace del mismo curso (SDLC/electrónica) resuelto por cada integrante por separado.

EDSIA-BEYOND

Repositorio en puro scaffolding: casi todo vacío (pyproject.toml, requirements.txt sin contenido), sin código ni arquitectura definida aún. Es Python por convención (.gitignore), sin framework elegido. Lo único con sustancia es CONTRIBUTING.md (en la rama dev remota): flujo main protegido + dev de integración, 2 revisores obligatorios, cobertura mínima 90%, y regla de que todo el código vive en src/. El AI_LOG.md de esa misma rama confirma que la intención explícita del equipo es analizar los 3 SensorHub existentes para repartir roles de cara a EDSIA-BEYOND — es decir, este nuevo proyecto probablemente reutilizará patrones/aprendizajes de esas tres implementaciones (posiblemente una consolidación o evolución del mismo dominio de sensores, aunque eso aún no está definido).

He procesado y entendido la arquitectura y relación entre los 4 proyectos. No realicé ni propuse ningún cambio. Listo para tus siguientes instrucciones.

```
**Qué se aceptó:** N/A

**Qué se denegó:** N/A

**Qué se modificó:** N/A