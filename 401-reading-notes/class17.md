# Web Scraping

Web scraping is a task that has to be performed responsibly so that it does not have a detrimental effect on the sites being scraped. Web Crawlers can retrieve data much quicker, in greater depth than humans, so bad scraping practices can have some impact on the performance of the site. While most websites may not have anti-scraping mechanisms, some sites use measures that can lead to web scraping getting blocked, because they do not believe in open data access.

Web Scraping best practices to follow to scrape without getting blocked

. Respect Robots.txt : Web spiders should ideally follow the robot.txt file for a website while scraping. It has specific rules for good behavior, such as how frequently you can scrape, which pages allow scraping, and which ones you can’t.

. Make the crawling slower, do not slam the server, treat websites nicely: Use auto throttling mechanisms which will automatically throttle the crawling speed based on the load on both the spider and the website that you are crawling. Adjust the spider to an optimum crawling speed after a few trial runs. Do this periodically because the environment does change over time.

. Do not follow the same crawling pattern: Incorporate some random clicks on the page, mouse movements and random actions that will make a spider look like a human.

. Make requests through Proxies and rotate them as needed: Create a pool of IPs that you can use and use random ones for each request. Along with this, you have to spread a handful of requests across multiple IPs.

. Rotate User Agents and corresponding HTTP Request Headers between requests:  user agent is a tool that tells the server which web browser is being used. If the user agent is not set, websites won’t let you view content. Every request made from a web browser contains a user-agent header and using the same user-agent consistently leads to the detection of a bot.

. Use a headless browser like Puppeteer, Selenium or Playwright: The simplest check is if the client (web browser) can render a block of JavaScript. If it doesn’t, then it pretty much flags the visitor to be a bot. While it is possible to block running JavaScript in the browser, most of the Internet sites will be unusable in such a scenario and as a result, most browsers will have JavaScript enabled.

. Beware of Honey Pot Traps: Honeypots are systems set up to lure hackers and detect any hacking attempts that try to gain information. It is usually an application that imitates the behavior of a real system. Some websites install honeypots, which are links invisible to normal users but can be seen by web scrapers.

. Check if Website is Changing Layouts: Some websites make it tricky for scrapers, serving slightly different layouts. For example, in a website pages 1-20 will display a layout, and the rest of the pages may display something else. To prevent this, check if you are getting data scraped using XPaths or CSS selectors. If not, check how the layout is different and add a condition in your code to scrape those pages differently.

. Avoid scraping data behind a login: If a page is protected by login, the scraper would have to send some information or cookies along with each request to view the page. This makes it easy for the target website to see requests coming from the same address. They could take away your credentials or block your account which can, in turn, lead to your web scraping efforts being blocked.

Its generally preferred to avoid scraping websites that have a login as you will get blocked easily, but one thing you can do is imitate human browsers whenever authentication is required you get the target data you need.

Notes taken from(https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)