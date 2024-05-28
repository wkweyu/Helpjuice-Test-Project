# Helpjuice-Test-Project
Helpjuice Test Project
Helpjuice Full-Stack (Rails & Vanilla JS) Internship Test

The fact that you’re reading this tells us one thing about you: you’re absolutely amazing and we want to hire you.

This internship (non-paid) test is designed to allow us to better understand you as a developer. 

Please send test project to:
menna.adel@helpjuice.com
emil@helpjuice.com 
legal@helpjuice.com 

How will we evaluate you? 
We’ll evaluate you by these 4 items. Each is very important, and we provide an outline below
How quickly you deliver it. 
How well tested your code is 
Your code quality 
Your communication 
Completeness

Standards for Success
No plagiarism and the idea is yours (you didn’t just piggy back off someone) ?
Code is clean?
Live link deployed?
Done in timeline requested?
App works using the examples provided 
Doesn’t have any major flaws (ux/ui/bugs) 
Due date:
We expect this project to be submitted in under 48 hours from us sending it to you by the latest.  The sooner the better. 
Standards:
TEST. Your. App.
GOOD Code. We can’t stress this enough. 
Documented code. We don’t expect you to write a novel, but at least remove the default Rails README
Scalability 
Deploy on Heroku or w/e for easier testing. Remember, it’s all about making the user’s life easier (in this case, us -- reviewing your code)


Task Description:
To create a realtime search box, where users search articles, and then to have analytics that display what users were searching for. You can also track via IP - no need to create a devise, etc.

Your goal is to record their input in realtime and ultimately display analytics & trends on what people are searching for the most. (this is not about search itself, but really about analytics behind it). 

It’s per user - so don't blend other users data

Don’t worry too much about populating it with articles, we only really care about the search, and search analytics. We don’t care how good your search engine is, but rather how good your algorithm for figuring out what people searched for. Search should be instant, and every search should be logged, regardless of what they type, but you should capture and summarize the searches so you dont have the ‘pyramid problem’
 
Hint: Because the search is real time, queries will be coming in segments, as listed in the example below

Bonus: You should expect thousands of requests per hour, so think of scalability. 
Bonus: Test your app with Rspec.

Example input <--> output
Belows are the input/output good & bad examples. 
If we test your app, and it behaves in a bad example, we won't hire you.  
Keep in mind that some users type slowly, but some users type. It's up to you to engineer around that -- your solution should be fail proof.
It should be instant search & results though.   
Better to over-engineer than to be lazy-engineer. Most importantly is to finish in the timeframe and fast. 

Good example

	User searches (because it’s instant it records it all):

(1st (random) user searches for)
What is 
What is a 
What is a good car  

(2nd (random) user searches for:)
How is
How is emil hajric 
How is emil hajric doing 

Your search engine only records: 
What is a good car
How is emil hajric doing 
(And removes the rest because it was an incomplete search )


BAD example (aka pyramid problem) 

	User searches (because it’s instant it records it all):
Hello
Hello world
Hello world how are you?

Your search engine only records: 
Hello 
Hello world
Hello world how are you?
(you didn’t filter what the user searched for)



Bonus points:
Stylize your app. We don't require you to write the CSS yourself, but if you do it we can evaluate your front-end skills and that's an extra;
Complete it quickly
Have amazing tests 
IT WORKS IN SCALE - meaning it can handle a lot of requests
Communicate to Emil & the rest of the team in a professional manner once done.


