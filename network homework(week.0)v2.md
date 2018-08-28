Пришлось покурить мануалы markdown, что бы узнать что катинки нельзя вставлять в файл без разрешения <br/>
![alt](strongpeach/cursor.free-aug-2018/blob/master/getrequest.png)


Task 1. Read.
http://code.tutsplus.com/articles/chrome-dev-tools-networking-and-the-console--net-28167
https://developer.chrome.com/devtools/docs/network#network-panel-overview <br/>
Прочитал гугл мануал по нетворк панели.


Task2. Play with Chrome Developers Toolkit (DevTools), and "Network" tab.
Choose at least 5 websites (any) - the list https://www.similarweb.com/top-websites/ukraine can be used as well (as an example of source of websites), or http://www.alexa.com/topsites/countries/UA, or any of https://en.wikipedia.org/wiki/List_of_most_popular_websites lists
Open each of them one by one. (that your browser made). Analyze the GET request/response packagies (the homework should include the whole package text including request-line and headers). Explain each of headers line (what "User-Agent" means? what "Accept" means? what does other means?)

Expected result:
the list of websites, with request and response (including the status-line & headers) of each of them
the list of headers (from above requests/responses) with descriptions of each (you need to google & find the purpose of each)
Познакомился с реквестами, разобрал 1 рандом реквест:

http://proshugaring.com/

Request headers: 
:authority: googleads.g.doubleclick.net
псвевдо хедер с доменом
:method: GET
псвевдо хедер с методом, кэп
:path: /pagead/adview?ai=C0DCFCd59W5-vGsybywW60LuIDNa9sd5SstDHkYEHwI23ARABIPfT6h1gpeajhogjyAEJqQJzECIb609jPqgDAcgDSKoEkAFP0ERE5lNZRxZIaA9lhaglRVtJT9QzV74fgC5P7rc6nXPllNkiCDRwb6DicBf1K0ixvsW52feFe0QZNlQ7HwOqEi-DxaPGEVqCxy0OZVzHOeDgdxWk1SOLplVnREPMH4RVY5jkMjOek9dtbMo4lddF2nLZQqVJQa1dAL0l9nUJcVKozDn1Zh5Wvi7e6Qhnig3ABJib56_XAZIFBAgEGAGSBQQIBRgEoAYugAftoZ1qqAeOzhuoB9XJG6gHqAaoB7oGqAfZyxuoB8_MG6gHpr4bqAeYzhuoB-nNG9gHAPIHBBCI0QnSCAcIgGEQARgCgAoB2BMC&sigh=AfpHQin17sQ&template_id=419&tpd=AGWhJms_0Md-Q_1LNtjMIp0TNCzK0TMxJlNYBmfTP7ebNTrePw
псвевдо хедер с урлой(путь+ возможные квери)
:scheme: https
псвевдо хедер с URI (протоколом)
accept: image/webp,image/apng,image/*,*/*;q=0.8
Media types that are acceptable for the response
accept-encoding: gzip, deflate, br
List of acceptable encodings
accept-language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,uk;q=0.6,fr;q=0.5
List of acceptable human languages for response
cache-control: no-cache
Used to specify directives that must be obeyed by all caching mechanisms along the request-response chain.
cookie: IDE=AHWqTUmTyocFkggDOpc6bZ4uo1-IHYEy9gQ1VoQnI4xIvCvVZksxjq-H5nMR5b8r; DSID=ADyxuktk4Mh-fMEi0ndHrAOdU54rRuuxC2fB2ImBS2cYfFTzeY9eO0w91F4e_pu3xtDtgck80jK-g7IPc8bIUUPEJPFRk0URDYbL0bpE32M6LrICqtFoYSM
HTTP cookie previously sent by the server with Set-Cookie
dnt: 1
do not track enabled
pragma: no-cache
Implementation-specific fields that may have various effects anywhere along the request-response chain.
referer: https://googleads.g.doubleclick.net/pagead/ads?client=ca-pub-2984730589635548&output=html&h=600&slotname=3335419140&adk=1830730735&adf=1648634183&w=240&fwrn=4&fwrnh=100&lmt=1534975496&rafmt=1&guci=2.2.0.0.2.2.0&format=240x600&url=http%3A%2F%2Fproshugaring.com%2F&flash=0&fwr=0&rh=300&rw=240&resp_fmts=4&wgl=1&dt=1534975496398&bpp=19&bdt=500&fdt=25&idt=252&shv=r20180815&cbv=r20180604&saldr=aa&abxe=1&correlator=4387649354616&frm=20&pv=2&ga_vid=1769947782.1534975497&ga_sid=1534975497&ga_hid=1715445334&ga_fc=0&iag=0&icsg=603925247&dssz=24&mdo=0&mso=0&u_tz=180&u_his=3&u_java=0&u_h=1080&u_w=1920&u_ah=1040&u_aw=1920&u_cd=24&u_nplug=3&u_nmime=4&adx=415&ady=1488&biw=1903&bih=150&scr_x=0&scr_y=1067&eid=4089040%2C10573695%2C21060853%2C368226400&oid=3&rx=0&eae=0&fc=528&brdim=0%2C0%2C0%2C0%2C1920%2C0%2C1920%2C1040%2C1920%2C150&vis=1&rsz=%7C%7CaopeEbr%7C&abl=CA&ppjl=f&pfx=0&fu=144&bc=7&ifi=1&fsb=1&xpc=v1JEiJyiLw&p=http%3A//proshugaring.com&dtd=287
This is the address of the previous web page from which a link to the currently requested page was followed.
user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36
Browser&OS&device of user
x-client-data: CJG2yQEIo7bJAQjEtskBCKmdygEI153KAQjZncoBCKijygEIn6bKAQ==
uncommon and non-standard header

Response headers:
alt-svc: quic="googleads.g.doubleclick.net:443"; ma=2592000; v="44,43,39,35",quic=":443"; ma=2592000; v="44,43,39,35"
A server uses "Alt-Svc" header (meaning Alternative Services) to indicate that its resources can also be accessed at a different network location (host or port) or using a different protocol
content-length: 0
  The length of the response body in octets (8-bit bytes)
date: Wed, 22 Aug 2018 22:04:57 GMT
The date and time that the message was originated
p3p: policyref="https://googleads.g.doubleclick.net/pagead/gcn_p3p_.xml", CP="CURa ADMa DEVa TAIo PSAo PSDo OUR IND UNI PUR INT DEM STA PRE COM NAV OTC NOI DSP COR"
This field is supposed to set P3P policy
server: cafe
A name for the server
status: 200
status of the HTTP response
timing-allow-origin: *
что это вообще такое...
x-xss-protection: 1; mode=block
Cross-site scripting (XSS) filter

Task3. What are differences between HTTP version 1.0 and 1.1?
navigate your browser to websites what you're frequently use (the company's website, some social networks, etc)

Expected result:
list of differences between 1.0 and 1.1
answer to question - how to pass user-data via GET? via POST? what is the diff?
few samples of websites (and cases) where POST method is used

Ответы:
list of differences between HTTP 1.0 and 1.1
Host в хедере, улучшенныая поддержка кеша и использование одногоTCP конекшена для множества реквестов.

how to pass user-data via GET? via POST? what is the diff?
Инфа методом get кодируется в url, инфа методом post высылается в body реквеста.

few samples of websites (and cases) where POST method is used
Поиск в http://www.liveinternet.ru/search/?q=1312321 отправляет инфу методом POST,
Подписка на удаве http://udaff.com/subscribe/ ну все заполнение форм, поидее, методом post работает.

Task4. Use the "telnet" program.
(!) in case if your're under Windows 7/8/10 - google how to enable the "telnet" service on your system
create the GET and HEAD package requests to google.com:80
if you receive the "3**" status code (redirection), try to manually navigate to new-location url

Expected result:
screenshot with http request
screenshot with http response package with response-code equals to "200 OK"
Телнет так и не запустился у меня, я использовал онлайн-телнет...


Task5. Use actions on "Network" tab.
try to use a "search" & "filter" fields/actions
use ordering by columns, sorting, etc

Expected result:
describe what feature have you used, and how you can use it in future
Пригодилась фильтрация запросов по type, размеру, времени загрузки. В будущем можно эту инфу использовать для дебага.
Можно менять юзерагента и смотреть мобайл версию с десктопа или же отключать кеш и даже смотреть скриншоты загрузки страницы...

Task 6. Using the hurl.it
create a GET request to any website
analyze the response

Expected result:
the HTTP request & response (including request-line / status-line & headers)
description of each header line on response

![Figure 1-1](http://i.piccy.info/i9/9e12c8e5e6eb99200807d17bbc891610/1533764685/354987/1259842/kk.png?raw=true "Figure 1-1")

Task 7. Using the hurl.it
the same as above task, but you need to create the "HEAD" requests


Task 8. What is the different with GET request?
Expected result:

the HTTP request & response (including request-line / status-line & headers)
the answer to question about differences between HEAD and GET methods


Task 9. Find and show few (at least 5) resources, where POST method is used
list the URLs of resources
explain how did you detect that POST method was used?
what response was returned after request has been sent?
Expected result:

list with websites & description where POST is used there
answer to question why the POST is used there

Task 10. Using the Postman extension
set it up, if not installed yet
send 5 any requests (including HEAD, GET & POST) to any website
Expected result: 

screenshot with request & response from Postman


Task 11. Find any free hosting that provides FTP accessgoogle "ftp free hosting", or "free hosting", etc

proceed registration, confirmation & get your ftp access credentials (host/port, login, password)
using any ftp client, deploy any static files (html, any images, etc)
provide an url (http link) that navigates to uploaded file
Expected result:

direct url into uploaded file



Advanced level
Не делал...
