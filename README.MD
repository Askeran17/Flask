# 🏛️ Byzantine Empire — Flask Web Project

## 📖 Overview

This project is a historical web application built with Flask, dedicated to the legacy of the Byzantine Empire. It features profiles of emperors, thematic pages, and a structured layout using Bootstrap and Jinja2 templates. The site is designed to be informative, visually engaging, and easy to expand.

### Live Site

- Go to live site - [Byzantine Empire](https://flask-app-prj-26927cc0ca85.herokuapp.com/)

## 🚀 How to Run

1. **Install dependencies**:
   ```bash
   pip install flask
   ```

2. **Run the app**:
   ```bash
   python run.py
   ```

3. **Visit in browser**:
   ```
   http://localhost:5000
   ```

## 🌐 Routes and Pages

| Route              | Template       | Description                                                                 |
|-------------------|----------------|-----------------------------------------------------------------------------|
| `/`               | `index.html`   | Homepage with featured historical posts                                     |
| `/about`          | `about.html`   | Dynamic page showing Byzantine emperors from `company.json`                |
| `/about/<slug>`   | (optional)     | Individual emperor profile page (to be implemented)                         |
| `/legacy`         | `legacy.html`  | Overview of the cultural, legal, and religious legacy of Byzantium         |
| `/contact`        | `contact.html` | Contact form or information (can be customized)                             |

## 🧠 Data Source

- `company.json`: Contains structured data about Byzantine emperors:
  ```json
  {
    "name": "Justinian I",
    "description": "...",
    "image_source": "https://...",
    "url": "justinian-i"
  }
  ```

This data is used to dynamically render emperor profiles on the `/about` page.

## 🎨 Styling

- Based on [Start Bootstrap Clean Blog](https://startbootstrap.com/theme/clean-blog)
- Custom styles added in `style.css`
- Background images and layout controlled via `clean-blog.css`

## 📌 Features

- Responsive design with Bootstrap
- Dynamic content rendering with Jinja2
- Modular templates with `base.html`
- Historical content focused on Byzantine rulers
- Easy to expand with new pages or data

## 🛠️ Future Improvements

- Add individual emperor pages (`/about/<slug>`)
- Integrate search or filtering by century/dynasty
- Add interactive timeline or map
- Connect to a database for scalable content management
- Implement contact form with Flask-WTF

