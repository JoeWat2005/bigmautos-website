# BigM Autos Website

A Django-powered website for **BigM Autos**, featuring a modern frontend built with **Tailwind CSS** using `django-tailwind`.

---

## 🛠 Tech Stack

- **Backend:** Django  
- **Frontend:** Tailwind CSS (via `django-tailwind`)  
- **Database:** SQLite (development)  
- **Node:** npm (for Tailwind build pipeline)

---

## 📁 Project Structure

```
website-code/
├── .gitignore
├── website/
│   ├── manage.py
│   ├── main/              # Main Django app
│   ├── theme/             # Tailwind / frontend app
│   ├── website/           # Django project settings
```

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/JoeWat2005/bigmautos-website.git
cd bigmautos-website
```

---

### 2️⃣ Create and activate a virtual environment

```bash
python -m venv env
```

**Windows:**
```bash
env\Scripts\activate
```

**macOS / Linux:**
```bash
source env/bin/activate
```

---

### 3️⃣ Install Python dependencies

```bash
pip install -r requirements.txt
```

> If `requirements.txt` is not present yet:
```bash
pip install django django-tailwind
```

---

### 4️⃣ Install Node dependencies (Tailwind)

```bash
cd website/theme/static_src
npm install
```

---

## 🎨 Running Tailwind (Development)

From the project root:

```bash
python manage.py tailwind start
```

This watches your Tailwind files and rebuilds CSS automatically.

---

## 🧑‍💻 Running the Django Development Server

```bash
python manage.py runserver
```

Then open:
```
http://127.0.0.1:8000/
```

---

## 📦 Collecting Static Files (Production)

```bash
python manage.py collectstatic
```

---

## ⚠️ Notes

- Keep Tailwind running during frontend development
- Edit Tailwind source files, not compiled CSS
- Configured for development use

---

## 📄 License

Private project for BigM Autos.
