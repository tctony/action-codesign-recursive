# action-codesign-recursive
do codesign on xcode app recursively

Use it inside steps like this
```
- name: Codesign
  uses: tctony/action-codesign-recursive@v1
  with:
    identity: ${{ secrets.CERT_NAME }}
    path: Some.app
    options: '--options runtime'
```
