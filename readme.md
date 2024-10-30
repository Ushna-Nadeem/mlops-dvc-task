dvc add data.csv
git add data.csv.dvc readme.md .gitignore
git commit -m "Track updated data.csv with DVC"
git push origin main
python main.py

==

git log
git checkout <commit_hash>  
dvc pull

==

git checkout main
git pull origin main
