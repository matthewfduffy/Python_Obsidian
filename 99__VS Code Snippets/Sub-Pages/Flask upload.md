#flask-snippet
`fup`

```py
@app.route('/upload', methods=['GET', 'POST'])
def upload_file():
	if request.method == 'POST':
		f = request.files['the_file']
		f.save('/path/to/save/the_file.txt')
```