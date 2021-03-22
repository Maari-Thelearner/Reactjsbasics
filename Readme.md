# Reactjs Basic Commands
	
**How to Create a Reactjs Application in quick!**\
		`npx create-react-app firstproject`\
	*This command which is used to create a REACTJS projects quick and it will create everything*

**************************************************************


**How to create a Reactjs Application from Stratch** \\
	Step 1 : `mkdir firstproject` \ 
	Step 2 : `cd firstproject` \ 
	Step 3 : `npm init -y` \
	Step 4 : `npm install -D lite-server` \
	Step 5 : `touch index.html` \
	Step 6 : Change one line in package.json
```javascript
				"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
  },
  			to
  			"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "lite-server"
  },
```
	Step 6 : `npm run dev`


**************************************************************

**Creating the javascript file inside the Reactjs project**\
	Step 1 : `touch app.js`
	Step 2 : Write a Javascript code inside the app.js file \ 
```javascript
const  name = React.createElement('h1',{},'This is my name Marimuthu');

ReactDOM.render(name,document.getElementById('root'))
```
_This is the example code purpose of this code is to print our name in the webpage_\
	Step 3 : Connect our index.html page with Reactjs and ReactDOM Javascript file\
	_search the offical Reactjs site and click the CDN link (developer link is enough as of now) and get the two script crossorigin link_\
	Step 4 : Modify the index.html like the Below html code
```HTML
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>React Basis</title>
</head>
<body>
    <div id="root"></div>
<script crossorigin src="https://unpkg.com/react@17/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@17/umd/react-dom.development.js"></script>
<script src="app.js"></script>
</body>
</html>
```


