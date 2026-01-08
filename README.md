@'
# Rick & Morty Explorer 🛸

Web-приложение для поиска и просмотра информации о персонажах, эпизодах и локациях из мультсериала **Rick and Morty**.  
Проект реализован с разделением **frontend / backend**, где все внешние API вызываются **только с серверной части**, согласно требованиям задания.

---

## 🔗 Live Demo

- **Frontend (Vercel):**  
  https://rick-morty-app-alpha-ecru.vercel.app

- **Backend (Render):**  
  https://rick-morty-app-z3ub.onrender.com

---

## ✨ Возможности

-  Поиск персонажей по имени
-  Пагинация с URL-state (`?name=rick&page=2`)
-  Детальная информация о персонажах
-  Просмотр эпизодов и локаций
-  Добавление персонажей в Favorites (localStorage)
-  Trending персонажи
-  Светлая / тёмная тема
-  Быстрый UI на Vite + React
-  Все внешние API вызываются **через backend-прокси**

---

##  Архитектура

rick-morty-app/
├── client/ # Frontend (Vite + React)
│ ├── src/
│ └── vercel.json
├── server/ # Backend (Node.js + Express)
│ └── index.js
└── README.md


---

##  Технический стек

### Frontend
- React
- Vite
- React Router
- CSS
- localStorage

### Backend
- Node.js
- Express
- node-fetch
- dotenv
- cors

### Deployment
- Vercel — frontend
- Render — backend

---

- **React + Vite** — высокая производительность и быстрый DX
- **Express** — простой и надёжный backend для прокси-логики
- **Разделение frontend/backend** — best practices и требование ТЗ
- **Vercel + Render** — быстрый и бесплатный деплой

---

## Установка и запуск локально

### Backend
```bash
cd server
npm install
npm run dev

http://localhost:5000/health

### Frontend
```bash
cd client
npm install
npm run dev

### Создай .env
VITE_API_BASE_URL=http://localhost:5000

##Frontend не обращается напрямую к rickandmortyapi.com.
##Все запросы идут через backend:

/api/characters
/api/characters/:id
/api/episodes
/api/locations

##GitHub: https://github.com/Nurislam841

##'@ | Out-File -Encoding UTF8 README.md
