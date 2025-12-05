# 🏅 LA28 Olympics Glory Dashboard

**Paris 2024 Olympic Games Data Explorer**

A comprehensive multi-page Streamlit dashboard visualizing data from the Paris 2024 Olympic Games. Built for the LA28 Volunteer Selection Challenge.

---

## 📋 Features

### Page 1: Overview (Command Center)
- 5 Key Performance Indicators (Athletes, Countries, Sports, Medals, Events)
- Global Medal Distribution (Donut Chart)
- Top 10 Medal Standings (Stacked Bar Chart)
- Interactive filters (Country, Sport, Medal Type, Continent)

### Page 2: Global Analysis (World View)
- World Medal Map (Choropleth)
- Medal Hierarchy by Continent (Sunburst & Treemap)
- Continent vs Medals (Grouped Bar Chart)
- Top 20 Countries by Medals (Grouped Bar Chart)

### Page 3: Athlete Performance (Human Story)
- Athlete Profile Card with Search
- Age Distribution (Box & Violin Plots)
- Gender Distribution (by World/Continent/Country)
- Top Athletes by Medals (Stacked Bar Chart)

### Page 4: Sports & Events (Competition Arena)
- Event Schedule (Gantt/Timeline Chart)
- Medal Count by Sport (Treemap)
- Olympic Venues Map (Scatter Mapbox)

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- pip

### Installation

1. Clone the repository:
```bash
git clone https://github.com/AbdallahYettou/olympics_dashboard.git
cd olympics_dashboard
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
venv\Scripts\activate     # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the dashboard:
```bash
streamlit run Overview.py
```

5. Open your browser at `http://localhost:8501`

---

## 📁 Project Structure

```
olympics_dashboard/
├── Overview.py           # Main page
├── pages/
│   ├── Global_Analysis.py
│   ├── Athlete_Performance.py
│   └── Sports_and_Events.py
├── data/                       # Paris 2024 Olympic data
│   ├── athletes.csv
│   ├── medals.csv
│   ├── medals_total.csv
│   ├── medallists.csv
│   ├── events.csv
│   ├── nocs.csv
│   ├── schedules.csv
│   ├── venues.csv
│   └── ...
├── utils/
│   ├── shared_filters.py       # Global filter functions
│   ├── data_ingest.py          # Data loading functions
│   └── mappers.py              # Country/continent mappings
├── requirements.txt
├── clean_data.py               # Data cleaning script
└── README.md
```

---

## 🎛️ Global Filters

All pages include consistent filters in the sidebar:

- **🌍 Continent** - Filter by continent (Europe, Asia, Africa, etc.)
- **🏳️ Country (NOC)** - Filter by specific countries
- **🏃 Sport** - Filter by sport/discipline
- **🏅 Medal Type** - Checkboxes for Gold, Silver, Bronze

---

## 📊 Data Sources

Data from the Paris 2024 Olympic Games:
- [Kaggle: Paris 2024 Olympic Games Dataset](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games)

| File | Description |
|------|-------------|
| athletes.csv | 11,113 athletes |
| medals_total.csv | 92 countries with medals |
| medals.csv | 1,044 medal events |
| medallists.csv | 2,315 individual medallists |
| events.csv | 329 events |
| nocs.csv | 224 National Olympic Committees |
| venues.csv | 35 Olympic venues |

---

## 🛠️ Technologies

- **Streamlit** - Web framework
- **Pandas** - Data processing
- **Plotly Express** - Interactive visualizations
- **Python 3.8+**

---

## 👥 Team

Built for the LA28 Volunteer Selection Challenge - Paris 2024 Olympic Games Streamlit Dashboard Competition.

---

## 📝 License

This project is for educational purposes as part of the Software Engineering for Data Science module.

---

**🏅 From Paris 2024 to Los Angeles 2028 - Celebrating athletic excellence!**
