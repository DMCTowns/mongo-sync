# mongo-sync

A bash script that allows data to be synchronised between multiple configured MongoDB instances

## Usage

- Download / Clone the script

  ```bash
  git clone https://github.com/DMCTowns/mongo-sync.git
  cd mongo-sync
  ```

- Edit `config.yml` and insert your configuration details

- Use the script like this:

  ```bash
  ./mongo-sync dev prod [options] # Push DB from dev to prod
  ```

- Options

  ```
  -y  # Skip confirmation
  --config alternate-config-file.yml
  ```

## Notes

- `mongo-sync` requires `mongodump` and `mongorestore` binaries to be installed in your system. If you have [`mongodb`](http://docs.mongodb.org/manual/tutorial/#getting-started) installed, then you probably already have them
- Pushing **_overwrites_** the Target DB
- It's a good idea to keep your `config.yml` in `.gitignore` if you're using it inside some other project

## License

Copyright (c) 2025 Diccon Towns
Copyright (c) 2015 Sheharyar Naseer

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
