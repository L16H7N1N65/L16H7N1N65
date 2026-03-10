
markdown

<div align="center">

```
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║    ██╗     ██╗ ██████╗ ██╗  ██╗███████╗███╗  ██╗██╗███╗  ██╗ ██████╗ ███████╗   ║
║    ██║    ██╔╝██╔════╝ ██║  ██║╚══███╔╝████╗ ██║██║████╗ ██║██╔════╝ ██╔════╝   ║
║    ██║   ██╔╝ ██║  ███╗███████║  ███╔╝ ██╔██╗██║██║██╔██╗██║███████╗ ███████╗   ║
║    ██║  ██╔╝  ██║   ██║╚════██║ ███╔╝  ██║╚████║██║██║╚████║██╔═══╝ ╚════██║   ║
║    ███████╔╝   ╚██████╔╝     ██║███████╗██║ ╚███║██║██║ ╚███║╚██████╗ ███████║   ║
║    ╚══════╝     ╚═════╝      ╚═╝╚══════╝╚═╝  ╚══╝╚═╝╚═╝  ╚══╝ ╚═════╝ ╚══════╝   ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

</div>

<div align="center">

![](https://img.shields.io/badge/OS-Arch_Linux-%231793D1?style=flat-square&logo=archlinux&logoColor=white&labelColor=0d1117)
![](https://img.shields.io/badge/ROLE-Data_Engineer-%23E2E8F0?style=flat-square&labelColor=0d1117)
![](https://img.shields.io/badge/STATUS-Online-%2322C55E?style=flat-square&labelColor=0d1117)
![](https://img.shields.io/badge/UPTIME-365d-%231793D1?style=flat-square&labelColor=0d1117)

</div>

---

```
┌─[ neofetch ]─────────────────────────────────────────────────────────────────┐
│                                                                               │
│   ██╗     ██╗ ██████╗ ██╗  ██╗███████╗    ██████████╗                        │
│   ██╔╝    ██║██╔════╝ ██║  ██║╚══███╔╝    ╚══██╔══██║    handle   : L16H7N1N65  │
│   ██║    ██╔╝ ██║  ███╗███████║  ███╔╝        ██║  ██║    class    : Data Engineer  │
│   ██║   ██╔╝  ██║   ██║╚════██║ ███╔╝         ██║  ██║    focus    : ETL · Search · RAG  │
│   ██████╔╝    ╚██████╔╝     ██║███████╗        ██║  ██║    mission  : Ingest. Transform. Scale.  │
│   ╚═════╝      ╚═════╝      ╚═╝╚══════╝       ╚═╝  ╚═╝                       │
│                                                                               │
│   OS      : Arch Linux x86_64          Shell   : zsh + tmux                  │
│   WM      : i3wm                       Editor  : neovim                      │
│   Stack   : Python · Kafka · Solr · K8s · PostgreSQL · FastAPI               │
│   Uptime  : 365d 0h 0m                 Packages: 2.4M+ rec/day               │
│                                                                               │
└───────────────────────────────────────────────────────────────────────────────┘
```

---

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

---

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

---

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

---

<div align="center">

```
┌─[ github.stats ]──────────────────────────────────────────────────────────────┐
```

</div>

<div align="center">

<img height="160em" src="https://github-readme-stats.vercel.app/api?username=L16H7N1N65&show_icons=true&theme=github_dark&bg_color=0d1117&title_color=1793D1&text_color=c9d1d9&icon_color=1793D1&border_color=30363d&border_radius=0&include_all_commits=true&count_private=true"/>
<img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=L16H7N1N65&layout=compact&theme=github_dark&bg_color=0d1117&title_color=1793D1&text_color=c9d1d9&border_color=30363d&border_radius=0&langs_count=6"/>

</div>

<div align="center">

<img src="https://streak-stats.demolab.com?user=L16H7N1N65&theme=github-dark-blue&background=0d1117&border=30363d&stroke=1793D1&ring=1793D1&fire=e05d44&currStreakNum=c9d1d9&sideNums=c9d1d9&currStreakLabel=1793D1&sideLabels=1793D1&dates=6e7681&border_radius=0"/>

</div>

<div align="center">

```
└────────────────────────────────────────────────────────────────────────────────┘
```

</div>

---

```
┌─[ trophy.ls ]──────────────────────────────────────────────────────────────────┐
```

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=L16H7N1N65&theme=onestar&no-frame=true&no-bg=true&margin-w=6&column=7"/>
</div>

```
└────────────────────────────────────────────────────────────────────────────────┘
```

---

```
┌─[ activity.log ]───────────────────────────────────────────────────────────────┐
```

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=L16H7N1N65&bg_color=0d1117&color=1793D1&line=1793D1&point=c9d1d9&area=true&area_color=0d2137&border_color=30363d&custom_title=COMMIT+ACTIVITY+LOG"/>
</div>

```
└────────────────────────────────────────────────────────────────────────────────┘
```

---

<div align="center">

```
┌─[ contact ]────────────────────────────────────────────────────────────────────┐
│                                                                                │
│           $ ssh linda.meghouche@gmail.com                                      │
│           $ curl https://linkedin.com/in/lindamg                               │
│                                                                                │
└────────────────────────────────────────────────────────────────────────────────┘
```

<a href="mailto:linda.meghouche@gmail.com"><img src="https://img.shields.io/badge/EMAIL-linda.meghouche%40gmail.com-%231793D1?style=flat-square&logo=gmail&logoColor=white&labelColor=0d1117"/></a>
&nbsp;
<a href="https://www.linkedin.com/in/lindamg/"><img src="https://img.shields.io/badge/LINKEDIN-lindamg-%231793D1?style=flat-square&logo=linkedin&logoColor=white&labelColor=0d1117"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=L16H7N1N65&label=PROFILE+VIEWS&color=1793D1&style=flat-square&labelColor=0d1117"/>

<br/><br/>

```
[ session terminated — connection closed ]
```

</div>