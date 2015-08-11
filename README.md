twstat blog cli tool
---

A blog cli tool for twstat development usage.

## Install 

```
sudo npm install -g twstat-blog
```

#### Build project

First of all, go to your `taiwanstat.com` repo's root folder and enter the command.

```
twstatblog
```

#### watch project

First of all, go to your `taiwanstat.com` repo's root folder and enter the command, add watch option, will rebuild only the specific which is modifed.

```
twstatblog -w
```

#### Init your project

```
twstatblog init <date> <time> <name>
```

for example

```
twstatblog init 2015/08/11 11:10:27 test
```

this command will extend a new object in `blog.json`

```js
  {
    "title": "test",
    "date": "2015/08/11 11:10:27",
    "categories": [
      ""
    ],
    "tags": [
      ""
    ],
    "cover": "/assets/article_images/2015-08-11/test-cover.png",
    "content": "./posts/2015-08-11-test.md",
    "url_name": "test",
    "author": "taiwanstat"
  },
```

and also create a new folder for your project, for this example it will create and new folder called `2015-08-11-test.md` in `./posts/`.


`md`:

```md
## Title

content

### Subtitle

subcontent
```
