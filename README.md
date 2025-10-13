[PYTHON_BADGE]:https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[PANDAS_BADGE]:https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white
[NUMPY_BADGE]:https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white
[PRS_BADGE]:https://img.shields.io/badge/PRs-welcome-green?style=for-the-badge

<h1 align="center" style="font-weight: bold;">Automated Product Registration with PyAutoGUI 🖱️</h1>

![python][PYTHON_BADGE]
![pandas][PANDAS_BADGE]
![numpy][NUMPY_BADGE]
![prs][PRS_BADGE]

<details open="open">
<summary>Table of Contents</summary>
  
- [🚀 Getting started](#started)
  - [Prerequisites](#prerequisites)
  - [Cloning](#cloning)
  - [Environment Setup](#environment)
  - [Starting](#starting)
- [📍 How It Works](#how-it-works)
- [📁 CSV Structure](#csv)
- [🧰 Files Overview](#files)
- [🤝 How to Reach Me](#reach)
- [📌 Obs](#obs)
  
</details>

<p align="center">
  <b>A Python automation project using PyAutoGUI to log in and register products on a web system automatically.</b>
</p>

---

<h2 id="started">🚀 Getting started</h2>

<h3 id="prerequisites">Prerequisites</h3>

- [Python 3.10+](https://www.python.org/downloads/)
- [pip](https://pip.pypa.io/en/stable/installation/)
- [Google Chrome browser](https://www.google.com/chrome/)

<h3 id="cloning">Cloning</h3>

```bash
git clone https://github.com/monosodrac/registration_automation.git
```

<h3 id="environment">Environment Setup</h3>

Install dependencies:

```bash
pip install pyautogui pandas numpy openpyxl
```

<h3 id="starting">Starting</h3>

1. Run the system login automation:
```bash
python codigo.py
```

2. If you need to check screen coordinates for mouse clicks, run:
```bash
python Auxiliar.py
```
⚠️ Before starting, make sure your screen resolution and browser are correctly configured, as the automation depends on cursor positions.

<h2 id="how-it-works">📍 How It Works</h2>

This automation performs the following steps:
1. Opens Google Chrome.
2. Accesses the login page: https://dlp.hashtagtreinamentos.com/python/intensivao/login
3. Fills in the email and password fields.
4. Imports a CSV file (produtos.csv) containing the list of products.
5. Iterates through each product and automatically fills in the form fields:
    - Código
    - Marca
    - Tipo
    - Categoria
    - Preço unitário
    - Custo
    - Observação (optional)
6. Submits each product registration.

<h2 id="csv">📁 CSV Structure</h2>

The file produtos.csv must follow this structure:
| codigo     | marca    | tipo    | categoria | preco_unitario | custo | obs |
| ---------- | -------- | ------- | --------- | -------------- | ----- | --- |
| MOLO000251 | Logitech | Mouse   | 1         | 25.95          | 6.5   |     |
| CAHA000251 | Hashtag  | Camisa  | 1         | 25.00          | 11.0  |     |
| CEMO000271 | Motorola | Celular | 1         | 279.00         | 72.5  |     |

📄 The automation reads each line from the CSV and registers all products on the platform.

<h2 id="files">🧰 Files Overview</h2>

| File           | Description                                                                                   |
| -------------- | --------------------------------------------------------------------------------------------- |
| `codigo.py`    | Main automation script responsible for logging in, reading the CSV, and registering products. |
| `Auxiliar.py`  | Helper script for identifying mouse coordinates on screen.                                    |
| `produtos.csv` | Example database containing products to be registered automatically.                          |

<h2 id="reach">🤝 How to reach me</h2>

<table>
  <tr>
    <td align="center">
      <a href="https://linktr.ee/monosodrac">
        <img src="https://avatars.githubusercontent.com/u/141099551?v=4" width="100px;" alt="Mono Cardoso Profile Picture"/><br>
        <sub>
          <b>Mono</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

<h2 id="contribute">📫 Contribute</h2>

Contributions are welcome! 🧩  
If you’d like to help improve this automation or add new features, follow the steps below:

1. Clone the repository  
```bash
git clone https://github.com/monosodrac/registration_automation.git
```
2. Create a new branch for your feature or fix 
```bash
git checkout -b feature/your-feature-name
```
3. Follow good commit message practices
4. After implementing your change, open a Pull Request describing:
   - The problem solved or the feature added
   - Steps to test the modification
   - (If applicable) screenshots or short videos showing the automation working
Once your PR is submitted, wait for code review and feedback! 🚀

<h3>Documentations that might help</h3>

[📝 How to create a Pull Request](https://www.atlassian.com/br/git/tutorials/making-a-pull-request)

[💾 Commit pattern](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)
