from django.db import models


class Author(models.Model):
    author_name = models.CharField(max_length=30)
   
    def __str__(self):             
        return self.author_name

class Article(models.Model):
    author_name = models.ForeignKey(Author)
    article_title = models.CharField(max_length=100, default ="the")
    article_text = models.CharField(max_length=1000)
    pub_date = models.DateTimeField('date published')
    
    def __str__(self):             
        return self.article_title
