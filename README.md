
# 📄 PDFGen (JSON → PDF using pdfcpu)

A simple and powerful project to generate PDF files from JSON data using **pdfcpu**.
Designed for Debian users and developers who want full control over PDF creation.

---

## 🚀 Features

* Convert JSON → PDF easily
* Works with `pdfcpu` (lightweight, fast)
* Clean structure for customization
* Ready-to-use examples
* Debian-friendly setup

---

## 📦 Requirements

* Debian / Ubuntu
* Go (for pdfcpu)
* pdfcpu installed

---

## ⚙️ Installation

### 1. Install Go

```bash
sudo apt update
sudo apt install golang -y
```

### 2. Install pdfcpu

```bash
go install github.com/pdfcpu/pdfcpu/cmd/pdfcpu@latest
```

Add to PATH:

```bash
export PATH=$PATH:$(go env GOPATH)/bin
```

Verify:

```bash
pdfcpu version
```

---

## 📁 Project Structure

```
PDFGen/
├── examples
│   └── basic_01
├── README.md
├── scripts
└── templates
```

---


## ▶️ Generate PDF

```bash
pdfcpu create content.json output.pdf
```

---

## ⚠️ Common Errors

### ❌ `invalid font size: 0`

✔ Fix: Ensure `"size"` is not `0`

```json
"size": 12
```

---

## 🧪 Example Commands

```bash
# Create PDF
pdfcpu create content.json out.pdf

# Validate PDF
pdfcpu validate out.pdf

# Inspect PDF
pdfcpu info out.pdf
```

---

## 📚 Advanced Ideas

* Add tables using JSON layout
* Create invoices / bills
* Multi-page reports
* Tamil + English text support (Unicode fonts)
* Dynamic PDF from scripts (Python/C++)

---

## 💡 Future Improvements

* GUI tool for JSON editing
* Template engine
* Auto layout system
* REST API for PDF generation
* Docker support

---

## 🤝 Contributing

Pull requests are welcome.
Feel free to add new templates, fixes, or examples.

---

## 📜 License

MIT License

---

## ⭐ Goal

Build a **simple, powerful JSON → PDF engine** for developers.

---

