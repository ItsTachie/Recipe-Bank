# Recipe Bank

A personal collection of recipes documented in Markdown and deployed as a static website. This project serves as a digital cookbook, organized to handle everything from daily staples (Sadza, Rice, Pasta) to global cuisines (Middle Eastern, European, Chinese).

[View the site](https://itstachie.github.io/Recipe-Bank/)

## Tech Stack

* **Authoring:** Obsidian
* **Static Site Generator:** MkDocs
* **Theme:** ReadTheDocs
* **Hosting:** GitHub Pages

## Project Structure

The repository is structured to cleanly separate site configuration from the Markdown content. The `docs/` directory acts as the Obsidian vault.

```text
recipe-book/
├── mkdocs.yml              # Site configuration and navigation tree
└── docs/                   # Markdown content (Obsidian Vault)
    ├── index.md            # Homepage
    ├── staples/            # Sadza, rice, pasta, and potatoes
    ├── stews/              # Curries and stews
    ├── global/             # Regional cuisines (Chinese, Middle Eastern, etc.)
    ├── stylesheets/        # custom css styling 

```

## Local Setup

To run this project locally, you will need Python installed on your machine.

1. **Clone the repository:**

```bash
git clone https://github.com/ItsTachie/Recipe-Bank
cd recipe-bank

```

1. **Create and activate a virtual environment:**

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

```

1. **Install dependencies:**

```bash
pip install -r requirements.txt

```

1. **Run the development server:**

```bash
mkdocs serve

```

The site will be available at `http://127.0.0.1:8000`. The server will automatically rebuild the site and refresh your browser whenever you save a Markdown file.

## Workflow: Adding a Recipe

1. Open the `docs/` directory as a Vault in Obsidian.
2. Navigate to the appropriate category folder.
3. Create a new note and apply the Obsidian `Recipe Template`.
4. Write the recipe using standard Markdown syntax.
5. Add the file path to the `nav` section in `mkdocs.yml` so it appears in the sidebar.
6. Commit and push the changes to the repository.

## Deployment

This site is hosted on GitHub Pages. To build the static HTML and deploy it manually, run the following command from the project root:

```bash
mkdocs gh-deploy

```

This command builds the site and automatically pushes the compiled HTML to the `gh-pages` branch.

---
