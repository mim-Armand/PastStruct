# PastStruct
A structured data specification for standardized storage and exchange of historical event information.


# PastStruct Specification

**PastStruct** is an open and standardized data specification designed for the structured storage, exchange, and interoperability of historical event data. Inspired by successful data standards like FHIR in healthcare, PastStruct aims to streamline the representation of historical information, facilitating accurate data sharing and integration across diverse historical research platforms and archives.

---

## 🎯 Purpose

Historical data is often fragmented, stored in incompatible formats, and difficult to share consistently. PastStruct solves these challenges by providing a clear, flexible, and universally understandable schema for historical events, empowering historians, archivists, researchers, educators, and developers.

---

## 🚀 Key Features

- **Standardized Schema:** Robust JSON-based schema ensuring uniformity and clarity.
- **Interoperable:** Facilitates easy integration across various digital archives, tools, and services.
- **Rich Metadata:** Comprehensive metadata capture including sources, citations, event context, participants, and location.
- **Extensible:** Easily adaptable schema to accommodate specialized historical domains and custom requirements.
- **Version Control:** Clearly defined versioning to maintain historical accuracy and data integrity.
- **Dynamic Priority:** Assign event importance to enable intuitive timeline visualizations, ensuring clarity when zooming in and out.

---

## 📋 Schema Overview

```json
{
  "id": "uuid",
  "type": "event-type",
  "emoji": "🎯",
  "categories": [
    {
      "main": "Category Name",
      "sub": "Subcategory Name"
    }
  ],
  "funFacts": [
    "Interesting fact about the event",
    "Another engaging detail",
    "Memorable historical tidbit",
    "Educational insight"
  ],
  "description": "Detailed description of the historical event.",
  "dateRange": {
    "from": "ISO8601 date",
    "to": "ISO8601 date",
    "precision": "exact/year/month/day"
  },
  "priority": {
    "range": 10,
    "level": "integer (1-10)",
    "description": "Significance of the event, with 1 being least and 10 being most important."
  },
  "entities": [
    {
      "id": "uuid",
      "label": "Name of entity",
      "entityType": "person/place/group/nation"
    }
  ],
  "location": {
    "address": "Optional address or location name",
    "country": "Country name",
    "coordinates": {
      "lat": "latitude float",
      "long": "longitude float"
    }
  },
  "relationships": [
    {
      "type": "preceded-by/succeeded-by/part-of",
      "reference": "related event uuid"
    }
  ],
  "citations": [
    {
      "citationId": "uuid",
      "referenceType": "textual/artifact/multimedia",
      "title": "Citation title",
      "link": "uri"
    }
  ],
  "additionalInfo": {
    "notes": "Additional contextual information or annotations.",
    "keywords": ["relevant", "tags"]
  },
  "metadata": {
    "created": "ISO8601 date",
    "modified": "ISO8601 date",
    "version": "version number"
  }
}
```

---

## 📖 Documentation

Comprehensive documentation including detailed schema definitions, examples, and guidelines can be found in the `/docs` directory.

### 📂 Category System

PastStruct uses a comprehensive 17-category classification system to organize historical events thematically. Each category includes multiple subcategories for precise classification.

**Category File**: `category.yml` in the root directory contains the complete category system with:
- 17 main categories with emojis and descriptions
- 6-8 subcategories per main category
- Usage guidelines and best practices
- Version information and maintenance details

**Key Categories Include**:
- 🛡️ **War & Conflict** - Military events, revolutions, treaties
- 👑 **Politics & Government** - Dynasties, elections, leadership changes
- ✝️🕉️☪️✡️ **Religion & Spirituality** - Religious developments and conflicts
- 🧠 **Philosophy & Ideas** - Intellectual movements and philosophical works
- 🎨 **Art & Culture** - Cultural movements and artistic developments
- 🧬 **Science & Discovery** - Scientific breakthroughs and innovations
- ⚙️ **Industry & Technology** - Industrial revolutions and technological advances
- 💰 **Economics & Trade** - Economic systems and trade networks
- 🧭 **Exploration & Expansion** - Geographic discoveries and colonization
- ⚖️ **Law & Justice** - Legal systems and human rights milestones
- 👥 **Society & Daily Life** - Social structures and cultural practices
- 🌍 **Environment & Climate** - Environmental changes and natural disasters
- 🦠 **Health & Medicine** - Medical developments and public health
- 🌐 **Media & Communication** - Communication technologies and media
- 🌎 **Globalization & International Relations** - International cooperation and diplomacy
- 🪙 **Economy of Knowledge** - Knowledge systems and education
- 🧩 **Historical Mysteries & Controversies** - Unexplained events and debates

**Benefits of the Category System**:
- **Multi-dimensional Classification**: Events can belong to multiple categories
- **Flexible Filtering**: Users can filter events by theme, era, or type
- **Thematic Organization**: Related events can be grouped and analyzed together
- **Educational Value**: Categories help learners understand historical themes and connections
- **Search Enhancement**: Categories improve searchability and discovery

---

## 🛠️ Contributing

Contributions are warmly welcomed! Please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Commit your changes: `git commit -am 'Add your feature description'`.
4. Push to your branch: `git push origin feature/your-feature-name`.
5. Open a Pull Request with a clear description of your changes.

---

## 📜 License

PastStruct is released under the [MIT License](LICENSE), enabling open and unrestricted usage across academic, non-profit, and commercial applications.

---

## 📧 Contact

Have questions or feedback? Open an issue or contact the maintainers:

- **Contributors** - [my Linkedin]([mailto\:your.email@example.com](https://www.linkedin.com/in/3dots/))

---

🌐 Visit us online at [paststruct.io](https://PastStruct.com)

**Together, let's build the future of historical data interoperability!**

