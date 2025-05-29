# Campus-Navigate-3D — Frontend (React)

[![Project Status](https://img.shields.io/badge/Status-In_Development-yellow)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Українська](https://img.shields.io/badge/Мова-Українська-brightgreen)](README.md)

[![Fullstack](https://img.shields.io/badge/Integration-Fullstack-blueviolet)]()
[![React](https://img.shields.io/badge/React-19.1-%2361DAFB?logo=react)](https://react.dev/)
[![Three.js](https://img.shields.io/badge/Three.js-0.176-%23000000?logo=three.js)](https://threejs.org/)
[![Vite](https://img.shields.io/badge/Vite-6.3.5-%23646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)

Веб-додаток для візуалізації та навігації 3D-моделлю університету з двома режимами: **автоматичний обліт** обраних точок і **вільний політ**. Інформація про локації підвантажується динамічно через API.

---

## ✨ Основні можливості
- **Режими переміщення**:
    - 🛩 Автоматичний обліт обраних локацій (кнопкова навігація).
    - 🕹 Вільний рух камери (з обмеженнями меж моделі).
- **Інформаційна панель**: Деталі про локацію зліва під час обльоту.
- **Адмін-панель**: Додавання/редагування точок через Django.
- **Оптимізація**: Плавна робота з великою 3D-моделлю.

---

## 🤝 Взаємодія з бекендом
Цей фронтенд працює виключно з [бекенд-додатком на Django](https://github.com/Zebaro24/Campus-Navigate-3D-BE).
Ключові залежності:
- Адмінка бекенду використовується для оновлення точок навігації
- 3D-модель завантажується безпосередньо з бекенду

---

## 🛠 Технології
- **React 19** (хуки, функціональні компоненти)
- **Three.js**
- **Vite** (збірка)
- **Axios** (HTTP-запити до API)
- **TWEEN.js** (анімації перельоту)
- **CSS Modules** (стилізація)

---

## 🚀 Установка та запуск

1. **Клонування репозиторію**
   ```bash
   git clone https://github.com/Zebaro24/Campus-Navigate-3D-FE.git frontend
   cd frontend
   ```

2. **Встановлення залежностей**
   ```bash
   npm install
   # або
   yarn install
   ```

3. **Налаштування змінних середовища**  
   Створіть файл `.env` в корені проекту:
   ```
   VITE_API_BASE_URL=http://localhost:8000/api
   VITE_MODEL_URL=http://localhost:8000/api/active-model-file
   ```

4. **Запуск сервера розробки**
   ```bash
   npm run dev
   # або
   yarn dev
   ```
   Додаток буде доступний за адресою [http://localhost:5173](http://localhost:5173)

---

## 🎮 Керування у режимі вільного польоту
- **ЛКМ + перетягування**: Обертання камери
- **ПКМ + перетягування**: Переміщення сцени
- **Коліщатко миші**: Зум
- **WASD**: Переміщення у просторі
- **Q/E**: Підйом/опускання

---

## 📧 Контакти
- **Автор**: Денис Щербатий
- **Пошта**: zebaro.work@gmail.com

