chinese-keywords
================

Contained is a set of sensitive Chinese keywords (that is, keywords related to the Chinese Communist party, pornography, dissident material, violence/terrorism, censorship, etc). These keywords may be helpful to researchers who are searching for sensitive content in Chinese or testing for network interference.

As of Dec 9, there are 9,054 sensitive keywords collected from 13 different lists (see below for detailed info on the lists). To get a sense of what data is included in these CSV files, you can view a Google Doc spreadsheet of these 9,054 keywords sorted by the number of lists they appear on: https://docs.google.com/spreadsheets/d/19eS47Dg086vR1jh9oo51pXstYVT2wft13JGCrnAeU7A/edit?usp=sharing

The CSV files contain machine translations (from Google) and human translations/notes for most of the keywords. Many also have theme and category variables included as well thanks to various sources which have previously tagged their keyword lists. Currently, there are three different versions:
* __all.csv__: all the keywords, all available data/variables, plus 3,987 popular (3,803 non-sensitive) keywords which can be used as possible controls for searching. These popular/non-sensitive keywords were taken from [article titles of the top 1000 most viewed articles on Wikipedia China in April 2013](http://stats.grok.se/zh/top) (995 after a few Wikipedia meta-pages were removed) and  [titles of articles that generated more than a total of 10 combined views on August 1, 0:00-1:00 and 12:00-13:00](http://dumps.wikimedia.org/other/pagecounts-raw/2013/2013-08/).
* __no-dummy-vars-for-categories-and-themes.csv__: all the keywords without dummy variables for each of the themes and categories that were tagged by The Citizen Lab. Category/theme info is instead stored in catch-all "category" and "theme" variable (column). 
* __no-dummy-vars-for-categories-and-themes_only-sensitive-words.csv__: same as above except also with the non-sensitive words removed.
Once downloaded, you can also sort by keyword length as well as how many of the lists each keyword appears on. 

The thirteen lists this collection contains are:

Creator/source | Tested on/found from | # of keywords | Year | Method + source
------------ | ------------- |---------|------------|------------
The Citizen Lab | Sina UC | 1,818 | 2013| [reverse engineered](http://firstmonday.org/ojs/index.php/fm/article/view/4628/3727) from the client; more analysis [here](https://citizenlab.org/2013/07/using-the-china-chats-surveillancecensorship-keyword-list-analyzing-blocked-terms-search-result-numbers-and-overlaps-of-censored-terms-between-services/); [download link](https://github.com/citizenlab/chat-censorship/tree/master/TOM-Skype--Sina-UC)
The Citizen Lab | Tom-Skype | 2,574 | 2013 | [reverse engineered](http://firstmonday.org/ojs/index.php/fm/article/view/4628/3727) from the client; more analysis [here](https://citizenlab.org/2013/07/using-the-china-chats-surveillancecensorship-keyword-list-analyzing-blocked-terms-search-result-numbers-and-overlaps-of-censored-terms-between-services/); [download link](https://github.com/citizenlab/chat-censorship/tree/master/TOM-Skype--Sina-UC)
The Citizen Lab | LINE | 673 | 2014 | [reverse engineered](https://citizenlab.org/2013/11/asia-chats-investigating-regionally-based-keyword-censorship-line/) from the client; more analysis [here](http://blockedonweibo.tumblr.com/post/67667357020/update-the-chinese-keywords-on-messaging-app-line-s-bad); [download link](https://github.com/citizenlab/chat-censorship/tree/master/LINE)
Jason Q. Ng (Blocked on Weibo) | Sina Weibo | 839 | 2013| [running Wikipedia China article titles](http://www.wagingnonviolence.org/feature/how-china-gets-the-internet-to-censor-itself/) through Sina Weibo search; [more analysis](http://blockedonweibo.tumblr.com) and [book](http://www.jasonqng.com/p/book-blocked-on-weibo.html)
Xia Chu | Great Firewall | 669 | 2014 | [HTTP request scans of Wikipedia China articles](https://docs.google.com/file/d/0B8ztBERe_FUwLWxUX0laeWF3aE0/edit) to see if they'd trigger GFW block; more analysis [here](http://blockedonweibo.tumblr.com/post/72871268045/comments-and-takeaways-from-xia-chus-complete-gfw); [download link](https://docs.google.com/spreadsheet/ccc?key=0AsztBERe_FUwdDVBSk8waThMeHlvS2d6dF9GMWl6dkE&usp=sharing#gid=0) (removed duplicates and keywords related to meta and user pages)
China Digital Times | Sina Weibo | 2,448 | ongoing | [crowdsourced testing of suspected sensitive keywords](https://docs.google.com/spreadsheet/ccc?key=0Aqe87wrWj9w_dFpJWjZoM19BNkFfV2JrWS1pMEtYcEE#gid=0) on Sina Weibo; more analysis on [CDT](http://chinadigitaltimes.net/china/sensitive-words-series/) and in CDT's [Grass Mud Horse Lexicon e-book](http://chinadigitaltimes.net/space/Grass-Mud_Horse_Lexicon); [download link](https://docs.google.com/spreadsheet/ccc?key=0Aqe87wrWj9w_dFpJWjZoM19BNkFfV2JrWS1pMEtYcEE#gid=0)
GreatFire.org | Wikipedia | 488 | 2013 | testing to see if Wikipedia pages are available in China; [more info](https://en.greatfire.org/blog/2013/jun/wikipedia-drops-ball-china-not-too-late-make-amends); [download link](https://en.greatfire.org/search/wikipedia-pages)
Google/ATGFW.org | Google/Great Firewall | 456 | 2012 | ATGFW.org and GreatFire.org [reverse engineered the keywords Google was using](https://en.greatfire.org/blog/2012/jun/all-blocked-keywords-according-google) to warn users of censorship while using their service in China; [download link](http://www.atgfw.org/2012/06/googlegfw.html)
Jeff Knockel | Sina Show | 910 | 2014 | [extracted list from Sina Show app](http://cs.unm.edu/~jeffk/sinashow/); [download link](http://cs.unm.edu/~jeffk/sinashow/SinaShow.plain)
Unknown | 163.com | 376 | 2008 | [archived by Nart Villeneuve](http://www.nartv.org/2008/11/25/keyword-lists/); circulated on 163.com, a Chinese portal website [download link](http://www.nartv.org/projects/keywords/badwords.txt)
Omnitalk BBS users? | Tencent QQ | 863 | 2004 | [archived by Nart Villeneuve](http://www.nartv.org/2008/11/25/keyword-lists/); extracted from Tencent QQ app, [more info and analysis from CDT](http://chinadigitaltimes.net/2004/08/the-words-you-never-see-in-chinese-cyberspace/) [download link](http://www.nartv.org/projects/keywords/qqdll.txt)
Jed Crandall et al / "ConceptDoppler" | Great Firewall | 669 | 2008 | [archived by Nart Villeneuve](http://www.nartv.org/2008/11/25/keyword-lists/); "HTTP keyword filtering by Internet routers"; [website](http://www.conceptdoppler.org/); [paper](https://www.cs.unm.edu/~crandall/concept_doppler_ccs07.pdf); [download link](http://www.nartv.org/projects/keywords/condoppler.txt)
Unknown | a "blog provider" | 844 | 2005 | [archived by Nart Villeneuve](http://www.nartv.org/2008/11/25/keyword-lists/); according to Villeneuve: "This is a keyword list from a blog provider in China." [download link](http://www.nartv.org/projects/keywords/keyword.txt)
This project was started at [The Citizen Lab's 2014 Connaught Summer Institute workshop](http://citizenlab.org/summerinstitute/2014.html). 
