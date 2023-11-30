<h1>Selenium Webdriver overview</h1>
<p>"Selenium automates browsers ... Primarily it is for automating web applications for testing purposes, but is certainly not limited to just that. Boring web-based administration tasks can (and should) also be automated as well.<a href="https://www.selenium.dev/">[ref]</a> "</p>
<p>The purpose of Selenium's Webdriver is to communicate directly with an instance of a web browser. Developers may want to do this for many reasons, but it is most prominently used in the industry for front-end testing. Selenium can also be used to automate tasks and can be anything from logging daily visits to a website, to, in my case, logging into a website, and scraping data on a timely basis. This can all be done in code, as the python library offers multiple functions for clicking, executing javascript code, scraping the DOM, among others.</p>
<p>Some of the functionalities of the Selenium Webdriver are showcased in the code. These include:
    <ul>
        <li>Navigating to a webpage: ```driver.get(login_url)```</li>
        <li>Executing Javascript on the browser: ``` driver.execute_script(
        "document.getElementById('username').value = arguments[0];", 
        username
    )```</li>
        <li>Clicking links within the page: ```continue_button_selector = "#basic-login > div:nth-child(1) > form > div:nth-child(2) > div:nth-child(6) > div.sign-in.hide-if-one-time-linking > button.solid-button.continue-submit.new-design"
    driver.execute_script(f"document.querySelector('{continue_button_selector}').click();")```</li>
        <li>Teeing up a webpage to be scraped by other libraries like Beautiful Soup: ```soup = BeautifulSoup(driver.page_source, 'html.parser')```</li>
    </ul>
</p>
<p>Selenium was created by Jason Huggins in 2004 <a href="https://www.guru99.com/introduction-to-selenium.html">[ref]</a></p>
<p>I selected this library because I needed to automate a boring and time-consuming task that was going to have to be done manually by one of my finance club team members. More importantly, there is no marketwatch API so I needed to go on the website and sign in, turn pages of the leaderboard table, and scrape the data.</p>
<p>Learning to use Selenium Webdriver forced me to enhance my data analysis and manipulation skills as the data I got back was raw HTML. It also stressed the importance of javascript's await/async framework, and python's data manipulation capabilities. It really made me appreciate each language and understand it's strengths and weaknesses.</p>
<p>my experience with the library was really seamless and easy. I would recommend this library to anyone who needs to automate web based tasks and maybe perform unorthodox tasks that are not exposed to an API. I would continue using this package in the future, but it depends on the nature of the task I need to perform. If I need to automate a quick task or to test front-end elements, I would surely use it. But if I need robust, reliable data, I would find a way to reverse engineer an API</p>

