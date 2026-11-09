# FSAE Telemetry Sandbox 🏎️

A lightweight data pipeline designed to ingest real-time F1 sensor data via the OpenF1 API, process vehicle performance metrics, and implement threshold-based monitoring for overrev detection in Formula SAE applications.

---

## 🎯 Engineering Problem & Purpose

In motorsport engineering, telemetry data is crucial for assessing vehicle health and optimizing driver performance. Raw data from Engine Control Units (ECUs) often arrives as noisy, continuous streams that must be filtered and analyzed in real-time. 

This project simulates a trackside engineering environment by pulling real F1 data and executing automated **Data Logging** constraints to track critical thresholds:
* **Overrev Detection:** Automatically flags logs where the engine operates above safe RPM boundaries.
* **Driver Input Coordination (Planned):** Analyzing synchronized throttle and braking overlaps to identify driving inefficiencies.

---

## 🛠️ Tech Stack & Architecture

* **Language:** Python 3.10+
* **Data Manipulation:** Pandas (DataFrames)
* **Data Ingestion:** Requests (REST API Integration)
* **Data Source:** OpenF1 API (Live/Historical Vehicle Data)

### Data Workflow
`OpenF1 API (JSON)` ➡️ `Requests Ingestion` ➡️ `Pandas Transformation` ➡️ `Threshold Logic Analysis` ➡️ `Structured Log Output (TXT)`

---

## 📂 Repository Structure

```text
fsae-telemetry-sandbox/
├── dados/                    # Local temporary data storage (if applicable)
├── src/
│   ├── main.py               # Core data pipeline and analytical logic
│   └── relatorio_fsae.txt    # Generated trackside engineering report
├── .gitignore                # Production ignore rules
├── LICENSE                   # MIT License
├── README.md                 # Project Documentation
└── requirements.txt          # Python dependencies
```

---

## 🚀 Getting Started

Follow these instructions to set up and run the telemetry analyzer locally.

### 1. Prerequisites
Make sure you have Python installed, then clone the repository and install the dependencies:

```bash
pip install -r requirements.txt
```

### 2. Running the Analyzer
To fetch the telemetry data directly from the OpenF1 API and generate the engineering report, run:

```bash
python src/main.py
```

After execution, look for the generated trackside insights inside `src/relatorio_fsae.txt`.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🧑‍💻 Developed By Maria Júlia Lazarini Oleto 
Linkedin: https://www.linkedin.com/in/maria-j%C3%BAlia-lazarini-oleto-a29106356/
* **[Your Name]** - Software Engineering Student
* Connect with me on [LinkedIn]([Your LinkedIn URL Here])
