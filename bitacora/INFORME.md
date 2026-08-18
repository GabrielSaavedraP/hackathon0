| Hallazgo | Dónde estaba | Técnica de Git | Comando exacto | Referencia |
|---|---|---|---|---|
| FRAG-01 | bitacora/frag-01.txt, borrado en commit de limpieza | Leer archivo borrado desde el commit padre | `git show 2de6fb9~1:bitacora/frag-01.txt` | `2de6fb9` |
| FRAG-02 | Mensaje del tag anotado `respaldo/pre-incidente` | Leer mensaje de un objeto tag con cat-file | `git cat-file -p refs/bundle/tags/respaldo/pre-incidente` | `refs/tags/respaldo/pre-incidente` |
| Glifo | Árbol del commit apuntado por el tag de respaldo | Checkout de un archivo desde una ref específica | `git checkout refs/bundle/tags/respaldo/pre-incidente -- assets/sello.svg` | `refs/tags/respaldo/pre-incidente` |
