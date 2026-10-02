# 🧠 Reinforcement Learning

<p align="center">

## Reinforcement Learning

### Talleres, prácticas y experimentos académicos

<br>

**Jheansel Hasler Beltrán Forero**  
**Andres Felipe Cuervo Torres**

</p>

---

## 📚 Sobre este repositorio

Este repositorio contiene el desarrollo de los talleres, prácticas,
implementaciones y experimentos realizados durante el curso de
**Reinforcement Learning**.

El contenido se organiza de manera progresiva, comenzando con métodos
tabulares y avanzando hacia métodos basados en aproximación de funciones
y aprendizaje por refuerzo profundo.

El repositorio está diseñado para incorporar nuevos talleres a medida
que avance el curso, manteniendo una estructura organizada para el
código, notebooks, configuraciones, experimentos y resultados.

---

## 🎯 Objetivos del repositorio

- Implementar algoritmos fundamentales de Reinforcement Learning.
- Comprender los principales conceptos del aprendizaje por refuerzo.
- Trabajar con Markov Decision Processes (MDP).
- Analizar estados, acciones, recompensas y políticas.
- Implementar métodos basados en modelos conocidos.
- Implementar métodos basados en experiencia.
- Estudiar métodos de Monte Carlo.
- Estudiar métodos de Temporal Difference.
- Implementar métodos basados en funciones de valor.
- Explorar métodos de aproximación de funciones.
- Implementar algoritmos de Deep Reinforcement Learning.
- Analizar los resultados obtenidos mediante experimentación.
- Documentar progresivamente el trabajo desarrollado durante el curso.

---

# 🗺️ Roadmap del curso

La siguiente estructura representa la organización general de los
métodos de Reinforcement Learning abordados durante el curso.

```text
                         REINFORCEMENT LEARNING
                                  │
                 ┌────────────────┴────────────────┐
                 │                                 │
                 ▼                                 ▼
         TABULAR METHODS                 FUNCTION APPROXIMATION
                 │                                 │
        ┌────────┴────────┐              ┌─────────┴─────────┐
        │                 │              │                   │
        ▼                 ▼              ▼                   ▼
  KNOWN MODEL       UNKNOWN MODEL   UNKNOWN MODEL       LEARNED MODEL
        │                 │              │                   │
        │                 │              │                   │
        ├── Linear        ├── Monte      ├── DQN             └── World
        │   System       │   Carlo      │                      Models
        │   Solving      │              │
        │                 ├── SARSA      ├── Policy
        ├── Policy        │              │   Gradient
        │   Evaluation    │              │
        │                 └── Q-Learning └── Actor-Critic
        │
        ├── Policy
        │   Iteration
        │
        └── Value
            Iteration
```

---

# 🧩 Contenidos del curso

## 1. Tabular Methods

Los métodos tabulares permiten representar explícitamente los estados,
acciones y valores asociados a un problema de Reinforcement Learning.

### Known Model

Cuando el modelo del entorno es conocido:

- Linear System Solving
- Policy Evaluation
- Policy Iteration
- Value Iteration

### Unknown Model

Cuando el modelo del entorno no es conocido y el agente aprende a partir
de la experiencia:

- Monte Carlo
- SARSA
- Q-Learning

---

## 2. Function Approximation Methods

Cuando el espacio de estados o acciones es demasiado grande para utilizar
tablas explícitas, se utilizan aproximadores de funciones.

Los principales métodos considerados son:

- Deep Q-Networks (DQN)
- Policy Gradient
- Actor-Critic
- World Models

---

# 📊 Progreso del curso

## Tabular Methods

- [x] Dynamic Programming
- [ ] Monte Carlo
- [ ] Temporal Difference — SARSA
- [ ] Temporal Difference — Q-Learning

## Function Approximation Methods

- [ ] Deep Q-Networks (DQN)
- [ ] Policy Gradient
- [ ] Actor-Critic
- [ ] World Models

---

# 📝 Talleres

| # | Taller | Tema principal | Estado |
|---|---|---|---|
| 01 | Dynamic Programming | Policy Evaluation, Policy Iteration y Value Iteration | ✅ Completado |
| 02 | Monte Carlo | Monte Carlo Methods | ⏳ Pendiente |
| 03 | SARSA | Temporal Difference — SARSA | ⏳ Pendiente |
| 04 | Q-Learning | Temporal Difference — Q-Learning | ⏳ Pendiente |
| 05 | DQN | Deep Q-Networks | ⏳ Pendiente |
| 06 | Policy Gradient | Policy Gradient Methods | ⏳ Pendiente |
| 07 | Actor-Critic | Actor-Critic Methods | ⏳ Pendiente |
| 08 | World Models | World Models | ⏳ Pendiente |

---

# 📂 Estructura del repositorio

```text
reinforcement_learning/
│
├── README.md
│
├── .gitignore
│
├── recursos/
│
└── talleres/
    │
    ├── 01-dynamic-programming/
    │
    ├── 02-monte-carlo/
    │
    ├── 03-sarsa/
    │
    ├── 04-q-learning/
    │
    ├── 05-dqn/
    │
    ├── 06-policy-gradient/
    │
    ├── 07-actor-critic/
    │
    └── 08-world-models/
```

> Las carpetas correspondientes a los talleres futuros serán incorporadas
> progresivamente a medida que se desarrollen las actividades.

---

# 📁 Organización de cada taller

Cada taller puede tener una estructura independiente dependiendo de
los requerimientos de la actividad.

Una estructura de referencia es:

```text
XX-nombre-del-taller/
│
├── README.md
│
├── notebooks/
│
├── src/
│
├── configs/
│
├── data/
│
├── results/
│
├── models/
│
├── requirements.txt
│
└── pyproject.toml
```

No todos los talleres necesariamente tendrán todas estas carpetas.

---

# 🚕 Taller 01 — Dynamic Programming

## Descripción

El primer taller aborda los fundamentos de **Dynamic Programming**
aplicados a Reinforcement Learning.

El taller trabaja métodos que permiten evaluar y mejorar políticas
utilizando un modelo conocido del entorno.

Los principales métodos implementados son:

- Linear System Solving
- Policy Evaluation
- Policy Iteration
- Value Iteration

---

## 🧠 Conceptos principales

Durante este taller se trabajan conceptos relacionados con:

- Markov Decision Processes (MDP)
- Estados
- Acciones
- Recompensas
- Probabilidades de transición
- Políticas
- Funciones de valor
- State Value Function
- Action Value Function
- Bellman Equation
- Bellman Optimality Equation
- Policy Evaluation
- Policy Improvement
- Policy Iteration
- Value Iteration

---

## 🔬 Métodos implementados

### Linear System Solving

Resolución directa del sistema de ecuaciones asociado a una política
para obtener su función de valor.

### Policy Evaluation

Evaluación iterativa de una política para estimar la función de valor
de los estados.

### Policy Iteration

Proceso iterativo que combina evaluación y mejora de políticas:

```text
Policy Evaluation
        │
        ▼
Policy Improvement
        │
        ▼
Policy Evaluation
        │
        ▼
Policy Improvement
        │
        ▼
       ...
```

El proceso continúa hasta alcanzar una política estable.

### Value Iteration

Método basado en la actualización iterativa de los valores de los
estados mediante la ecuación de optimalidad de Bellman.

---

## 🚖 Entorno utilizado

El taller utiliza un entorno basado en un problema tipo Taxi:

```text
MilanTaxiEnv
```

El entorno permite estudiar los métodos tabulares utilizando un espacio
de estados y acciones definido explícitamente.

---

## 📓 Contenido del taller

Los archivos correspondientes al primer taller se encuentran en:

```text
talleres/01-dynamic-programming/
```

La carpeta contiene los notebooks, código fuente, configuraciones y
archivos necesarios para ejecutar los experimentos.

---

## 🔗 Repositorio de referencia

El desarrollo inicial del taller se encuentra en:

**Taller 1 — Dynamic Programming**

https://github.com/Cuervinho/Taller-1-Dynamic-Programming

---

# 🛠️ Tecnologías y herramientas

## Lenguaje

- Python

## Reinforcement Learning

- Gymnasium
- Stable-Baselines3

## Computación científica

- NumPy
- SciPy
- Pandas

## Machine Learning / Deep Learning

- PyTorch

## Visualización

- Matplotlib

## Desarrollo experimental

- Jupyter Notebook

## Control de versiones

- Git
- GitHub

---

# 🧪 Metodología de trabajo

Cada taller seguirá, en la medida de lo posible, el siguiente flujo:

```text
             PROBLEMA
                 │
                 ▼
           FORMULACIÓN
                 │
                 ▼
           IMPLEMENTACIÓN
                 │
                 ▼
            EXPERIMENTOS
                 │
                 ▼
         ANÁLISIS DE RESULTADOS
                 │
                 ▼
           DOCUMENTACIÓN
                 │
                 ▼
               COMMIT
                 │
                 ▼
              GITHUB
```

---

# 📈 Seguimiento de experimentos

Cuando sea necesario, cada taller podrá incluir:

- Resultados numéricos
- Gráficas
- Tablas
- Comparaciones entre algoritmos
- Análisis de convergencia
- Evaluación de políticas
- Evaluación de recompensas
- Métricas de desempeño
- Modelos entrenados

Los resultados específicos dependerán de las características de cada
actividad.

---

# 📊 Progreso

### Talleres completados

```text
1 / 8
```

### Progreso actual

```text
[██░░░░░░] 12.5%
```

### Estado

```text
Dynamic Programming     ████████████████████  COMPLETADO
Monte Carlo             ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
SARSA                   ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
Q-Learning              ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
DQN                     ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
Policy Gradient         ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
Actor-Critic            ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
World Models            ░░░░░░░░░░░░░░░░░░░░  PENDIENTE
```

---

# 🤝 Trabajo colaborativo

El repositorio se desarrolla de manera colaborativa mediante Git y
GitHub.

El control de versiones permite:

- Mantener un historial de cambios.
- Trabajar de manera colaborativa.
- Crear ramas para nuevas actividades.
- Integrar cambios mediante Pull Requests.
- Mantener organizada la evolución del proyecto.
- Documentar las diferentes versiones de los talleres.

---

# 📌 Convención de nombres

Los talleres seguirán una numeración consecutiva:

```text
01-dynamic-programming
02-monte-carlo
03-sarsa
04-q-learning
05-dqn
06-policy-gradient
07-actor-critic
08-world-models
```

La numeración permite mantener los talleres organizados y facilita
su navegación dentro del repositorio.

---

# 📚 Recursos

Los recursos complementarios del curso podrán almacenarse en:

```text
recursos/
```

Esta carpeta puede contener material complementario, referencias,
configuraciones generales o documentación compartida entre diferentes
talleres.

---

# 🚀 Estado del proyecto

**Curso en desarrollo**

```text
┌─────────────────────────────────────────────┐
│          REINFORCEMENT LEARNING             │
├─────────────────────────────────────────────┤
│                                             │
│  01  Dynamic Programming       ✅           │
│  02  Monte Carlo               ⏳           │
│  03  SARSA                     ⏳           │
│  04  Q-Learning                ⏳           │
│  05  DQN                       ⏳           │
│  06  Policy Gradient           ⏳           │
│  07  Actor-Critic              ⏳           │
│  08  World Models              ⏳           │
│                                             │
└─────────────────────────────────────────────┘
```

---

# 👥 Integrantes

### Jheansel Hasler Beltrán Forero

Estudiante y desarrollador del proyecto.

### Andres Felipe Cuervo Torres

Estudiante y desarrollador del proyecto.

---

# 📖 Referencias

Las referencias bibliográficas y fuentes utilizadas en cada actividad
serán documentadas dentro del README correspondiente a cada taller.

---

<p align="center">

**Reinforcement Learning**

**Jheansel Hasler Beltrán Forero · Andres Felipe Cuervo Torres**

Repositorio académico

</p>
