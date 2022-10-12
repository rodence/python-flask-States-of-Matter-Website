# python-flask-ITE-306-SAS-21-States-of-Matter-Website
States of Matter Flask Website

## If you want to see this website click the link below

Link:  [States of Matter Website](https://rodence.github.io/stateofmatter/index.html)


<div align='center'>
 <br><br>
<h2>TOOLS I USED TO BUILD THIS SITE</h2> 
 <img src="https://skillicons.dev/icons?i=html,css,js,vscode,python,bootstrap,flask&theme=dark&perline=8" />
 <br>
 <br>
 <br>
 <br>
</div>
			


## Step 1:

* Create a new folder and name it any what you want.
* Inside the folder create a new folder named `templates` and `static`.

## Step 2:
* Inside the templates folder create the html files of your website.
* Inside the static folder put all your resources including css,js,img files.
* And start coding your website.


## Step 3: 
* Now inside of your main folder create a new python file named `function.py`
and type the code below and save it:


```python
from flask import Flask, render_template, url_for

app = Flask(__name__)


@app.route("/home")
def home():
    return render_template("index.html")

@app.route("/gas")
def gas():
    return render_template("gas.html")

@app.route("/liquid")
def liquid():
    return render_template("liquid.html")


@app.route("/plasma")
def plasma():
    return render_template("plasma.html")

@app.route("/solid")
def solid():
    return render_template("solid.html")


if __name__ == "__main__":
    app.run(debug=True)
```
			
			
			
			
## Step 4:
* Run 	`function.py` in the terminal using the command `python function.py`
* The output in the terminal should be this:
		
```bash
* Serving Flask app 'function'
* Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
* Running on http://127.0.0.1:5000
Press CTRL+C to quit
* Restarting with stat
* Debugger is active!
* Debugger PIN: 836-352-937		
```
* Try to access the url:
			
			http://127.0.0.1:5000/home
			http://127.0.0.1:5000/gas
			http://127.0.0.1:5000/solid
			http://127.0.0.1:5000/liquid
			http://127.0.0.1:5000/plasma
