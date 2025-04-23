
# 🌱 Environmental Impact Calculator (MERN + Android)

A full-stack web and mobile application that helps users calculate their carbon footprint based on daily activities such as electricity usage, transportation, diet, and plastic consumption.

---

## 📌 Project Goal

To educate and motivate users to adopt more eco-conscious habits by calculating their environmental impact and offering personalized tips for improvement.

---

## ✅ Minimum Viable Product (MVP)

### Core Features
- 🌿 User inputs:
  - Electricity usage (kWh)
  - Transportation (car, bike, public transport, flights)
  - Diet type (meat-based or vegetarian/vegan)
  - Plastic usage
- 🧮 Carbon footprint calculation based on input
- 📊 Display results using charts (Chart.js)
- 🌟 Tips and suggestions to reduce emissions
- 💾 Optional: User login and data saving

---

## 🧱 Tech Stack

| Part         | Technology                       |
|--------------|-----------------------------------|
| Frontend     | React.js, Bootstrap, Chart.js     |
| Backend      | Express.js, Node.js               |
| Database     | MongoDB + Mongoose                |
| API Requests | Axios                             |
| Mobile App   | Capacitor.js (wraps React app)    |
| Charts       | Chart.js                          |
| Auth (opt.)  | JWT, bcrypt                       |
| Hosting      | Netlify / Render / Vercel         |
| Mobile Build | Android Studio (via Capacitor)    |

---

## 📂 Project Structure

```
environment-impact-calculator/
├── client/              # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.js
│   │   └── index.js
├── server/              # Express backend
│   ├── routes/
│   ├── models/
│   ├── controllers/
│   └── server.js
├── README.md
└── package.json
```

---

## 🧮 Sample Emission Factors

| Activity               | Emission Factor                  |
|------------------------|----------------------------------|
| Electricity            | 1 kWh ≈ 0.92 lbs CO₂             |
| Car travel             | 1 km ≈ 0.21 kg CO₂               |
| Short flight (<3 hrs)  | ≈ 250 kg CO₂ per flight          |
| Beef meal              | ≈ 5.0 kg CO₂ per serving         |
| Plastic bottle         | ≈ 0.08 kg CO₂ per bottle         |

*(You can update values as per region or API)*

---

## 🛠️ Development Steps

### Phase 1: Backend (Express + MongoDB)
- Setup API endpoints
- Connect MongoDB (with Mongoose)
- Add emissions calculation route
- Setup CORS for frontend connection

### Phase 2: Frontend (React.js)
- Build form UI to collect data
- Connect with backend using Axios
- Display result with Chart.js
- Add basic routing (React Router)

### Phase 3: Android Build (Capacitor)
1. From `client/` folder:
   ```bash
   npm run build
   npm install @capacitor/core @capacitor/cli
   npx cap init
   npx cap add android
   npx cap copy
   npx cap open android
   ```
2. Run and test in Android Studio
3. Build APK for deployment

---

## 🔐 Optional: Add Authentication
- JWT-based login/register
- bcrypt for password hashing
- Save user emissions history in MongoDB

---

## 🔮 Future Ideas
- Daily eco-friendly tips
- Share footprint on social media
- Push notifications (Capacitor plugin)
- Global leaderboards
- Admin dashboard for data analysis

---

## 🔗 Useful Resources
- [Capacitor.js Docs](https://capacitorjs.com/docs)
- [MongoDB Docs](https://www.mongodb.com/docs/)
- [React.js Docs](https://reactjs.org/docs/getting-started.html)
- [Chart.js Docs](https://www.chartjs.org/docs/)
- [Node.js + Express Guide](https://expressjs.com/)

---

## 🚀 Deployment Notes
- Deploy frontend: Netlify / Vercel (from `/client`)
- Deploy backend: Render / Railway / Cyclic
- Mobile app build: Android Studio using Capacitor

---

## 👤 Author Notes
- Remember to test responsiveness and mobile build early
- Keep emission factors updated or API-driven
- Push regularly to GitHub and document progress
