# To2Moon_Doc

Petite Doc pour suivre l'avancement du projet et surtout comprendre facilement comment ça marche.
Objectif, n'importe qui doit pouvoir editer le projet pour implem et update les features qu'il veut.

git worktree add /tmp/book gh-pages
mdbook build
rm -rf /tmp/book/* # this won't delete the .git directory
cp -rp book/* /tmp/book/
cd /tmp/book
git add -A
git commit -m 'deploy new book'
git push origin gh-pages
cd -
