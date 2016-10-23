1) Open /home/git/go/src/github.com/gogits/gogs/templates/base/head.tmpl

Add after:
```html
	<!-- Stylesheet -->
	<link rel="stylesheet" href="{{AppSubUrl}}/css/semantic-2.2.1.min.css">
	<link rel="stylesheet" href="{{AppSubUrl}}/css/gogs.css?v={{MD5 AppVer}}">
```
This line:
```html
	<link rel="stylesheet" href="{{AppSubUrl}}/css/custom.css">
```
2) Copy `custom.css` to `/home/git/go/src/github.com/gogits/gogs/public/css`
3) Run `service gogs restart`