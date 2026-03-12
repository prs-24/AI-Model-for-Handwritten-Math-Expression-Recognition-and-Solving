<div align="center">

<!-- Animated Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=200&section=header&text=✍️%20AI%20Equation%20Solver&fontSize=50&fontColor=fff&animation=twinkling&fontAlignY=35&desc=Handwritten%20Math%20Recognition%20Powered%20by%20AI&descAlignY=55&descSize=18" width="100%"/>

<br/>

<!-- Badges Row 1 -->
![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Google Cloud Vision](https://img.shields.io/badge/Google%20Cloud%20Vision-API-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-UI-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)
![SymPy](https://img.shields.io/badge/SymPy-Math%20Engine-3B5526?style=for-the-badge&logo=python&logoColor=white)

<br/>

<!-- Badges Row 2 -->
![OpenCV](https://img.shields.io/badge/OpenCV-Image%20Processing-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-blueviolet?style=for-the-badge)

<br/><br/>

> **Upload a photo of any handwritten math equation — and watch AI recognize and solve it in real time.**

<br/>

[🚀 Try Demo](#-demo) · [📖 Docs](#-how-it-works) · [🛠️ Setup](#%EF%B8%8F-installation) · [🤝 Contribute](#-contributors)

</div>

---

## 📸 Demo

<div align="center">
<table>
<tr>
<td align="center"><b>📥 Upload Equation</b></td>
<td align="center"><b>🔍 Processed Image</b></td>
<td align="center"><b>🧮 Solution Output</b></td>
</tr>
<tr>
<td align="center">
<img src="https://placehold.co/250x150/1a1a2e/ffffff?text=Handwritten+Image" alt="Input" width="250"/>
</td>
<td align="center">
<img src="https://placehold.co/250x150/16213e/ffffff?text=Binary+Threshold" alt="Processed" width="250"/>
</td>
<td align="center">
<img src="https://placehold.co/250x150/0f3460/ffffff?text=x+%3D+5" alt="Solution" width="250"/>
</td>
</tr>
</table>
</div>

---

## ✨ Features

<div align="center">

| Feature | Description |
|:---:|:---|
| 📝 **OCR Recognition** | Extracts handwritten equations using **Google Cloud Vision API** |
| 🧮 **Smart Solver** | Solves algebraic equations symbolically with **SymPy** |
| 🔍 **Image Enhancement** | Preprocesses images with **OpenCV** for cleaner OCR results |
| 🖥️ **Interactive UI** | Browser-based drag-and-drop interface via **Gradio** |
| ⚡ **Real-time Results** | Instant output with original + processed image comparison |
| 🌐 **Shareable Link** | Auto-generates a public link to share with others |

</div>

---

## 🧠 How It Works

```
📷 Upload Image
      │
      ▼
┌─────────────────────────┐
│  OpenCV Preprocessing   │  ← Grayscale + Binary Threshold
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│  Google Vision API OCR  │  ← Detects & extracts text
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│    Text Sanitization    │  ← Regex cleanup, symbol parsing
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│    SymPy Math Engine    │  ← Symbolic equation solving
└────────────┬────────────┘
             │
             ▼
       ✅ Solution + Images displayed in Gradio UI
```

---

## 🛠️ Installation

### Prerequisites

- Python 3.8 or higher
- A **Google Cloud Vision API** service account JSON key

### Step 1 — Clone the repo

```bash
git clone https://github.com/YOUR_USERNAME/handwritten-equation-solver.git
cd handwritten-equation-solver
```

### Step 2 — Install dependencies

```bash
pip install google-cloud-vision sympy opencv-python-headless matplotlib gradio numpy pillow
```

### Step 3 — Add your API credentials

Place your Google Cloud Vision credentials JSON file in the project root and update the path in the script:

```python
API_JSON_PATH = "/path/to/your-credentials.json"
```

### Step 4 — Run the app

```bash
python app.py
```

Your app will launch at `http://localhost:7860` — and a shareable public URL will be printed in the terminal!

---

## 📂 Project Structure

```
📦 handwritten-equation-solver
 ┣ 📜 app.py                  # Main application file
 ┣ 📜 requirements.txt        # Python dependencies
 ┣ 📁 assets/                 # Sample equation images
 ┗ 📜 README.md               # You're reading this!
```

---

## 💡 Usage Tips

> 🖊️ **Best results with:**
> - Clear, dark ink on white paper
> - Simple algebraic equations (e.g. `2x + 5 = 11`)
> - Well-spaced characters
> - Good lighting / scanned images

> ⚠️ **Known Limitations:**
> - Complex multi-line expressions may not parse correctly
> - Handwriting with ambiguous symbols (e.g. `0` vs `O`) may be misread
> - Currently supports single-variable equations

---

## 🧪 Example Equations

| Input (Handwritten) | Recognized | Solved |
|:---:|:---:|:---:|
| `2x + 5 = 11` | `2*x+5=11` | `x = 3` |
| `x^2 - 4 = 0` | `x**2-4=0` | `x = [-2, 2]` |
| `3y - 9 = 0` | `3*y-9=0` | `y = 3` |

---

## 👥 Contributors

<div align="center">

### 🌟 Meet the Team

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/apurvafx">
        <img src="https://github.com/apurvafx.png" width="100px;" style="border-radius:50%" alt="apurvafx"/>
        <br />
        <sub><b>apurvafx</b></sub>
      </a>
      <br/>
      <a href="https://github.com/apurvafx">
        <img src="https://img.shields.io/badge/GitHub-apurvafx-181717?style=flat-square&logo=github"/>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/prs-24">
        <img src="https://github.com/prs-24.png" width="100px;" style="border-radius:50%" alt="prs-24"/>
        <br />
        <sub><b>prs-24</b></sub>
      </a>
      <br/>
      <a href="https://github.com/prs-24">
        <img src="https://img.shields.io/badge/GitHub-prs--24-181717?style=flat-square&logo=github"/>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/saketsumanai">
        <img src="https://github.com/saketsumanai.png" width="100px;" style="border-radius:50%" alt="saketsumanai"/>
        <br />
        <sub><b>saketsumanai</b></sub>
      </a>
      <br/>
      <a href="https://github.com/saketsumanai">
        <img src="https://img.shields.io/badge/GitHub-saketsumanai-181717?style=flat-square&logo=github"/>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Aashish-Chandr">
        <img src="https://github.com/Aashish-Chandr.png" width="100px;" style="border-radius:50%" alt="Aashish-Chandrin"/>
        <br />
        <sub><b>Aashish-Chandr</b></sub>
      </a>
      <br/>
      <a href="https://github.com/Aashish-Chandr">
        <img src="https://img.shields.io/badge/GitHub-Aashish--Chandr-181717?style=flat-square&logo=github"/>
      </a>
    </td>
  </tr>
</table>

</div>

---

## 🤝 Contributing

We welcome contributions! Here's how to get started:

```bash
# 1. Fork the repo
# 2. Create your feature branch
git checkout -b feature/amazing-feature

# 3. Commit your changes
git commit -m "Add amazing feature"

# 4. Push to your branch
git push origin feature/amazing-feature

# 5. Open a Pull Request 🎉
```

Please make sure your code follows the existing style and includes relevant comments.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- [Google Cloud Vision API](https://cloud.google.com/vision) — for powerful OCR capabilities
- [SymPy](https://www.sympy.org/) — for symbolic mathematics
- [Gradio](https://gradio.app/) — for the beautiful and easy UI framework
- [OpenCV](https://opencv.org/) — for image preprocessing

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer" width="100%"/>

**Made with ❤️ by the team**

⭐ If you found this useful, please **star** this repository!

</div>
