import requests
from bs4 import BeautifulSoup

def get_article_cnn(url):
  response = requests.get(url)
  soup = BeautifulSoup(response.content, 'lxml')
  article = soup.findAll("div", {"class : "zn-body__paragraph"})
  return(article)
 
url = 'any_cnn_news_article'
print(get_article_cnn(url))
