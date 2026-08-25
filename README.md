<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,50:764ba2,100:00D4FF&height=180&section=header&text=Jos%C3%A9%20Luis%20Garc%C3%ADa%20Orobio&fontSize=40&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Growth%20Engineer%20%C2%B7%20AI%20Systems%20Architect&descAlignY=55&descSize=18" alt="José Luis García Orobio — Growth Engineer & AI Systems Architect" />

<a href="https://www.xperta.social">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3500&pause=900&color=00D4FF&center=true&vCenter=true&width=680&lines=Sistemas+que+automatizan+ingresos;Meta+Ads+algor%C3%ADtmico+a+escala;LLM+orchestration+en+producci%C3%B3n;Infraestructura%2C+no+scripts+sueltos" alt="Sistemas que automatizan ingresos · Meta Ads algorítmico · LLM orchestration en producción · Amazon Ads Internal · " />
</a>

<br /><br />

<a href="https://www.xperta.social"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
<a href="https://linkedin.com/in/jlgarciaorobio"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://x.com/lbaddassl"><img alt="X" src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" /></a>
<a href="https://stackoverflow.com/users/28878221/luis"><img alt="Stack Overflow" src="https://img.shields.io/badge/Stack_Overflow-F58025?style=for-the-badge&logo=stackoverflow&logoColor=white" /></a>
<a href="https://gitlab.com/lbaddass"><img alt="GitLab" src="https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white" /></a>

<br />

<img alt="Profile views" src="https://komarev.com/ghpvc/?username=lbaddass&color=00D4FF&style=flat-square&label=Profile+views" />
<img alt="Followers" src="https://img.shields.io/github/followers/lbaddass?color=764ba2&label=Followers&style=flat-square" />
<img alt="Stars" src="https://img.shields.io/github/stars/lbaddass?affiliations=OWNER%2CCOLLABORATOR&color=667eea&label=Stars&style=flat-square" />
<img alt="Basado en México, remoto" src="https://img.shields.io/badge/M%C3%A9xico-Remote%20first-2ea44f?style=flat-square" />

</div>

---

## 🧭 En una frase

Construyo **infraestructura de crecimiento**: pipelines que conectan adquisición pagada, generación creativa con IA y datos de producto en un solo sistema medible — no campañas sueltas ni scripts desechables.

> **Misión de largo plazo:** financiar programas de social-tech que enseñen ciencia e ingeniería a comunidades vulnerables en México.
> *La ingeniería es la herramienta. La educación es el resultado.*

<div align="center">

| 🎯 Enfoque | 🏗️ Rol | ⚙️ Modo de trabajo |
|:---:|:---:|:---:|
| Growth systems y Meta Ads algorítmico | Arquitecto → implementador → operador | Reproducible, medible, modular |

</div>

---

## 📊 Impacto

<!-- ⚠️ REEMPLAZA estos números por los reales antes de publicar. -->

<div align="center">

| Métrica | Resultado |
|:---|:---:|
| 💰 Ad spend gestionado con sistemas propios | **$XXX K USD** |
| 📉 Reducción de CPA en cuentas migradas a Andromeda | **-XX %** |
| 🎬 Creativos generados y testeados por mes vía pipeline IA | **XXX** |
| ⚡ Horas/mes de trabajo manual eliminadas | **XX h** |
| 🚀 Sistemas en producción mantenidos | **XX** |

</div>

---

## 🏗️ Cómo construyo — arquitectura de referencia

```mermaid
flowchart LR
    subgraph SRC["Fuentes"]
        A1["Meta Marketing API"]
        A2["Google Ads y GA4"]
        A3["Shopify y CRM"]
    end

    subgraph CORE["Núcleo de automatización"]
        B1["Ingesta<br/>Python + FastAPI"]
        B2["Estado<br/>PostgreSQL + Redis"]
        B3["Motor de decisión<br/>Andromeda"]
    end

    subgraph AI["Capa de IA"]
        C1["LLM orchestration"]
        C2["Generación creativa<br/>Veo · Runway · Kling"]
        C3["Scoring de creativos"]
    end

    subgraph OUT["Salidas"]
        D1["Activación de campañas"]
        D2["Dashboards y alertas"]
        D3["Documentación viva"]
    end

    A1 --> B1
    A2 --> B1
    A3 --> B1
    B1 --> B2 --> B3
    B3 --> C1 --> C2 --> C3
    C3 --> B3
    B3 --> D1
    B2 --> D2
    B3 --> D3
    D1 -.->|"señal de retorno"| A1

    classDef src fill:#dbeafe,stroke:#1e40af,color:#0f172a
    classDef core fill:#ede9fe,stroke:#5b21b6,color:#0f172a
    classDef ai fill:#ccfbf1,stroke:#0f766e,color:#0f172a
    classDef out fill:#fef3c7,stroke:#b45309,color:#0f172a
    class A1,A2,A3 src
    class B1,B2,B3 core
    class C1,C2,C3 ai
    class D1,D2,D3 out
```

<div align="center"><sub>El bucle cerrado es el punto: cada activación devuelve señal que alimenta la decisión siguiente.</sub></div>

---

## 🔁 Andromeda — bucle de optimización

```mermaid
sequenceDiagram
    autonumber
    participant M as Meta API
    participant E as Motor Andromeda
    participant L as Capa LLM
    participant C as Fábrica creativa

    M->>E: Métricas por ad set cada N minutos
    E->>E: Detección de fatiga y outliers
    alt Creativo agotado
        E->>L: Brief con ganadores y perdedores
        L->>C: Prompts de variantes
        C-->>E: Assets nuevos listos
        E->>M: Sube, asigna presupuesto, pausa lo muerto
    else Rendimiento estable
        E->>M: Reasignación incremental de budget
    end
    M-->>E: Nueva señal
```

---

## 🚀 Trabajo seleccionado

<table>
<tr>
<td width="50%" valign="top">

### 🔥 Andromeda Ads Engine
`🟡 Beta · Privado`

**Problema.** La optimización manual de Meta Ads no escala: la fatiga creativa aparece más rápido de lo que un humano puede reaccionar.

**Solución.** Motor en Python que lee la Marketing API en ciclos cortos, detecta degradación por ad set, dispara generación de variantes vía LLM y video IA, y reasigna presupuesto automáticamente.

**Stack.** `Python` `Meta Marketing API` `Redis` `PostgreSQL`

[Demo →](https://xperta.social)

</td>
<td width="50%" valign="top">

### 📘 EF-Élite Playbook
`🟢 Activo`

**Problema.** El conocimiento de growth vive en cabezas y capturas de pantalla; no se transfiere ni se audita.

**Solución.** Playbook versionado y desplegado como documentación viva, con procesos reproducibles y criterios de decisión explícitos.

**Stack.** `Next.js` `Python` `PostgreSQL` `MkDocs`

[Docs →](https://xperta.social)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎨 Creative Matrix
`🟡 En desarrollo`

**Problema.** Producir y clasificar cientos de variantes creativas al mes sin perder trazabilidad de qué ángulo funcionó.

**Solución.** Matriz de ángulos × formatos × hooks con generación asistida por IA y scoring de rendimiento retroalimentado.

**Stack.** `React` `TypeScript` `AI APIs`

[Preview →](https://xperta.social)

</td>
<td width="50%" valign="top">

### ⚡ Career Velocity v2
`🟢 Activo`

**Problema.** Los perfiles técnicos se desactualizan y nadie los mantiene a mano.

**Solución.** Sistema de perfil y portafolio construido sobre CI/CD: el contenido se genera, valida y publica automáticamente.

**Stack.** `Markdown` `GitHub Actions` `Automation`

[Repo →](https://github.com/lbaddass/jluisgarciaorobio)

</td>
</tr>
</table>

---

## 🧰 Stack

<details open>
<summary><b>Ver stack completo</b></summary>

<br />

**Lenguajes y frameworks**

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img alt="Vue.js" src="https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white" />
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
</p>

**Cloud e infraestructura**

<p>
  <img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img alt="Google Cloud" src="https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
  <img alt="WordPress" src="https://img.shields.io/badge/WordPress-21759B?style=for-the-badge&logo=wordpress&logoColor=white" />
  <img alt="Shopify" src="https://img.shields.io/badge/Shopify-7AB55C?style=for-the-badge&logo=shopify&logoColor=white" />
</p>

**IA y sistemas creativos**

<p>
  <img alt="LLM APIs" src="https://img.shields.io/badge/LLM_APIs-000000?style=for-the-badge&logo=openai&logoColor=white" />
  <img alt="Hugging Face" src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
  <img alt="Modelos locales" src="https://img.shields.io/badge/Modelos_locales-000000?style=for-the-badge&logo=ollama&logoColor=white" />
  <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img alt="TensorFlow" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img alt="Flow y Veo" src="https://img.shields.io/badge/Flow_%2F_Veo-00FFD1?style=for-the-badge&logo=google&logoColor=black" />
  <img alt="Runway" src="https://img.shields.io/badge/Runway-000000?style=for-the-badge" />
  <img alt="Kling AI y Sora" src="https://img.shields.io/badge/KlingAI_%2F_Sora-8A2BE2?style=for-the-badge" />
</p>

**Growth, analytics y automatización**

<p>
  <img alt="Meta Ads" src="https://img.shields.io/badge/Meta_Ads-0081FB?style=for-the-badge&logo=meta&logoColor=white" />
  <img alt="Google Ads" src="https://img.shields.io/badge/Google_Ads-4285F4?style=for-the-badge&logo=googleads&logoColor=white" />
  <img alt="GA4" src="https://img.shields.io/badge/GA4-E37400?style=for-the-badge&logo=googleanalytics&logoColor=white" />
  <img alt="Matomo" src="https://img.shields.io/badge/Matomo-3152A0?style=for-the-badge&logo=matomo&logoColor=white" />
  <img alt="Zapier" src="https://img.shields.io/badge/Zapier-FF4A00?style=for-the-badge&logo=zapier&logoColor=white" />
  <img alt="n8n" src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" />
</p>

**Datos**

<p>
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img alt="MySQL" src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img alt="Redis" src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img alt="SQLite" src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
  <img alt="Google Sheets" src="https://img.shields.io/badge/Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white" />
</p>

**Creativo y media**

<p>
  <img alt="Photoshop" src="https://img.shields.io/badge/Photoshop-31A8FF?style=for-the-badge&logo=adobephotoshop&logoColor=white" />
  <img alt="Illustrator" src="https://img.shields.io/badge/Illustrator-FF9A00?style=for-the-badge&logo=adobeillustrator&logoColor=white" />
  <img alt="Blender" src="https://img.shields.io/badge/Blender-F5792A?style=for-the-badge&logo=blender&logoColor=white" />
</p>

</details>

---

## 🧠 Principios de ingeniería

<table>
<tr>
<td width="33%" valign="top"><b>🔁 Reproducible</b><br /><sub>Si no se puede recrear desde cero con un comando, no es infraestructura: es suerte.</sub></td>
<td width="33%" valign="top"><b>📏 Medible</b><br /><sub>Cada sistema define su métrica de éxito antes de la primera línea de código.</sub></td>
<td width="33%" valign="top"><b>🧩 Modular</b><br /><sub>Piezas reemplazables. Ningún proveedor de IA o de ads es punto único de falla.</sub></td>
</tr>
<tr>
<td valign="top"><b>📚 Documentado</b><br /><sub>La documentación es parte del entregable, no un extra posterior.</sub></td>
<td valign="top"><b>⚙️ Automatizado por defecto</b><br /><sub>Lo que se hace tres veces a mano se convierte en pipeline.</sub></td>
<td valign="top"><b>💵 Orientado a P&amp;L</b><br /><sub>El código que no mueve una métrica de negocio es un pasatiempo.</sub></td>
</tr>
</table>

---

## 📈 GitHub

<div align="center">

<img height="165" alt="Estadísticas de GitHub" src="https://github-readme-stats.vercel.app/api?username=lbaddass&show_icons=true&theme=radical&hide_border=true&include_all_commits=true&count_private=true&border_radius=12" />
<img height="165" alt="Lenguajes más usados" src="https://github-readme-stats.vercel.app/api/top-langs/?username=lbaddass&layout=compact&theme=radical&hide_border=true&langs_count=8&border_radius=12" />

<br />

<img alt="Racha de contribuciones" src="https://streak-stats.demolab.com?user=lbaddass&theme=radical&hide_border=true&border_radius=12" />

<br /><br />

<!-- Requiere el workflow .github/workflows/snake.yml -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/lbaddass/lbaddass/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/lbaddass/lbaddass/output/github-contribution-grid-snake.svg" />
  <img alt="Animación snake del grafo de contribuciones" src="https://raw.githubusercontent.com/lbaddass/lbaddass/output/github-contribution-grid-snake.svg" />
</picture>

</div>

---

## 🌱 Ahora mismo

- 🔭 Escalando **Andromeda** a multi-cuenta con presupuesto compartido
- 🧪 Evaluando modelos locales para bajar el costo de inferencia de la fábrica creativa
- ✍️ Escribiendo la versión pública del **EF-Élite Playbook**
- 🎓 Diseñando el currículum del programa social-tech en México
- 📚 Aprendiendo SOPs de Amazon con el equipo de Amazon ADS Internal como CM

---

## 🤝 Trabajemos juntos

<div align="center">

Disponible para **arquitectura de sistemas de growth**, **automatización con IA** e **iniciativas de impacto social**.

<a href="https://www.xperta.social"><img alt="Hablemos" src="https://img.shields.io/badge/Hablemos-00D4FF?style=for-the-badge&logo=vercel&logoColor=black" /></a>
<a href="https://www.linkedin.com/in/jlgarciaorobio/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>

</div>

| Recurso | Qué encontrarás |
|:---|:---|
| [xperta.social](https://www.xperta.social) | Sistemas de growth engineering y frameworks de automatización |
| [LinkedIn](https://www.linkedin.com/in/jlgarciaorobio/) | Red profesional y discusión técnica |
| [Growth Playbook](https://www.xperta.social) | Documentación pública de EF-Élite, Andromeda y pipelines de IA |
| [Stack Overflow](https://stackoverflow.com/users/28878221/luis) | Huella técnica y respuestas |

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00D4FF,50:764ba2,100:667eea&height=110&section=footer" alt="" />
