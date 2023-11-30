# ExplorationActivity2
<h1>Exploration Activity 2</h1>
<h2>Automation with Selenium, Time series analysis with pandas</h2>
<ol>
    <li>This program demonstrates the Selenium webdriver library, and builds on the previous EA's use of the pandas library for time series analysis, other data manipulation activities</li>
    <li>To run the program, Install all dependencies using pipfile:
    <pre><code>
    pipenv install
    </pre></code>
    You can alternatively install each dependency individually if you don't have pipenv setup.
    Run (exact command might differ slightly depending on the environment): 
    <pre><code>
    python3 index.py
    </pre></code>
    </li>
    <li>The purpose of this program is to calculate a weekly winner in the UNB finance club's paper trading competition. The original program is hosted at https://github.com/Khalid0md/marketwatch-weekly-movers and is scheduled to run weekly on a github actions cron job. This is a demo program, designed to be ran at will by a user. It will calculate the highest gainer since the first week of the competition. Another difference between this exploration activity demo and the original, this activity is designed to be ran multiple times without overwriting 'lastWeek.csv', the code to do so has been changed to write to 'lastWeek1.csv'.The original activity dynamically updates the file every week, getting ready for next week's run.</li>
    <li>There is no input required</li>
    <li>Here is a demo and some sample output: https://youtu.be/yVLYUxy0wac</li>
</ol>