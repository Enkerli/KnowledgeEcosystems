# Knowledge Ecosystems: Parallel Timelines

An interactive visualization exploring the parallel evolution of disciplines, institutions, and knowledge regimes from 20,000 BCE to the present day.

**[View the live visualization →](https://github.com/[username]/KnowledgeEcosystems)** *(Update this link after deployment)*

## Overview

This project presents a synchronized, three-track timeline that traces the development of knowledge systems across human history. It visualizes how scientific disciplines, educational institutions, and broader knowledge regimes have evolved, intersected, and influenced one another over millennia.

### Key Features

- **487 historical entries** spanning from 20,000 BCE to 2020 CE
- **Three parallel tracks**: Disciplines, Institutions, and Knowledge Regimes
- **13 thematic storylines** for filtered exploration:
  - Women and gender
  - Credentialism and professionalization
  - Applied and mission-oriented research
  - Indigenous and decolonial perspectives
  - Regional focuses (Aotearoa New Zealand, Vietnam)
  - Knowledge hubs and networks
  - State and policy leadership
  - Cultural movements and circles
  - Language sciences
  - Health and wellness
  - Engineering disciplines
  - Civilization Tech Tree
- **Interactive exploration**: Click entries to see connections, filter by region, category, or time period
- **Global coverage**: Includes non-Western knowledge traditions (Buddhist universities, Islamic madrasas, Sanskrit cosmopolis, Silk Road networks)
- **Cross-references**: Visual links showing how different events and institutions influenced each other

## Dataset Highlights

### Ancient Knowledge Systems
- Writing systems and administrative recordkeeping (3400 BCE)
- Agricultural revolution and crop domestication (10,000 BCE)
- Astronomical observatories (700 BCE)
- Coinage and monetary systems (650 BCE)
- Early postal and courier infrastructures (550 BCE)

### Global Knowledge Networks
- Silk Road caravan cities and broker networks (130-1500 CE)
- Sanskrit cosmopolis and transregional exchange (400-1400 CE)
- Arabic scholarly and commercial lingua franca (650-1800 CE)
- Persianate cosmopolis and scribal mobility (900-1900 CE)
- Swahili coastal trade networks (1000 CE-present)

### Non-Western Institutions
- Buddhist monastic universities (427-1400 CE)
- al-Qarawiyyin and trans-Maghrebi scholarly networks (859 CE-present)
- Nizamiyya madrasa networks (1067-1258 CE)
- Confucian academy traditions (1179-1905 CE)
- Imperial examination systems (605-1905 CE)

### Civilization Tech Tree
43 foundational technologies modeled after the *Civilization* game series:
- Ancient Era: Agriculture, Pottery, Bronze/Iron Working, The Wheel, Writing
- Classical/Medieval: Mathematics, Astronomy, Philosophy, Gunpowder, Printing Press
- Industrial Era: Steam Power, Railroad, Electricity, Internal Combustion
- Modern Era: Flight, Rocketry, Computers, Nuclear Technology, Lasers

## Using the Visualization

1. **Browse the timeline**: Scroll horizontally to explore different time periods
2. **Filter by storyline**: Click storyline chips to focus on specific themes
3. **Select entries**: Click any bar to see detailed information and related events
4. **Adjust time window**: Use range sliders to zoom into specific periods
5. **Filter by category**: Use dropdowns to filter by region, category, or track
6. **Follow connections**: Purple curves show relationships between entries

## Project Structure

```
KnowledgeEcosystems/
├── index.html          # Interactive visualization webapp
├── data.json           # 487 historical entries with metadata
├── LICENSE             # CC0 1.0 Universal Public Domain Dedication
├── README.md           # This file
└── .gitignore          # Git ignore rules
```

## Technical Details

### Data Structure

Each entry in `data.json` contains:

```json
{
  "id": "e1",
  "title": "Event title",
  "track": "Disciplines|Institutions|Knowledge Regimes",
  "category": "Event category",
  "region": "Geographic region",
  "start": -3000,
  "end": 2025,
  "description": "Detailed description...",
  "links": ["e2", "e3"],
  "tags": ["Tag1", "Tag2"],
  "perspectives": ["General", "Storyline name"]
}
```

### Technology Stack

- **Frontend**: Pure HTML, CSS, JavaScript (no dependencies)
- **Visualization**: SVG with custom lane layout algorithm
- **Data**: JSON format for easy editing and extension
- **Deployment**: Github Pages (static hosting)

## Dataset Methodology

This dataset was created through:

1. **Historical research**: Key dates verified against scholarly sources
2. **Global perspective**: Deliberate inclusion of non-Western knowledge traditions
3. **Interdisciplinary scope**: Covering sciences, humanities, social sciences, and technologies
4. **Decolonial lens**: Recognition of biopiracy, colonial extraction, and indigenous knowledge systems
5. **Merged sources**: Integration of canonical events with expanded storylines

### Date Accuracy

- Ancient dates (pre-500 BCE): Approximate, based on archaeological and historical consensus
- Classical/Medieval (500 BCE-1500 CE): Generally accurate within ±25 years
- Early Modern (1500-1800): Accurate within ±10 years
- Modern (1800+): Precise dates verified against primary sources

## Contributing

This dataset is released under CC0 (public domain). Contributions are welcome!

### How to Contribute

1. Fork this repository
2. Add or modify entries in `data.json`
3. Ensure entries follow the data structure format
4. Verify dates against reliable sources
5. Submit a pull request with:
   - Description of changes
   - Source citations for new entries
   - Rationale for modifications

### Areas for Expansion

- **Regional depth**: More entries for Africa, Latin America, Oceania
- **Underrepresented fields**: More coverage of arts, music, literature
- **20th-21st century**: Denser coverage of recent developments
- **Citations**: Add source references for all entries
- **Translations**: Multi-language support for global accessibility

## Use Cases

- **Education**: Teaching history of science, technology, and institutions
- **Research**: Exploring interdisciplinary connections and knowledge flows
- **Public engagement**: Museum exhibits, digital humanities projects
- **Data journalism**: Visualizing historical trends and patterns
- **Game design**: Reference for historically-grounded tech trees and progression systems

## Known Limitations

- **Western bias**: Despite efforts, some regions remain underrepresented
- **Simplification**: Complex historical processes reduced to single events
- **Dates**: Some ancient dates are approximations or scholarly consensus
- **Selection bias**: 487 entries cannot capture all significant developments
- **Language**: Currently English-only (contributions for translations welcome)

## Credits

Dataset compiled and curated as an open educational resource. Special acknowledgment to:

- Historical scholarship informing entry dates and descriptions
- *Civilization* game series for tech tree inspiration
- Global knowledge traditions often marginalized in Western-centric histories

## License

This work is dedicated to the public domain under the [CC0 1.0 Universal Public Domain Dedication](LICENSE).

You are free to:
- Copy, modify, and distribute the dataset
- Use it for commercial or non-commercial purposes
- Create derivative works
- Use it without attribution (though attribution is appreciated)

## Citation

If you use this dataset in academic work, consider citing:

```
Knowledge Ecosystems: Parallel Timelines Dataset (2025).
Available at: https://github.com/[username]/KnowledgeEcosystems
Released under CC0 1.0 Universal Public Domain Dedication.
```

## Links

- **Live Demo**: *[Add Github Pages URL after deployment]*
- **Repository**: *[Add Github repo URL]*
- **Issues**: *[Add Github issues URL]*
- **Discussions**: *[Add Github discussions URL]*

---

**Last Updated**: March 2025
**Dataset Version**: 1.0
**Total Entries**: 487
**Timeline Coverage**: 20,000 BCE - 2020 CE
