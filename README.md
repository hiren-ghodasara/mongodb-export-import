# mongodb-export-import

## Usage
- Download / Clone the script

    ```bash
    git clone https://github.com/hiren-ghodasara/mongodb-export-import.git
    cd mongo-sync
    ```

- Edit `config.yml` and insert your configuration details

	```yaml
	local:
	uri: "mongodb://localhost:27017"
	db: "xyz"

	remote:
	uri: "mongodb://localhost:27017"
	db: "abc"
	# For Heroku MongoDB URLs, here's the legend:
	# mongodb://username:password@hosturl.com:port/db_name
	# All fields are required
	```

- Use the script like this:
	
	```bash
	./mongo-sync push [options]		# Push DB to Remote
	./mongo-sync pull [options]		# Pull DB to Local
	```
- Options

	```
	-y  # Skip confirmation
	--config alternate-config-file.yml
	```
## License

Copyright (c) 2015 Hiren Ghodasara

MIT License

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

