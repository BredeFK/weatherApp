# 🖥️ Dashboard

A Kotlin-based Spring Boot dashboard application using various API's to be displayed through a front-end application

---

## 🔗 Useful Links

- **Base URL:** http://localhost:8080
- **Swagger UI:** http://localhost:8080/swagger-ui/index.html

---

## 📦 Tech Stack

- Kotlin 2.2.0
- Spring Boot 3.5.3
- Java 21

### API used

- YR / MET Weather API : https://api.met.no/weatherapi/locationforecast/2.0/documentation
- Nominatim API : https://nominatim.openstreetmap.org/ui/about.html
- Strava API : https://developers.strava.com/
- Discord Webhooks: https://discord.com/developers/docs/resources/webhook

---

## ▶️ Run Locally

### Prerequisites

- Java 21
- Maven 3.9+

### Build and Run

#### .env Example
```properties
STRAVA_CLIENT_ID=some-id
STRAVA_CLIENT_SECRET=some-secret
STRAVA_REFRESH_TOKEN=valid-unexpired-refresh-token
DISCORD_WEBHOOK_URL=some-webhook-utl
```

#### Terminal
```bash
mvn clean install
export $(cat .env | xargs)
mvn spring-boot:run
```