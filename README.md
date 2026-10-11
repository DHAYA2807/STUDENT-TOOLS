# Student Tools — FOS Assignment 2

## Aim
Create a sample Python package, host it in a Git repository, check out a file, modify it, and push the changes.

## Package contents
- `student_tools/__init__.py` — exposes package functions.
- `student_tools/greetings.py` — greeting function.
- `student_tools/calculator.py` — addition and subtraction functions.
- `main.py` — runs the package examples.

## Run locally
Install Python 3. Run from this folder:
```bash
python main.py
```

Expected output:
```text
Hello, Student! Welcome to Student Tools.
10 + 5 = 15
10 - 5 = 5
```

## Git hosting and change workflow
Create an empty repository on GitHub named `student-tools-fos` (do not add a README if you already have this folder).

```bash
git init
git add .
git commit -m "Create student tools package"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/student-tools-fos.git
git push -u origin main
```

To check out the repository and edit a file:
```bash
cd ..
git clone https://github.com/YOUR-USERNAME/student-tools-fos.git
cd student-tools-fos
```
Open `student_tools/greetings.py` and change the greeting text, for example:
```python
return f"Hello, {name}! Welcome to the Updated Student Tools Package."
```
Then commit and push:
```bash
git add student_tools/greetings.py
git commit -m "Update greeting message"
git push origin main
```

Replace `YOUR-USERNAME` with your actual GitHub username. Use your own repository URL. Capture screenshots of the repository page, initial commit, changed file, and successful push for your submission.
