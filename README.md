# scratcher
Scraper
This program is a simple tool, collecting information about housing in israel.
For now, there is default city code (7900) stands for Petah-Tikva, user can change city simply replacing petah-tikva`s code with some other
(for example kiryat-ono has a code 7800). Then the user must pass an argument about how many search pages he needs in this session, the default will only bring 
the first page.
Scratcher will analyze each page individualy with a request function, extract the symbols nedded for further requests(get responses in json format),
it will then write json to a json file.
Example: I need to get information from the first 10 pages in kiryat ono for sale search. I then pass 7800 for city code num and 10 as for 10 pages.
for this requirements I will get 10 files, each containing about 40 results for this search.