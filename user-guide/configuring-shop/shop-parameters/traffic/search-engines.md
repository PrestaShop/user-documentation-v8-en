# Search Engines

A lot of you visitors will come from search engines. In order to know what they were looking for, and how you can improve your shop for their search queries, you need to know their queries.

This page presents a table of all the search engines that your installation of PrestaShop supports – meaning that PrestaShop is able to recognize it, and to extract the query that the visitor from that given search engine used to find your shop.

![](<../../../../.gitbook/assets/23789937 (4) (4) (2).png>)

While Google has the biggest share of search engines users, there are many other search engines that people could use to find your website. Therefore, you have to be able to retrieve their search requests too. When an unknown search engine is starting to bring regular visitors, it is high time that you add it to your database – otherwise, those visitors would be marked in your statistics as coming from "Other search engines", which is not helpful at all.

## Adding a Search Engine <a href="#searchengines-addingasearchengine" id="searchengines-addingasearchengine"></a>

It is very simple to add a new search engine to your list.

![](<../../../../.gitbook/assets/23789939 (4) (4) (4).png>)

Let's say you want to add DuckDuckGo, a search engine that emphasizes its respect for data privacy:

1. Get the full referrer URL for the search. For instance, [http://duckduckgo.com/?q=kids+shoes](http://duckduckgo.com/?q=kids+shoes)
2. Take the domain name, which is specific to that search engine, and put it in the "Server" field. In our case, "duckduckgo".
3. Find the query variable:
   1. Find the query string. It should be a set of letters, followed by an "=" sign, followed by the query itself, closed by a "&" or the end of the string. In our case, it is "q=kids+shoes".
   2. The query variable is the set of letters before the "=" sign. In our case: "q". Put that in the "$\_GET variable" field.
4. Click the "Save" button, and from now on, PrestaShop will be able to recognize visitors from DuckDuckGo.
