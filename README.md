# JekyllFrontMatterMd
### Motivation
I like to write articles that use markdown `#` as the title. By default, [Jekyll](https://jekyllrb.com/) uses the file name as the title of the article. We can use the [Front Matter](https://jekyllrb.com/docs/frontmatter/) `tittle` property to customize the title of the article, but when we need to publish the article to different blog platform, We need to add different formatting of the same article. So I wrote this python tool to convert the original article into an article with [Front Matter](https://jekyllrb.com/docs/frontmatter/).

The tool will set the first line with `#` to the [Front Matter](https://jekyllrb.com/docs/frontmatter/)'s `title` property and the convert time to the `date` property.

### Usage
```python
python3 md_to_jekyll_post.py [input file name]

```
before:
```
# This is a temp markdown title
This is a temp markdown content.
```
after:
```
---
title: This is a temp markdown title
date: 2018-05-10 12:12:33 +0800
---
This is a temp markdown content.
```

### ToDo
* Add output path argument
* Use [argparse](https://docs.python.org/3.3/library/argparse.html) to process command arguments

# License
	Copyright (c) 2018 littlegnal

	Permission is hereby granted, free of charge, to any person obtaining a copy
	of this software and associated documentation files (the "Software"), to deal
	in the Software without restriction, including without limitation the rights
	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
	copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:

	The above copyright notice and this permission notice shall be included in all
	copies or substantial portions of the Software.

	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
	SOFTWARE.