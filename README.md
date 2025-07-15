<div align="center">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
    
</div>

![Project Banner](./imgs/banner.png)

<div align="center">

# 🎧 **Project Overview**

</div>

<div align="center">

This repository performs an exploratory data analysis on Spotify Brazil’s Top 50 tracks using Python and Jupyter Notebook. By leveraging the Spotify Web API, it extracts track and artist metadata to uncover insights into musical trends in Brazil.

</div>

<br/>

## 📋 **Prerequisites**

- **Python 3.7+**
- **pip**
- **Existing ****\`.env\`**** file** in the project root containing your Spotify API credentials.

<br/>

## 🔑 **Spotify API Credentials**

You already have a `.env` file—simply replace the placeholders with your actual keys:

```ini
client_id="YOUR_CLIENT_ID_HERE"
client_secret="YOUR_CLIENT_SECRET_HERE"
```

> **Note:** Do not include extra quotes or whitespace.

To obtain these values:

1. Go to the [**Spotify Developer Dashboard**](https://developer.spotify.com/dashboard) and log in.
2. Click **Create an App**.
3. Copy the **Client ID** and click **Show Client Secret**.

<br/>

## 🚀 **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/brunnox/spotify_top50_study.git
   ```
2. Navigate to the project folder:
   ```bash
   cd spotify_top50_study
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
<br/>

## 📂 **Directory Structure**


```
spotify_top50_study/
├── imgs/              # Images used in README and notebook
│   └── banner.png
├── .env               # Your Spotify client_id and client_secret
├── spotify.ipynb      # Jupyter Notebook with full analysis
└── requirements.txt   # File with necessary python libs to install
```

<br/>

## 📝 **Notebook Description** (`spotify.ipynb`)

1. **Banner Display**: shows `imgs/banner.png`.
2. **Environment Setup**: loads `.env` via `python-dotenv`.
3. **Authentication**: implements the Client Credentials flow to fetch an access token.
4. **Data Collection**: requests the “Top 50 Brazil” playlist endpoint.
5. **Data Transformation**: builds a `pandas.DataFrame` with attributes like name, popularity, duration, and explicit flag.
6. **Exploratory Analysis**: computes descriptive stats and visualizes with Plotly Express.
7. **Regression Modeling**: fits a `LinearRegression` model to explore feature correlations.

<br/>

## ▶️ **Running the Analysis**

```bash
jupyter notebook spotify.ipynb
```

Run cells in order to reproduce the full workflow.

<br/>

## ✉️ **Author**

Developed by **brunnox** – [GitHub/brunnox](https://github.com/brunnox)

[contributors-shield]: https://img.shields.io/github/contributors/brunnox/spotify_top50_study.svg?style=for-the-badge
[contributors-url]: https://github.com/brunnox/spotify_top50_study/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/brunnox/spotify_top50_study.svg?style=for-the-badge
[forks-url]: https://github.com/brunnox/spotify_top50_study/network/members
[stars-shield]: https://img.shields.io/github/stars/brunnox/spotify_top50_study.svg?style=for-the-badge
[stars-url]: https://github.com/brunnox/spotify_top50_study/stargazers
[issues-shield]: https://img.shields.io/github/issues/brunnox/spotify_top50_study.svg?style=for-the-badge
[issues-url]: https://github.com/brunnox/spotify_top50_study/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/brunnox