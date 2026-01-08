# Blog Templating Project (Flask & Jinja)

A dynamic blog website built using Python and Flask. This project fetches blog post data from an external JSON API and renders it using Jinja2 templates. It features a home page listing all posts and dynamic routing for individual article pages.


## 🚀 Features

* **API Integration:** Fetches blog data dynamically using the `requests` library from an npoint.io JSON endpoint.
* **Object-Oriented Design:** Uses a `Post` class (defined in `post.py`) to structure the blog data.
* **Dynamic Routing:**
    * `/`: Renders the home page with a loop of all blog posts.
    * `/post/<int:index>`: dynamically renders a specific blog post based on its ID.
* **Jinja Templating:** Utilizes Jinja2 for control flow (loops/conditionals) inside HTML files.

## 🛠️ Built With

* [Python 3.x](https://www.python.org/)
* [Flask](https://flask.palletsprojects.com/) - Web Framework
* [Requests](https://pypi.org/project/requests/) - HTTP Library
* [Jinja2](https://jinja.palletsprojects.com/) - Templating Engine

## 💻 Installation & Usage

1.  **Clone the repository:**
    git clone https://github.com/yourusername/blog-templating.git
    cd blog-templating

2.  **Install the required dependencies:**
    pip install flask requests

3.  **Run the Application:**
    python main.py

4.  **View the Website:**
    Open your web browser and go to: http://127.0.0.1:5000/

## 📝 Code Overview

### `main.py`
The entry point of the application. It:
1.  Fetches JSON data from the API.
2.  Instantiates `Post` objects for each entry.
3.  Defines Flask routes (`/` and `/post/<index>`) to handle navigation.

### `post.py`
Contains the `Post` class, which initializes with:
* `post_id`
* `title`
* `subtitle`
* `body`

## Author
* Param Sangani
