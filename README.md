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
pelican content -o output -s pelicanconf.py
ghp-import output -r origin -b master -c www.flowious.com
git push origin master
```

## References
https://rasor.github.io/using-pelican-blog-on-github-pages.html
