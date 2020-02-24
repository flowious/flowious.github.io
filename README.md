## Develop
```
cd flowious.github.io
git checkout pelican
pelican content
cd output
python -m pelican.server
```
Browse to http://localhost:8000

## Publish
```
pelican content -o output -s pelicanconf.py -c www.flowious.com
ghp-import output -r origin -b master
git push origin master
```
