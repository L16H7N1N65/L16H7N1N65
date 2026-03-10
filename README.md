div align="center">
  <img src="https://i.imgur.com/8b2zY6k.gif" width="600"/>
</div>

<div align="center">

<img src="https://img.shields.io/badge/OS-Arch_Linux-D900FF?style=for-the-badge&logo=arch-linux&logoColor=white&labelColor=1a1b26">
<img src="https://img.shields.io/badge/ROLE-Data_Engineer-00FFA3?style=for-the-badge&labelColor=1a1b26">
<img src="https://img.shields.io/badge/STATUS-Online-D900FF?style=for-the-badge&logo=server&logoColor=white&labelColor=1a1b26">
<img src="https://img.shields.io/badge/UPTIME-365d-00FFA3?style=for-the-badge&labelColor=1a1b26">

</div>

---

<div align="center">

```
┌─[ neofetch ]──────────────────────────────────┐
│                                                 │
│   handle   : L16H7N1N65                         │
│   class    : Data Engineer                      │
│   focus    : ETL · Search · RAG                 │
│   mission  : Ingest. Transform. Scale.          │
│                                                 │
│   OS      : Arch Linux x86_64                   │
│   Shell   : zsh + tmux                          │
│   Editor  : neovim                              │
│   Stack   : Python · Kafka · Solr · K8s         │
│                                                 │
└─────────────────────────────────────────────────┘
```

</div>

---

<div align="center">

```
┌─[ pipeline.arch ]────────────────────────────────────────────────────────────┐
│                                                                               │
│   WEB SOURCES          ETL PIPELINE         MESSAGE LAYER                    │
│   ┌──────────┐         ┌──────────┐         ┌──────────┐  ┌──────────┐      │
│   │ scrapers │──────▶  │transform │──────▶  │  kafka   │  │ rabbitmq │      │
│   └──────────┘         └──────────┘         └────┬─────┘  └────┬─────┘      │
│                                                   │             │            │
│                                             ┌─────▼─────────────▼────┐       │
│                                             │    PROCESSING NODE      │       │
│                                             │    normalize · enrich   │       │
│                                             └──────────┬─────────────┘       │
│                                                        │                     │
│                              ┌──────────────┬──────────▼──────┐              │
│                              │              │                 │              │
│                         ┌────▼─────┐  ┌────▼─────┐    ┌──────▼──────┐      │
│                         │ postgres │  │   solr   │    │  API / RAG  │      │
│                         │  store   │  │  search  │    │   expose    │      │
│                         └──────────┘  └──────────┘    └─────────────┘      │
│                                                                               │
└───────────────────────────────────────────────────────────────────────────────┘
```

</div>

---

<div align="center">

```
┌─[ htop ]──────────────────────────────────────────────────────────────────────┐
│                                                                                │
│  CPU  [██████████████████████████░░░░░░░]  73%    MEM  [████████████░░░░░░]  │
│  I/O  [█████████████████████████████░░░░]  87%    NET  [███████████████░░░░]  │
│                                                                                │
│  PID    PROCESS               STATUS      THROUGHPUT                          │
│  ─────────────────────────────────────────────────────                        │
│  0001   etl-pipeline          ● running   2.4M  rec/day                       │
│  0002   kafka-broker          ● running   12K   msg/sec                       │
│  0003   solr-indexer          ● running   98%   uptime                        │
│  0004   rag-api               ● running   <50ms p99 latency                   │
│  0005   k8s-scheduler         ● running   14    pods active                   │
│                                                                                │
└────────────────────────────────────────────────────────────────────────────────┘
```

</div>

---

<div align="center">

```
┌─[ projects.ls -la ]───────────────────────────────────────────────────────────┐
│                                                                                │
│  drwxr-xr-x  PROJECT X          [LIVE]  Patent data pipeline                 │
│  │           ├── ingestion · normalization · indexing · search                │
│  │           └── Python  Kafka  Solr  K8s                                     │
│                                                                                │
│  drwxr-xr-x  MINDEASE           [LIVE]  AI mental health platform             │
│  │           ├── RAG · vector search · LLM · feedback loops                  │
│  │           └── FastAPI  React  Python                                        │
│                                                                                │
│  drwxr-xr-x  REAL ESTATE AI     [LIVE]  Property intelligence platform        │
│  │           ├── scrapers · valuation · AI agents · geospatial                │
│  │           └── Scrapy  PostgreSQL  Next.js                                  │
│                                                                                │
│  drwxr-xr-x  ETL PIPELINES      [LIVE]  High-throughput ingestion             │
│              ├── crawling · stream processing · 2.4M+ rec/day                 │
│              └── Scrapy  Kafka  RabbitMQ  Solr                                │
│                                                                                │
└────────────────────────────────────────────────────────────────────────────────┘
```

</div>

---

<div align="center">

<img height="140em" src="https://github-readme-stats.vercel.app/api?username=L16H7N1N65&show_icons=true&theme=synthwave&bg_color=1a1b26&title_color=D900FF&text_color=00FFA3&icon_color=D900FF&border_color=00000000&border_radius=0&include_all_commits=true&count_private=true"/>
<img height="140em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=L16H7N1N65&layout=compact&theme=synthwave&bg_color=1a1b26&title_color=D900FF&text_color=00FFA3&border_color=00000000&border_radius=0&langs_count=6"/>

<img src="https://streak-stats.demolab.com?user=L16H7N1N65&theme=synthwave&background=1a1b26&border=00000000&stroke=D900FF&ring=D900FF&fire=00FFA3&currStreakNum=00FFA3&sideNums=00FFA3&currStreakLabel=D900FF&sideLabels=D900FF&dates=6e7681&border_radius=0"/>

</div>

---

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=L16H7N1N65&theme=radical&no-frame=true&no-bg=true&margin-w=6&column=7&border_radius=0"/>

</div>

---

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=L16H7N1N65&bg_color=1a1b26&color=00FFA3&line=D900FF&point=00FFA3&area=true&area_color=1a1b26&border_color=00000000&custom_title=COMMIT+ACTIVITY+LOG"/>

</div>

---

<div align="center">

<a href="mailto:linda.meghouche@gmail.com"><img src="https://img.shields.io/badge/EMAIL-linda.meghouche%40gmail.com-D900FF?style=for-the-badge&logo=gmail&logoColor=white&labelColor=1a1b26"/></a>
&nbsp;
<a href="https://www.linkedin.com/in/lindamg/"><img src="https://img.shields.io/badge/LINKEDIN-lindamg-00FFA3?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1a1b26"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=L16H7N1N65&label=PROFILE+VIEWS&color=D900FF&style=for-the-badge&labelColor=1a1b26"/>

<br/><br/>

```
[ session terminated — connection closed ]
```

</div>
