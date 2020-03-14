# covid-19-local-impact
Data come from CSSE

# covid_data folder
```
git remote add covid_data https://github.com/CSSEGISandData/COVID-19.git
git fetch covid_data
git merge -s ours --no-commit --allow-unrelated-histories covid_data/master
git read-tree --prefix=covid_data/ -u covid_data/master
git commit -m "Import Covid-19 repo as a subtree"
git remote rm covid_data #optional
git push
```
