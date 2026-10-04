# ClassMark 🎓

**AI-powered attendance system for modern classrooms**

Mark attendance from classroom photos or a voice recording, in seconds.

- 🌐 **Website:** [cm-landing-page-iota.vercel.app](https://cm-landing-page-iota.vercel.app/) – project overview and features
- 🚀 **Live App:** [classmark-main.streamlit.app](https://classmark-main.streamlit.app/) – try the actual attendance app
- 💻 **App Source Code:** [github.com/AnishaSinha01/classmark](https://github.com/AnishaSinha01/classmark) – Streamlit app's code

| Landing Page | Streamlit App |
| --- | --- |
| ![Landing Page screenshot](static/img/demo/app-preview.png) | ![Streamlit App screenshot](static/img/demo/snap-landing.png) |

## 📖 About

ClassMark replaces manual roll-calls with face and voice recognition. This repo contains the responsive landing page. The Streamlit app is in a separate repository (linked above).

## ⚙️ How It Works

**Teacher:** register / log in → create a subject → share the join link or QR code → take attendance (photos or voice) → review and confirm → view records

**Student:** register once with Face ID (voice is optional) → join a subject with its code, link or QR → log in with Face ID and view your attendance count per subject

## ✨ Features

- 📸 **Face ID:** recognizes students from classroom photos
- 🎙️ **Voice ID:** identifies students from a single classroom recording
- 📱 **QR enrollment:** students join a subject by scanning a QR code or using a join link
- 📊 **Records:** attendance shown in a table, with CSV download

## 🛠️ Tech Stack

| Layer | Tools |
| --- | --- |
| Landing page | Flask, HTML, CSS, JavaScript |
| App | Streamlit, Pandas, Segno (QR) |
| Face recognition | Dlib, scikit-learn |
| Voice recognition | Resemblyzer, Librosa |
| Auth | bcrypt |
| Database | Supabase (PostgreSQL) |

## 🚀 Run Locally (Landing Page)

```bash
git clone https://github.com/AnishaSinha01/cm-landing-page
cd cm-landing-page
pip install flask
python app.py
```


## 📁 Structure

```
├── app.py
├── requirements.txt
├── vercel.json
├── templates/index.html
└── static/
    ├── css/style.css
    ├── js/script.js
    └── img/
```
