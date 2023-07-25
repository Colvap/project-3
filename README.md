# Taiwan's Allies

Click <a href="https://colvap.github.io/project-3/">here</a> to have a look!

# # Aims
This project was an attempt to see how far I could go if I was ambitious. Projects 1 and 2 of the Lede Program were small in scale, so I wanted to see if I could answer a big question: how much aid does Taiwan give its remaining allies each year, and how does this compare to the aid China gives? 

The process would involve some investigation, and (at the start of the project) I hoped to use it to learn Adobe Illustrator, scrollama, and a little bit of mapping. 

# # Findings
I'm reluctant to say anything conclusively without running the numbers past an expert first. I'm new to national budgets and foreign aid, so am certain I have a few blindspots. There are a few things I'd need to double check, like exchange rates. Each nation collated their data in a different manner, making standardization challenging, while Tuvalu only had forecasts for some years (liable to differ from actual funds received), and Palau's data proved impossible to sort through - the only figure I could find for how much aid they are given was in one article in the Guardian from 2018, with no source attributed. Both Tuvalu and Palau's government's should therefore be contacted for more concrete answers.

Having said all of that, the data suggests the PRC is reluctant to make grants - it can afford to give far more than Taiwan, but on the rare occasions it does give, it gives at equivalent levels to Taiwan. 

# # Collection
To give the project some parameters, I decided to focus on Taiwan's allies in the Pacific islands - a manageable number (four), with some recent islands switching sides to allow for comparisons. These islands tend to be transparent in their budgets, so it would make for an easy start. If all went well, this could be a good base to build on for regions where data could be harder to obtain. 

With a simple google search of 'inurl' and 'filetype:pdf', I was able to extract PDFs of each country's budget records for the past ten years. I've put all of these in the 'pdfs' folder above. I then went through manually, using control f, to spot Taiwan's (or the PRC's) rate each year. The Marshall Islands already uses USD in their reports, but other reports had to be converted to USD - I did this either with exchange rates provided in the reports or with the help of a website collating historical exchange rates, making them out to January 1st each year. These were put in separate excel spreadsheets.

# # Analysis
The spreadsheets were converted to CSV and parsed with pandas, then turned into a line chart in Flourish, converted to animate on ai2html, and then added to a scrollama animation.

# # How did I grow?
This project felt like a failure, built on nothing. I was creating something based on data I didn't trust 100% (and missing the data of one nation), while the numbers didn't seem to tell an interesting story at the end. I had to double back and check the numbers I had created multiple times (and only noticed the prescribed exchange rates in Nauru's reports late in the process). Next time I start a project like this, I would try to save time by being more careful about the factors surrounding the numbers I find - exchange rates, whether these numbers include residual aid rolled over from previous years, to beware of forecasts over actuals.  

One plus that came out of a dead end, was learning how to use Camelot, for tables from Palau's PDFs - the text was unselectable, the tables had no grid lines, with rows that did not align with each other and columns that did not match up across multiple pages. However I was able to get one table of data cleaned and polished using Camelot. 

One solid positive was that I was able to manipulate the dataset in pandas with no problems at all - something that caused me a lot of trouble in Project 1. So solid progress right there. 

I also discovered Flourish for the first time during this Project, and it's an absolute delight. I'm never using Datawrapper again.

This was my first time using Adobe Illustrator, ai2html, and scrollama. Each tool was fiddly, and often broke. Dead ends and doubling back were the norm. But advice to myself:
* Make sure that the two CSSes from different scrollys aren't written the same way. That stops the interactives from working.
* Move any .jpg and .svg up to the main folder
* interactions:svg in Adobe Illustrator
* Multiple stickies? Use multiple numbered scrollys
* Using 'br' can ansure stickies don't overlap when transferring
* A blank p tag at the end of a sticky overlay can ensure the final text goes all the way up the page before the sticky-thing moves
* To get the scrolly interactives to work going back up, you need to create a series of d3.select commands one step before that return it to the way it was at step one, five, etc.


# # What would I have liked to have done?
I looked at Palau's data and wept. They collate the aid given them by Taiwan in the form of the work projects funded by them, listing ongoing work projects by quarter, with no indication of when the money was first issued - sifting through 40 PDFs for this information, work code by work code, was too much for the time and resources available to me. If done properly, it would need several people.

I would have loved to use MapBox or Flourish to place each island on an interactive map, to show the reader where each island is. 

As I said at the start, this is one piece of a much bigger puzzle. Taiwan currently has 13 allies - I was looking at just four. 