# web-crawler
#python code for a web crawler based

print url
page = page[end_quote:]
start_link = page.find('<a href=')
start_quote = page.find('"', start_link)
end_quote = page.find('"', start_quote + 1)
url = page[start_quote + 1: end_quote]

#s is the parameter and is equal to page
def get_next_target(s):
    start_link = s.find('<a href=')
    start_quote = s.find('"', start_link)
    end_quote = s.find('"', start_quote + 1)
    url = s[start_quote + 1: end_quote]
    return url, end_quote
    #return is an <expression> that we want to get out of the webcrawler 
