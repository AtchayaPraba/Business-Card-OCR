# Business-Card-OCR
## Intelligent Document Processing of Business Card you using Optical Character Recognition

### GitHub COMMANDS
1. Check remote url
```
git remote -v
```
2. Check branch of repository
```
git branch
```
3. Add files to GitHub repository
```
git add <file_name>
```
OR
```
git add <file_name1>, <file_name2>, <file_name3>, ...<file_namen>
```
OR
```
git add .
```
4. Check file status
```
git status
```
5. Save / commit the changes in GitHub for version control 
```
git commit
```
OR 
```
git commit -m "any_message"
```
6. View the versions in GitHub
```
git log
```
7. Send version / changes to github repo
```
git push origin main
```
8. Download files form remote url
```
git pull
```
OR
```
git fetch
```
9. Check the difference
```
git diff
```
10. Restore file
```
git restore --staged <file_name>
```
>>NOTE: [MORE GIT COMMANDS](https://git-scm.com/docs/gittutorial)


### Step 01:
1. Create a GitHub Repository
2. Add README.md, .gitignore and LICENSE files

### Step 02:
1. Clone the GitHub Repository
```
git clone <github_repo_link>
```
2. Open in VS code. Launch VS Code in the pwd
```
code .
```
### Step 03: VIRTUAL ENVIRONMENT 
1. Create conda virtual environment 
```
conda create -p venv python==3.7 -y
```
2. Activate conda virtual environment
```
conda activate venv
```
OR
```
conda activate venv/
```
3. Initialize virtual environment 
```
conda init cmd.exe
```
>> NOTE: close and reopen VS code

### Step 04: INSTALL .ipynb kernel
```
pip install ipykernel
```

### Step 05: "requirements.txt" FILE
1. Create requirements.txt file
2. Install requirements.txt file
```
pip install -r requirements.txt
``` 

### Step 06: PYTESSRACT
>> NOTE: [Python-tesseract](https://pypi.org/project/pytesseract/) is an optical character recognition (OCR) tool for python. That is, it will recognize and “read” the text embedded in images. Python-tesseract is a open source wrapper for Google’s Tesseract-OCR Engine.

1. Install stable version of .exe pytesseract form [pytessract](https://digi.bib.uni-mannheim.de/tesseract/) or [pytessract_versions](https://tesseract-ocr.github.io/tessdoc/Installation.html)
2. Install "pytesseract" in virtual environment
```
pip install pytesseract
```
3. LIMITATIONS: 
- Assumes text aligned in order. Text in image should not be rotated or skewed.
- Text should not be blur.
- Does not work for text with effects.
- Does not work for cursive handwritten text
- Resolution of the image should be at least 200 dpi or width and height should be at least 300 pixels.

### Step 07: spaCy
1. Install [spaCy](https://spacy.io/usage)
```
pip install -U spacy
```
2. Install "en_core_web_sm" module diretly or by downloading .tar or .whl files
```
python -m spacy download en_core_web_sm
```
or
```
pip install en_core_web_md-3.4.1.tar.gz
```
or
```
pip install en_core_web_md-3.4.1.tar.gz.whl
```
