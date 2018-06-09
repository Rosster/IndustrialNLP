# IndustrialNLP

Instructions:

First download the `wikihow` scrape here: https://archive.org/download/wikihowcom

Then download `spacy` here: https://spacy.io/usage/

And the `en_core_web_lg` according to instructions here: https://spacy.io/usage/models

First run the `Final Project Data Exploration` script, this will parse the XML, and isolate the sections of each page (using regular expressions).  The file will save a pickle file of `Post` objects that the next program uses to build a question-answer system.

Next run the `Final Project NLP Code` program.  This will create two objects, `robot` and `industry_qa`.  It will take ~ 2hrs to build them on a laptop.

Finally, use the `ask` method on either robot to get the tools required to solve various problems, ie:

```robot.ask('fix a hole in the wall')
Total similarity: 0.9619860490105135
Matched on Fix a Hole in a Wall
{'120 grit sandpaper',
 'a good six or four inch putty knife',
 'standard wallboard joint compound',
 'the block or sanding device'}
>>> 
```
