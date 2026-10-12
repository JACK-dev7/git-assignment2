# DataGrokr Git Assignment Part II

**Name:** <your-name>

---

## 1. Writing a Good README

README for the `country-capital-api` repository:

````markdown
# Country Capital API

## What is this?

This is a simple API built with Python and Flask. You give it the name of a capital city and it returns the name of the country.

The API is served using Uvicorn, an ASGI server.

A hosted version is available at: https://example.com/country-capital/

## Prerequisites

Make sure you have these installed:

- Python
- pip
- Git

## Local Setup

1. Clone the repository:

   ```
   git clone <repository-url>
   cd country-capital-api
   ```

2. Create a virtual environment:

   ```
   python -m venv venv
   ```

3. Activate the virtual environment:

   On Windows:
   ```
   venv\Scripts\activate
   ```

   On Linux/macOS:
   ```
   source venv/bin/activate
   ```

4. Install the dependencies:

   ```
   pip install -r requirements.txt
   ```

5. Start the server:

   ```
   uvicorn app:app --reload
   ```

   If your main file or Flask app variable has a different name, replace `app:app` with `<file_name>:<variable_name>`.
````

---

## 2. Using .gitignore to Keep the Repository Clean

```gitignore
# Build directory at the root of the repository
/build/

# All files ending with .env
*.env

# All files in test-runs/logs
test-runs/logs/

# All CSV files anywhere in the repository
*.csv
```

---

## 3. Raising Clean Pull Requests

```
PR Title: feat/FEAPP-420: Allow customer notification via WhatsApp

PR Description:

WHAT:
Adds an optional WhatsApp number field to the customer notification
settings. If a customer enters a number, product update notifications
are sent to both their email and their WhatsApp number. If the field is
left empty, notifications go out by email only, as before.

WHY:
Customers have been requesting the ability to get product update
notifications on WhatsApp in addition to email. This covers the
requirement in FEAPP-420.

Notes:
No changes to the local development setup or build process.

PR Reviewers: <teammate-1>, <teammate-2>, <team-lead>
```
