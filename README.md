# 🥛 IngeLac - Soluciones industriales 5.0

## 1. Descripción general

Este proyecto tiene como objetivo diseñar una planta de producción de derivados lácteos bajo un enfoque de automatización industrial y transformación digital.

La propuesta busca integrar los diferentes niveles de la organización y del proceso productivo mediante los lineamientos establecidos en las normas ISA-95 e ISA-88, permitiendo estructurar desde los procesos físicos y sistemas de control hasta los sistemas de gestión de producción y gestión empresarial.

Adicionalmente, se plantea el desarrollo de un gemelo digital de la planta que permita representar, simular y analizar el comportamiento del sistema productivo antes de su implementación física.

El proyecto contempla la integración entre tecnologías OT (Operational Technology) e IT (Information Technology), utilizando herramientas de automatización, simulación, comunicación industrial y gestión de datos.


---

# 2. Objetivos

## 2.1 Objetivo general

Diseñar una arquitectura integral de automatización y transformación digital para una planta de producción de derivados lácteos, aplicando los principios de ISA-95 e ISA-88 e integrando los niveles de proceso, control, supervisión, gestión de producción y gestión empresarial.

## 2.2 Objetivos específicos

- Diseñar la estructura general de la planta de producción.
- Definir los procesos productivos correspondientes a los derivados lácteos seleccionados.
- Identificar los principales equipos involucrados en cada proceso.
- Identificar sensores, actuadores y variables de proceso.
- Diseñar la arquitectura de automatización de la planta.
- Aplicar el modelo jerárquico propuesto por ISA-95.
- Aplicar conceptos de ISA-88 para la estructuración de procesos por lotes.
- Definir las recetas y lotes asociados a los procesos productivos.
- Diseñar una estrategia de trazabilidad de materias primas, procesos y productos terminados.
- Definir la arquitectura de comunicación entre sistemas OT e IT.
- Implementar una capa de integración utilizando Node-RED.
- Diseñar un gemelo digital de la planta.
- Simular el comportamiento del sistema productivo.
- Analizar el flujo de información entre los diferentes niveles de la organización.


---

# 3. Alcance del proyecto

El proyecto comprende el diseño conceptual y digital de una planta destinada a la fabricación de tres productos derivados de la leche.

Los productos inicialmente considerados son:

1. Queso fresco.
2. Yogurt.
3. UHT.

> Nota: Los productos pueden modificarse de acuerdo con los requerimientos y alcance final del proyecto.

El proyecto incluye las siguientes áreas:

- Recepción de materia prima.
- Almacenamiento de leche.
- Tratamiento de la leche.
- Producción de queso fresco.
- Producción de yogurt.
- Producción de UHT.
- Envasado.
- Almacenamiento de producto terminado.
- Sistemas auxiliares.
- Sistema de limpieza CIP.
- Sistema de control y supervisión.
- Gestión de producción.
- Integración con sistemas empresariales.


---

# 4. Arquitectura general del proyecto

La arquitectura del sistema se estructura utilizando como referencia el modelo funcional de ISA-95.

```text
                NIVEL 4
       Gestión empresarial - ERP
                  │
                  ▼
                NIVEL 3
       Gestión de operaciones - MES
                  │
                  ▼
                NIVEL 2
       Supervisión y control
         SCADA / HMI / PLC
                  │
                  ▼
                NIVEL 1
       Sensores y actuadores
                  │
                  ▼
                NIVEL 0
          Proceso productivo
