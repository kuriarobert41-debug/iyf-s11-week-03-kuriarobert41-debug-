# Terminal commands used (simulated)

This file documents the terminal commands you would run to complete the Week 3 terminal exercises. I added the project files directly to the repository, but to reproduce and practice these steps locally, run the commands below in your terminal.

## Task 5.2 / Task 5.1 — Create project structure

# From your desired parent directory
mkdir -p iyf-s11-week-03-kuriarobert41-debug-/src/{css,js,images} iyf-s11-week-03-kuriarobert41-debug-/docs iyf-s11-week-03-kuriarobert41-debug-/tests
cd iyf-s11-week-03-kuriarobert41-debug-

# Create files
touch README.md index.html about.html projects.html contact.html
touch src/index.html src/css/styles.css src/js/main.js

# Verify
ls -R

## Task 5.2 — File operations (examples)
# Copy and move
cp index.html backup.html
mv backup.html docs/

# Rename
mv index.html home.html
rm home.html

# Copy directory
cp -r src/ src-backup/
mv src-backup/ archive/
rm -r archive/

## Task 5.3 — Useful terminal commands (examples to run locally)
# Find files by name
find . -name "*.html"

# Search inside files
grep -r "contact" ./

# Count lines in CSS file
wc -l src/css/styles.css

# Last 10 commands
history | tail -n 10

## Task 5.4 — Run the setup script
# Make script executable and run
chmod +x new-project.sh
./new-project.sh my-sample-project
