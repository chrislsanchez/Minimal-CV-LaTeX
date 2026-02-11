# Modern LaTeX CV Template (German/English)

Hey there! Welcome to my CV template repository.

For the longest time, I relied on a trusty old LaTeX template. It served me well for years and got me through plenty of application rounds. But recently, I realized it was time for an upgrade. I wanted something cleaner, more modular, and easier to maintain.

So, I decided to "pair program" with an AI to build this. We took the best parts of the classic LaTeX approach and modernized the code structure, added easy configuration toggles, and polished the design for the German tech market.

It’s designed for **Senior Software Engineers**, but it’s flexible enough for anyone who wants a clean, professional look.

## Why this template?

*   **It’s Bilingual:** I needed a way to switch between German (*Lebenslauf*) and English (*CV*) without maintaining two separate files. There's a simple `true/false` toggle for that now.
*   **Academic Ready:** Since I have a background in research, I included a clean structure for PhD, Master, and Bachelor degrees.
*   **German Standards:** It respects the nuances of the German market (photo placement, signature space, "Anlagen" footer) but looks modern enough for international tech hubs like Berlin or Munich.
*   **ATS Friendly:** No weird text boxes or graphics that confuse Applicant Tracking Systems. Just clean, structured text.

## Features

*   **One-Page CV + Cover Letter:** Includes a matching *Anschreiben* on page 2.
*   **Smart Toggles:**
    *   `\englishfalse` / `\englishtrue`: Instantly swaps headers and date formats.
    *   `\showphototrue` / `\showphotofalse`: Hides the photo space if you prefer the US/UK style.
*   **Tech Stack Focus:** A dedicated side column for skills, languages, and certifications.
*   **Modern Icons:** Uses FontAwesome 5 for GitHub, LinkedIn, and Website links.

## How to use it

### 1. Prerequisites
You'll need a standard LaTeX distribution.
*   **Mac:** MacTeX
*   **Windows:** MiKTeX or TeX Live
*   **Linux:** `sudo apt install texlive-full`

### 2. Setup
Clone the repo and drop your profile picture in the folder.
```bash
git clone https://github.com/yourusername/cv-template.git
cd cv-template
```
*Make sure your photo is named `profile.jpg`. The code automatically crops it into a circle.*

### 3. Compile
I recommend using **XeLaTeX** because it handles fonts and icons much better than standard pdfLaTeX.

```bash
xelatex cv.tex
```
*(Run it twice to make sure the layout alignment is perfect).*

## Customization

Open `cv.tex` and look at the **Configuration** block at the top. It's heavily commented (thanks to the AI) so it's super easy to tweak.

**Switching Language:**
```latex
% Change to \englishtrue for English headers/dates
\englishfalse 
```

**Changing Colors:**
I use a "German Blue" (Prussian Blue), but you can swap it to black easily:
```latex
\colorlet{PrimaryColor}{black} 
```

**Adding Content:**
Just scroll down to the body and fill in your details.
*   Use `\workexp` for jobs.
*   Use `\education` for your degrees.
*   *Note: While the headers switch languages automatically, you still need to translate your bullet points manually!*

## License

Feel free to fork this, change it, and use it to land your next job. MIT License.