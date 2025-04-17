# python-qa

A lightweight setup for clean code and signal visualization in Python using `pre-commit`, `streamlit`, and the ultra-fast package manager [`uv`](https://github.com/astral-sh/uv).

---

## 🛠️ Installation with `uv`

1. **Install uv**
```bash
curl -Ls https://astral.sh/uv/install.sh | sh
```

2. **Create a virtual environment**
```bash
uv venv
```

3. **Activate the environment**
```bash
source .venv/bin/activate
```

4. **Install dependencies**
```bash
uv pip install .[dev]
```

---

## 🚀 Running the Streamlit App

Assuming the file is located in `src/app.py`, you can run:

```bash
streamlit run src/app.py
```

---

## ✅ Pre-commit Setup

This project uses `pre-commit` to ensure code quality automatically on every commit.

1. **Install pre-commit hooks**
```bash
pre-commit install
```

2. **Run checks on all files (optional)**
```bash
pre-commit run --all-files
```

---

## 🔁 Committing Changes

When committing code, if any formatting or linting issues are detected, the commit will be blocked until they are fixed. To proceed:

```bash
git add .
git commit -m "fix: corrected linting issues"
```

---

## 🧪 Running this Project on GitHub Codespaces with `uv`

This project is fully compatible with GitHub Codespaces.

### 🔧 Setup Instructions

1. **Open the repository in GitHub Codespaces**  
   - Go to the repository on GitHub  
   - Click the green **Code** button > **Codespaces** tab > **Create codespace on `main`**

2. **Open a terminal in the Codespace**
   Use `Ctrl + \`` or go to `Terminal > New Terminal`.

3. **Install `uv`**
```bash
curl -Ls https://astral.sh/uv/install.sh | sh
```

4. **Create and activate virtual environment**
```bash
uv venv
source .venv/bin/activate
```

5. **Install project dependencies**
```bash
uv pip install .[dev]
```

6. **Run the app**
```bash
streamlit run src/app.py
```

> Make sure the app is inside the `src/` folder. Update the path if necessary.

---

## 📚 References

- [pre-commit](https://pre-commit.com/)
- [uv](https://github.com/astral-sh/uv)
- [streamlit](https://streamlit.io/)
- [wily (complexity tool)](https://towardsdatascience.com/simplify-your-python-code-automating-code-complexity-analysis-with-wily-5c1e90c9a485/)