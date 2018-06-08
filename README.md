# Twitter-Sentiment-Analysis-using-Pig

Twitter Data using R

We will be using “RTweet” package from the GitHub, which is an extension of previously used package TwitteR. Link - https://github.com/mkearney/rtweet

We can install this package using one of these 2 way:
1.	Plain old method, install.packages(“rtweet”)(if any error occurs use “sudo yum install libcurl-devel”)

.	If you face errors in this one than we can use the development built of the package from github itself, now to install a package straight from GitHub we will require an additional package which is devtools(this package allows installation of packages from sources other than CRAN)
a.	Install.packages(“devtools”)
b.	devtools::install_github("mkearney/rtweet")
Once installed we will load the package using library(rtweet), once done we will have to login to our Twitter account and create an app from apps.twitter.com and add the callback url as http://127.0.0.1:1410, after this we need to get our Consumer Key and Token.

After that we will call this method:
twitter_tokens <- create_token(app = "xxxxx",
                               consumer_key = "yyyyy", 
                               consumer_secret = "zzzzzzzz")
Here xxxx is app name that you provided in Twitter app and its case sentitive so be careful, yyy and zzz are the consumer key and consumer secret of the created app. 
