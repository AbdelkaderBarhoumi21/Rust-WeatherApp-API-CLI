# 🌦️ Weather Station CLI

Une petite application en **Rust** qui permet de consulter la météo d'une ville donnée via l’API [OpenWeatherMap](https://openweathermap.org/api).  
L’application fonctionne directement en **ligne de commande** et affiche les résultats avec des **couleurs** et des **émojis** pour une meilleure lisibilité.

---

## 🚀 Fonctionnalités

- 🔎 Recherche météo par **nom de ville** et **code pays** (ex: `Paris, FR` ou `New York, US`).  
- 🌡️ Affiche :
  - la description du temps,
  - la température (°C),
  - l’humidité (%),
  - la pression (hPa),
  - la vitesse du vent (m/s).  
- 🎨 Résultats colorés grâce à la crate [`colored`](https://crates.io/crates/colored).  
- 😀 Ajout d’**émojis météo** selon la température :
  - ❄️ (froid < 0°C)  
  - ☁️ (frais 0–10°C)  
  - ⛅ (doux 10–20°C)  
  - 🌤️ (agréable 20–30°C)  
  - 🔥 (chaleur > 30°C)  
- 🔁 Possibilité de refaire une recherche en boucle tant que l’utilisateur répond "yes".  

---

## 🛠️ Technologies utilisées

- [Rust](https://www.rust-lang.org/)  
- [reqwest](https://crates.io/crates/reqwest) → pour effectuer les requêtes HTTP.  
- [serde](https://crates.io/crates/serde) & [serde_json](https://crates.io/crates/serde_json) → pour **désérialiser** les réponses JSON en structures Rust.  
- [colored](https://crates.io/crates/colored) → pour coloriser le texte en terminal.  

---

## 📦 Installation & utilisation

### 1. Cloner le projet
```bash
git clone https://github.com/ton-profil/weather-station-cli.git
cd weather-station-cli
