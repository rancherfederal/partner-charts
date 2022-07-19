# Partner Charts

Charts from our partners packaged into a Rancher Catalog.

#### Adding a new chart

From the `charts/` folder, run the following command:

` kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] ./PKG_NAME/`

#### Updating a chart

From the `charts/` folder, run the following command:

```
cp PKG_NAME/questions.yml /tmp/. && cp PKG_NAME/app-readme.md /tmp/. ; \
kpt pkg update PKG_NAME/[@VERSION] --strategy force-delete-replace ; \
cp /tmp/questions.yml PKG_NAME/. && cp /tmp/app-readme.md PKG_NAME/.
```