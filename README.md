# Sims 4 API 🎭 - Sims 4 Game Data Explorer

An experimental API for exploring **Sims 4 traits, careers, and more**—built to support a future planner app that helps users design Sims with purpose, not chaos.  

Hosted on [Render](https://render.com/), backed by PostgreSQL on [Neon](https://neon.tech/), and built with love.

---

## ✨ What It Does

This API serves as a foundation for an upcoming planner app. Currently, it allows basic retrieval of Sims 4 data, with a focus on traits. Future updates will support filtering, categorization, and more advanced planning logic.

### 🛠️ Current capabilities

- Retrieve all available traits (`/traits`)
- Returns structured JSON with name, description, ages, species, occults and game packs

### 🧪 In the works

- Trait types (e.g. CAS, Aspiration Reward, etc)
- Search and filtering
- More data: Careers, Aspirations, Worlds, Lots, etc

---

## 🔌 API Access

**Base URL:**  
`https://sims-api.onrender.com/api`

### Example: Get all traits

```http
GET /api/traits
```

## 🧪 Example Output

```json
{
  "name": "Wild",
  "description": "Spirited and full of Energy. These Toddlers love to explore...",
  "ages": "Toddler",
  "species": "Human",
  "occults": "Alien, Merfolk, Spellcaster, Vampire, Werewolf",
  "packs": "Base Game"
}
```
---

## ⚙️ Tech Stack
- FastAPI (Python)
- PostgreSQL (hosted on Neon)
- Render for deployment
- SQLAlchemy ORM + raw SQL for aggregations
