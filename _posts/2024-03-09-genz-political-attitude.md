---
layout: post
title: "Is there a growing gender gap of political attitude in Germany?"
date: 2024-03-09 06:00:00 +0100
last_modified_at: 2024-03-17 14:00:00 +0100
commants: false
---
On the blog of [Allen Downey](https://allendowney.com) I recently stumbled upon a [blogpost](https://www.allendowney.com/blog/2024/01/28/is-the-ideology-gap-growing/) about an [article of the Financial Times](https://www.ft.com/content/29fd9b5c-2f35-41bf-9d4c-994db4e12998) which claims that there is a **growing** gap in the political attitude of young man and woman emerging **globally**. This is a strong claim with lots if implications. If it is true.

Allen had a deep look into this claim **for the US** which you can find on his blog [here](https://www.allendowney.com/blog/2024/01/28/is-the-ideology-gap-growing/), [here](https://www.allendowney.com/blog/2024/02/04/political-alignmant-affiliation-and-attitudes/), [here](https://www.allendowney.com/blog/2024/02/11/the-political-gender-gap-is-not-growing/) and [here](https://www.allendowney.com/blog/2024/02/18/the-gender-gap-in-political-beliefs-is-small/). Spoiler: Allen is not able to replicate the results from the Article with multiple methods and datasets for the US.

A couple of month back I had a look into the [German General Social Survey ("ALLBUS")](https://www.gesis.org/en/allbus/allbus-home). The survey is conducted every two years and covers a wide range of topics. Unfortunately only few questions are asked every iteration but one of the questions which is asked regularly is a self report of the political belief on a scale from "left" to "right". While this questions has a lot of problems (e.g. what does "left" mean? is there a bias because of socially expected answers?) it still can give us an indication whetehr the FT claim holds for Germany.

The self reported political attitude is measured on a scale of 1 to 10 where 1 means "left" and 10 means "right". All values 1 to 5 are considered "left" and all values 6 to 10 are considered "right". The difference between the two attitudes is then plotted over time. The result is shown in the following plot:

<p align="center">
  <img alt="img-name" src="/assets/images/ideology_gap_unweighted.png">
</p>

Now lets compare this to the graph shown in the Financial Times article for Germany:

<p align="center">
  <img alt="img-name" src="/assets/images/ideology_gap_ft.png">
  <br>
    <em>Financial Times, https://www.ft.com/content/29fd9b5c-2f35-41bf-9d4c-994db4e12998</em>
</p>

While there is a gap in self reported political atittude between man and woman and this gap grew between 1990 and 2010 the claim of the FT that this gap is growing *recently* is hardly supported by the data.

Unfortunetaly that all I can do here. I do not have access to more or better data but beside that the article does not give us any way of validating the claims made:
- The article claims the data is based on social surveys but it does not provide a exact source according to scientific principles.
- The code of the analysis is not provided and thus can not be replicated.
- The plot is misleading since it *suggests* that man are becoming more conserative. This is not true. Both man and woman report themself to be more *left* leaning over time. If anything woman become more left leaning a little faster.

Hopefully somebody else has a look into data for other countries so we can get a better picture of the situation.

**Code:** [https://github.com/bhundt/PoliticalIdeologyGenZGermany](https://github.com/bhundt/PoliticalIdeologyGenZGermany)