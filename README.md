## RESUME BUILDING 

````markdown
# LaTeX Compilation Guide for `main.tex` (Linux)

This project contains a LaTeX file called `main.tex`.  
This guide explains how to compile it on **Linux** using standard LaTeX tools and libraries.
`````

## **1. Install LaTeX**

### **For Debian/Ubuntu**

Minimal installation:

```bash
sudo apt install texlive-latex-base
````

Full installation (recommended):

```bash
sudo apt install texlive-full
```

### **For Fedora**

```bash
sudo dnf install texlive-scheme-full
```

---

## **2. Compile `main.tex`**

To compile `main.tex` and generate a PDF:

```bash
pdflatex main.tex
```

This will create:

* `main.pdf` – Your output PDF
* `main.aux` – Auxiliary file
* `main.log` – Compilation log

---

## **3. View the PDF**

Open the generated PDF:

```bash
xdg-open main.pdf
```

Or use:

```bash
evince main.pdf
# or
okular main.pdf
```

---

## **4. Clean Up (Optional)**

Remove extra files generated during compilation:

```bash
rm main.aux main.log
```

---

## **5. Optional: Use `latexmk` for Automatic Compilation**

```bash
sudo apt install latexmk
latexmk -pdf main.tex
```

This automatically handles multiple runs if needed.

---

## **About `main.tex`**

This LaTeX file uses standard **LaTeX libraries** and packages such as:

* `amsmath` – For mathematical formulas
* `graphicx` – For including images
* Others as required





### **Happy Coding!**
