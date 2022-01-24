# Explanation of deliverable and video call

Welcome to our take home data science case! We're very happy that you applied for our new role.
Today you will be given a challenge for which we want you to find a solution.
You're free to be creative and use any package or method. 

After 24 hours you have to make a pull request, containing at least the following:

1. A working & understandable code solving the case
2. A requirements.txt file with packages used
3. A short presentation explaining how and why you've chosen this method / solution, 
       how your solution performs and which recommendations you have for further improvements. 

After 24 hours we will have a video call to walk through your solution, chosen methods, performance and recommendations. You will use the presentation as means to communicate clearly, this is something we often do in our company to keep everything understandable and explainable.

# Background information
KeyWI is a ai-driven solution for online marketeers. We provide valuable data insights for keywords and help SEO specialists to make the best choices. Therefor, we cluster keywords, predict search intention, show current rank, and much more. 

We are always interested in what does work and what does not work. Let me explain, some websites do rank, while others don't.. how come? To be able to aid in the creation of new content, we want to provide insights in currently ranking content. That's why we want to show which type of page rank, what kind of content did people create?

# Explanation of case

To start the case clone this repo to your machine and switch to a new branch.
- [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the repo to your own github account
- `git clone <reponame>`

After cloning, you should download a file called `pages.zip`,
which is publicly available on `https://keywi-public.s3.eu-west-1.amazonaws.com/pages.zip`.

In the repo you will find a data folder containing 2 files:
1. `urls.json`
1. `page types - explanation.pdf`

`urls.json` is a json file containing a single array of urls. For almost
each url (some might be missing data) there is a scraped html page in `pages.zip`.
The name of the html file corresponding to a given url is the encoded version of the url `urllib.parse.quote_plus(url)`.
The python library `urllib` was used to encode the urls.

Besides the provided data, there is also a PDF where a set of page types are defined with some extra explanation and an example. As you can see some look very much alike.. Some do not have that much information.. 

**It is your task to try to use unsupervised learning techniques to categorize as many urls as possible into one of these page types.**

Your model should be able to predict the page type of an unseen url - html combination.

You are free to use any additional publicly and legally available data sources to perform this task. 

If you have a question or something else is unclear, please let us know via e-mail. We'll try to respond as fast as possible.

