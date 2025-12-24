# AI-Agent TrajectoryAnalyzer

<p align="justify">
A modular, GROMACS-centric molecular dynamics (MD) trajectory analysis framework with an optional AI-assisted interface for structured task specification. This project provides a web-based UI for common MD trajectory analyses, backed by deterministic GROMACS execution modules. An optional AI agent converts natural-language requests into structured JSON tasks without directly executing simulations.
</p>

You can use this tool for free by clicking <a href="https://cadd.sean28299.dpdns.org/static/Probe-GridMap-Builder_package.zip">here</a>. 👉 [Live Demo](http://traj.sean28299.dpdns.org)

---

## ✨ Key Features

- Web-based MD trajectory analysis (Flask)
- Modular GROMACS backend (`gmx_*.py`)
- Expert-controlled atom selection (index groups + `gmx select`)
- Optional AI-assisted task specification (JSON-based)
- Fully deterministic and reproducible execution
- Pre-packaged Conda environments (Linux & macOS)
- No manual GROMACS compilation required

---

## 📁 Repository Structure

```
TrajectoryAnalyzer/
├── app-traj-analysis.py
├── gmx_ai.py
├── gmx_rms.py
├── gmx_rmsf.py
├── gmx_gyrate.py
├── gmx_sasa.py
├── gmx_cluster.py
├── gmx_pca.py
├── gmx_distance.py
├── gmx_contact.py
├── gmx_hbond.py
├── templates/
│   ├── traj_analysis_ui.html
│   ├── ai_ui.html
│   ├── pca_ui_compact.html
│   ├── hbond_ui.html
│   ├── distance_ui.html
│   └── custom_selection_guide.html
├── env/
│   ├── LINUX_gromacs_env.tar.gz
│   └── MAC_gromacs_env.tar.gz
├── traj_package.zip
└── README.md
```

## 🖥 System Requirements
Linux or macOS

## 📦 Installation & Activate the Environment
### Linux
```
tar -xzf LINUX_gromacs_env.tar.gz
source LINUX_gromacs_env/bin/activate
```
### MacOS
```
tar -xzf MAC_gromacs_env.tar.gz
source MAC_gromacs_env/bin/activate
```

## 🚀 Launching the Web Interface
```
unzip traj_package.zip
cd traj_package/
python app-traj-analysis.py
The interface will be available at: http://localhost:8082
```






