# datasette.ipwa02-01.iu.stefan-dev.de

[![Vercel](../../actions/workflows/vercel.yml/badge.svg)](../../actions/workflows/vercel.yml)

Global historical emissions from https://data.worldbank.org/indicator/EN.ATM.CO2E.KT.

## ⚙️ Get Started

You'll need [Datasette](https://datasette.io/) and [Python](https://python.org) installed.

### Clone Repository

First of all, you need to clone the repository:

```bash
$ git clone https://github.com/bystefankuehnel/datasette.ipwa02-01.iu.stefan-dev.de.git
$ cd datasette.ipwa02-01.iu.stefan-dev.de
```

### Install PIP Dependencies

```bash
$ python -m pip install --upgrade pip
$ pip install -r requirements.txt
```

### Download SQLite Database

```bash
$ curl \
    --silent \
    --show-error \
    --location \
    --output emissions.db \
    https://datasette.ipwa02-01.iu.stefan-dev.de/emissions.db
```

### Run Datasette

```bash
$ datasette emissions.db \
    --metadata metadata.json \
    --open
```

It will listen on [http://127.0.0.1:8001](http://127.0.0.1:8001) unless otherwise configured.

## 🔨 Technology

The following technologies, tools and platforms were used during development.

- **Code**: [Python](https://www.python.org)
- **Database**: [SQLite](https://sqlite.org)
- **Deployment**: [Vercel](https://vercel.com)

## 👷‍ Error Found?

Thank you for your message! Please fill out a [bug report](../../issues/new?assignees=&labels=&template=bug_report.md&title=).

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

```
The MIT License (MIT)

Copyright © 2022 Stefan Kühnel

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
