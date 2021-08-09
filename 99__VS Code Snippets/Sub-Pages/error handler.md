#flask-snippet
`feh`

```py
@app.errorhandler(404)
def bar(error):
	return render_template('error.html'), 404
```