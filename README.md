# Assignment 2: Protests
In recent years the United States has experienced a surge of protests, in support of Black Lives Matter, gender equity, and many other social or political issues.

In this assignment, you will work with data from [Count Love](https://countlove.org/), data that is occasionally [cited](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html) by the _New York Times_ when reporting on US demonstrations.

Through this assignment, you will be able to answer questions about protests, including:

* What were the most attended and least attended protests in the US in the last 5 years?
* How many protests occurred in Washington state?
* How did the number of protests in 2019 compare to 2020, and why?
* Why are people protesting in the US? What are the biggest motivators?

## Learning objectives
By completing the assignment, you will develop or skills for:

- **Version control** tools for managing code (git and GitHub)
- Writing documents with **markdown** syntax
- Coding in R
- Thinking critcally about data.

# 1. Critical Analysis & Reflection: Before You Code

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — that is, knowledge about the topic of the dataset. Sometimes the topic is very narrow; more often it is expansive, as in the case of CountLove. We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it. To get more familiar, we are going to begin by doing some background reading.

**Note:** Please write your answers below under the heading "Your Responses and Reflections."

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm).  **(R1a)** Based on the information in these pieces, why did the creators start collecting the CountLove data?

- Next, we would like you to read this [New York Times piece that uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) and that describes the Black Lives Matter protests that occurred in the summer of 2020. **(R1b)** Please summarize the main point or argument of this article.

Next, we're going to reflect about who collected this data, and what's actually inside it.

**(R1c)** Who collected and shared the CountLove data, and what do they do for a living?

**(R1d)** As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude?

**(R1e)** How and where does CountLove get their data about the protests?

**(R1f)** How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation?

**(R1g)** What are two central values of Count Love? Name and briefly describe them. (See the Envisioning Cards for a definition of "value".)

**(R1h)** Name and briefly describe one direct stakeholder and one indirect stakeholder (See the Envisioning Cards)?

# 2. Coding in R: Parts 1-6
**Instructions**. Assignment instructions and prompts are in this file: [analysis.R](analysis.R).

**Coding and reflection prompts**. You will find two kinds of prompts in [analysis.R](analysis.R):

* *Coding prompts*, which prompt you to write R code in [analysis.R](analysis.R).
* *Reflection prompts*, which prompt you to think and write in English below, in this file (README.md).

**Formatting Your Responses and Reflections**.

* When formatting your written responses and reflections below, please *retain* all
reflection prompt IDs (e.g., R1a, R2a, etc.).
* Fill in the ellipses (...) with your own words.
* Remove expected word counts.
* To write clearly, use markdown code appropriately (e.g., **bold**, _italics_, and `code`). As appropriate, include images, links, and so forth.

**Questions?** As always, please post on Teams or ask your Instructor or Teaching Assistant.

:computer: Good coding!
   :writing_hand: Good critical thinking!
      :smile: Good-luck!

(_Updated: October 2022, Your Teaching Team_)

# 3. Critical Analysis & Reflection: After You Code

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

**(R1h)** How does the CountLove project embody one or more of these 4 forms of challenging power?

**(R1i)** What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)

**(R1j)** What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

## Your Responses and Reflections

### Critical Analysis & Reflection: Before You Code (questions above)

* **(R1a)**
The creators of CountLove wanted to make protest data more accessible for everybody, from citizens to news organizations to politicians to help them make informed decisions in policymaking.

* **(R1b)**
The protests that occurred in the two weeks following George Floyd’s death were as diverse as they were pervasive across the country, signifying a greater collective feeling of outrage about the Black Lives Matter movement than has ever been demonstrated in the nation’s past.

* **(R1c)**
The data collectors are Tommy Leung and Nathan Perkins. Leung is an engineer and Perkins is a neuroscientist. They met at MIT while both studying technology and policy.

* **(R1d)**
Only demonstrations that have had publicity get counted into CountLove’s data. More specifically, demonstrations that show up in news articles online get counted. Even more specifically, online articles that are found by CountLove’s preliminary news crawler get counted.

* **(R1e)**
Leung and Perkins have set up a crawler that takes in large numbers of articles from different news sources, although the details of which news sources are initially viewed is not gone into in depth, and then they have text extractors that pull text from these sources and highlight key facts like where demonstrations took place and how many people were present.

* **(R1f)**
They say that they take the most conservative estimates of how many people attended. This could most commonly result in undercounting, which may be significant, especially since news sources may have initially also been conservative in their reporting.

* **(R1g)**
The CountLove website’s subtitle is a semistatement which ends with a nongrammatical period, which makes it more of a definitive statement or protest in and of itself: *“Protests for a kinder world.”* From this, not two but three values can be gleaned. **Protests** are an important value to the main goal. The main goal, the overarching value, is **kindness**. The desired reach of this value is **globality**, the **whole world**, even though data is taken only from one country.

* **(R1h)**
One direct stakeholder would be any of the protesters who were either counted or not counted by CountLove. An indirect stakeholder might be a police organization whose funding either increased, decreased, stayed the same, or was defunded as a result of the related Defund Police protest movement having impact on policymaking.



### Part 3: Locations (`analysis.R`)
* **(R3a)** The number of protests in Washington doesn’t surprise me too much. I remember seeing the news reports for a lot of them as they were getting media coverage.

* **(R3b)** Yes, I actually do think this is amazing! Languages I’m familiar with, namely Java and Python, don’t have that kind of functionality as far as I know, or don’t have that kind of functionality as prevalently as R does. In those languages, I would need to write a script to iterate any modification or comparison of a list or array over the entire array, probably using a `for()` or `forEach()` loop. ***AHHH-MAZING!***

* **(R3c)** Oops, I already solved one of the issues and pointed out the other one: see comments in code:

  Lines 288-290:
  ```
  # Not all 2-letter state abbreviations originally entered in all caps:
  # `toupper()` fixes this issue in the data only for `states` vector, not for
  # original dataset
  ```
  And lines 296-301:
  ```
  # It appears that some state 2-letter abbreviations have been errantly entered
  # as the wrong two letters. "TE" for example most likely refers to "Tennessee",
  # which should be "TN". I have not corrected for these types of errors. It appears
  # that there are at least 3 of them in the dataset, since the maximum number of
  # unique "states" including "DC" and "PR" for "Puerto Rico" should be 52, unless
  # some 2-letter abbreviations similarly refer to other territories of the US.
  ```

### Critical Analysis & Reflection: After You Code (questions above)
* **(R7h)**
CountLove embodies all these four forms of challenging power:

1.	Counting all the protest data falls under the **Collect** form.

2.	The project embodies the **Analyze** form, partially from the counting process, in which the creators needed to actually read and parse out protest data from the news articles and manually input it into database files, but also in the process of reviewing, aggregating, and displaying the data on the maps and in cartograms.

3.	There is also much **Imagination** in the display of the data, from the maps and cartograms to simply the idea of making the data public so that other sources and journalists could use it to **Imagine** a better future of co-liberation.

4.	The creators **Teach** us how they created CountLove, making not only their data, but also their data-collecting and -wrangling processes public. They also identify themselves.


* **(R7i)**
This may not be the most academic observation in terms of the meat of the analysis, but then again, in terms of the user experience, which is a large part of the website, it might have value. For some reason, I found not just the cartograms or the geographic maps interesting in the [stats](https://countlove.org/statistics.html) section of the website, but the interplay between the two views.

  Similarly to how the states would fade between different shades of blue when the different statistics were selected, which is not as new of a display functionality, and seems fairly simple to code, the states would morph between their geographic shapes and circles between the two modes, which was mesmerizing, partially because I’ve never seen anything exactly like it, although I’ve seen similar displays, but also because I have enough understanding of the data to see why the states are changing relative sizes and locations. This seems like it would be much more difficult to code since the relative positions of the circles in the cartogram mode are based on some combination of their original geographic positions on the map and their relative sizes so they don’t overlap. Other versions I’ve seen of a cartogram would keep their original geographic positions but reduce the opacity to allow for overlapping circles to be seen in full.


* **(R7j)**
One analysis that would be interesting to do, which I don’t have the time, skills, or processing power to do, would be to display the people involved in protests not as bubbles, not aggregated, but as individual dots. This would be so many dots, and would require zooming capability on the graphics. It might also be better displayed in three dimensions than in two dimensions, stacking the dots, or spheres, maybe, instead of showing them spilling out of their geographic cities of protest. The bubbles viewable currently are centered on their city, but do spill over outside of the city of the protest.
