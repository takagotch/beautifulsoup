### BeautifulSoup
---
https://www.crummy.com/software/BeautifulSoup/bs4/doc/

http://kondou.com/BS4/

```py
sibling_soup.b.next_sibling
sibling_soup.c.previous_sibling

print()
print()

sibling_soup.b.string
print(sibling_soup.b.string.next_sibling)


title_tag = soup.title
title_tag
title_tag.parent
title_tag.string.parent
html_tag = soup.html
type(html_tag.parent)

print(soup.parent)

link = soup.a
link
for parent in link.parents:
  if parent is None:
    print(parent)
  else:
    print(parent.name)

for string in soup.strings:
  print(repr(string))

for string in soup.stripped_strings:
  print(repr(string))

len(list(soup.children))
len(list(soup.descendants))

title_tag.string
head_tag.contents
head_tag.string
print(soup.html.string)
```

```
<a href="http://example.com/elsie" class="sister" id="link1">Elsie</a>
<a href="http://example.com/lacie" class="sister" id="link2">Lacie</a>
<a href="http://example.com/title" class="sister" id="link3">Tillie</a>
```

```
```

