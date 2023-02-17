# MyFirstDataAnalysis
I decided to do my first data analysis on Elon Musk's Twitter profile (likes,reposts,views,retweets, etc) I won't be using complex tools or languages. It's just a start for me, so be kind, please 🙏 


All the steps I did and every achivement of this process will be displayed here in this README document

Let's begin?

APIFY PART

First I went to Elon's Twitter account to copy the link (I need it to scrape the data from there)



![167664214286716756](https://user-images.githubusercontent.com/69323411/219675574-618d5bd3-223e-4bc2-9d26-46cab132cdf0.png)



Now I go to Apify which is a web scraper. You don't actually need to download any kind of software : all on website.


#######I know I could use Python for this task, but as I said earlier , I won't be using complex tools or languages######

Apify is not the only option you have if you want to do some web scraping. You may consider another option, I know this one is fast and does everything I need for this task.

Here's the Apify interface. Tasks are called ACTORS and you have a lot of pre-configured ACTORS, like Linkedin and others.

![Firefox_Screenshot_2023-02-17T14-16-12 515Z](https://user-images.githubusercontent.com/69323411/219680011-8f53b93b-49f4-45d6-85b9-774a1adc23ea.png)


If you click on task, you can see it's parameters

![Firefox_Screenshot_2023-02-17T14-23-21 459Z](https://user-images.githubusercontent.com/69323411/219680912-a8e4229b-a892-48fc-842c-37709091ba02.png)

You have several tabs 


![Firefox_Screenshot_2023-02-17T14-30-53 846Z](https://user-images.githubusercontent.com/69323411/219682993-8df4ef19-197d-40da-a43e-6005cdf75f5b.png)

And of course you can export all of data you scraped. I will download the CSV format, because I'll upload it later to Google Sheets for cleaning

![Firefox_Screenshot_2023-02-17T14-32-00 882Z](https://user-images.githubusercontent.com/69323411/219683434-9c332387-e02d-4505-8ada-efa3b6c0a149.png)

When you open the downloaded CSV file, it looks like crap. There are a lot of columns we don't need, a lot of information we won't analyze.

Just look at this 😔

![ezgif-2-bd30aed728](https://user-images.githubusercontent.com/69323411/219696173-2e008b38-0bb3-4fe6-bdee-722af0a3a005.gif)

GOOGLE SHEETS PART

Why not clean it and delete all unecessary columns?

![Firefox_Screenshot_2023-02-17T15-32-02 058Z(1)](https://user-images.githubusercontent.com/69323411/219697476-3c909bcd-a69d-41c8-ba8a-31eaec901bbb.png)

I think it looks better 🤌🏻

We did all the cleaning stuff

Now it's time to start our analysis work

![thinking-math](https://user-images.githubusercontent.com/69323411/219698117-ef10a877-a0ef-4aad-92c0-5cd26060bb23.gif)

FYI I pulled more than 1000 rows from Twitter with Apify, but now I have only 246 rows-tweets.
Why?
Because there were rows with NULL values or with 0 values. We don't need them. So we will work with these 246 rows.

![giphy](https://user-images.githubusercontent.com/69323411/219723376-a7b1e297-5269-4913-a247-3f5011ff8ec9.gif)

Let's imagine that I have a very kind boss who asks me to perform some basic calculations on these rows.
![giphy](https://user-images.githubusercontent.com/69323411/219727618-f9287e13-5032-48d4-9dc8-a81fc1e99fb7.gif)



❓He wants to know how many people added Elon's LAST 246 tweets to FAVORITES ❓

❓How many views he had over these tweets ❓

❓How many times he mentioned someone in his tweets ❓

❓How many tweets there are with a media file with a photo or image❓

For the first 2 questions we can use the SUM function in Sheets that will do the addition of all values in selected column.

ANSWER TO QUESTION 1 --> ❓He wants to know how many people added Elon's LAST 246 tweets to FAVORITES ❓

![Firefox_Screenshot_2023-02-17T18-02-46 719Z](https://user-images.githubusercontent.com/69323411/219741505-87ecf2db-c9ee-44e8-a171-bb0a0bf7ef59.png)

The result

![Firefox_Screenshot_2023-02-17T18-05-21 178Z](https://user-images.githubusercontent.com/69323411/219742338-7f89db64-2745-4aec-a562-753de5fabfa3.png)


But it's kinda hard to read this number. We will format it to "number". You'll see the difference


![Firefox_Screenshot_2023-02-17T18-08-36 082Z](https://user-images.githubusercontent.com/69323411/219743500-c3505247-2d01-4bce-801d-da4cc65b018a.png)

Voilà

![Firefox_Screenshot_2023-02-17T18-09-39 779Z](https://user-images.githubusercontent.com/69323411/219743992-678a695f-a1ec-430d-b9bb-390911765e70.png)


❗ 55,333,033 people added Elon's last 246 tweets to FAVORITE ❗


ANSWER TO QUESTION 2 --> ❓How many views he had over these tweets ❓


We will do the same as we did on the first question

We will jump directly to the answer, because it's the same solution as in the first question

![Firefox_Screenshot_2023-02-17T18-18-06 591Z](https://user-images.githubusercontent.com/69323411/219747570-70067fc2-3869-42d2-bf9b-d402f97e346c.png)









