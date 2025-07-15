# databases-cheat-sheet


- https://github.com/surrealdb/surrealdb


 Supabase — An Open-Source Alternative to Firebase


<br><br>
<br><br>

---

<br><br>
<br><br>


# logs

## parseabl
- https://github.com/parseablehq/parseable?tab=readme-ov-file









<br><br>
<br><br>

---

<br><br>
<br><br>

https://github.com/TanStack/db?utm_source=tldrwebdev


<br><br>
<br><br>


# Vector

## HelixDB 
- HelixDB is an open-source, high-performance graph-vector database written in Rust designed for RAG and AI applications. It combines graph and vector data storage, using LMDB for data persistence and ACID compliance. 







## server-less


# Turbopuffer

<details><summary>Click to expand..</summary>

**Ja**, das ist eine **Vector Database** – aber nicht irgendeine. **Turbopuffer** (grandioser Name übrigens) ist ein **serverloses Vektor- und Volltext-Suchsystem**, das:

### 🔍 **Was macht Turbopuffer konkret?**

Es kombiniert:

* **Vektorbasierte Suche** (für Embeddings, also semantische Suche z. B. bei LLMs),
* **Full-text Search** (klassische Schlagwortsuche),
* und speichert das Ganze **direkt auf Object Storage** wie **Amazon S3** – also **ohne klassische Datenbankserver**.

### 🚀 Architektur (vereinfacht):

```
Client ➜ API ➜ In-Memory SSD Cache ➜ Object Storage (S3)
```

Klingt nach: „Keep hot stuff fast, keep big stuff cheap.“

---

### 💸 **Was ist besonders daran?**

| Feature             | Turbopuffer                       |
| ------------------- | --------------------------------- |
| ✅ Serverless        | Kein Cluster, keine Maschinen     |
| ✅ Cheap AF          | S3-Level Kosten (z. B. \$0.33/GB) |
| ✅ High-Scale        | 150 Mrd. Dokumente, 6K+ QPS       |
| ✅ Hybrid-Search     | Vector + Full-Text                |
| ✅ Fast cold start   | Millisekunden-Range               |
| ✅ SSD Caching       | Für warme Daten                   |
| ✅ Embedding support | GPT/OpenAI kompatibel             |
| ✅ Fully managed     | Plug & Query                      |

---

### ⚙️ Typische Anwendung:

**Beispiel:** Du hast 1 Million Produktbeschreibungen und willst semantisch suchen („Zeig mir Produkte wie das hier…“) — aber *billig* und *schnell*. Turbopuffer erlaubt dir:

* `insert(vector, metadata)`
* `search("ähnlich zu diesem Vektor", topK=10)`
* `filter(price > 10 && category == 'Tools')`

---

### 📊 Performance (laut ihrer Benchmarks):

* **p50 (warm):** 16 ms
* **p99 (warm):** 33 ms
* **p99 (cold):** \~677 ms (immer noch okay für S3)

---

### 🤯 TL;DR:

**Turbopuffer** ist:

* eine **moderne, serverlose Vektor+FTS-Datenbank**
* **optimiert für Preis, Skalierung und Einfachheit**
* **besonders geeignet für LLM/RAG-Anwendungen**
* und versucht, **Weaviate**, **Pinecone**, **Qdrant** & Co den Rang abzulaufen — **für 10x weniger Geld**.

Wäre wie wenn Pinecone und Typesense zusammen ein Kind mit AWS S3 zeugen. 👶📦

Willst du ein Projekt drauf aufsetzen?

</details>
















---------------


 LiveStore is a next-generation state management framework based on reactive SQLite and built-in sync engine.
livestore.dev 







 Instant DB (Tool)

Give your frontend a real-time database that handles optimistic updates, multiplayer sync, offline mode, and collaboration features automatically. 




AlloyDB AI's ScaNN Index Boosts Vector and Hybrid Search Performance (5 minute read)

AlloyDB AI now integrates Google Research's ScaNN index to accelerate vector similarity searches by up to 3x and enable hybrid queries combining keyword and embedding-based retrieval. By supporting both dense and sparse data types, as well as custom distance metrics, ScaNN delivers sub-millisecond lookup times at scale. This enhancement sharpens relevance and recall across use cases while preserving AlloyDB's managed, serverless simplicity and strong consistency guarantees.
MindsDB (GitHub Repo)

MindsDB is an open-source platform designed to deliver answers from data scattered across disparate data sources. It handles query federation over structured and unstructured data sources, definition of unified views of knowledge bases, and natural language data queries. The server can be deployed via Docker or PyPI. It is available on the AWS Marketplace. A demo playground is available. 
