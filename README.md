# Taiwan's Allies

Click <a href="https://colvap.github.io/project-3/">here</a> to have a look!

## Aims
This project was an attempt to see how far I could go if I was ambitious. Projects 1 and 2 of the Lede Program were small in scale, so I wanted to see if I could answer a big question: how much aid does Taiwan give its remaining allies each year, and how does this compare to the aid China gives? 

The process would involve some investigation, and (at the start of the project) I hoped to use it to learn Adobe Illustrator, scrollama, and a little bit of mapping. 

## Findings
Each nation collated their data in a different manner, making standardization challenging, while Tuvalu only had forecasts for some years (liable to differ from actual funds received), and Palau's data proved impossible to sort through - the only figure I could find for how much aid they are given was in one article in the Guardian from 2018, with no source attributed. Both Tuvalu and Palau's government's should therefore be contacted for more concrete answers.

## Collection
To give the project some parameters, I decided to focus on Taiwan's allies in the Pacific islands - a manageable number (four), with some recent islands switching sides to allow for comparisons. These islands tend to be transparent in their budgets, so it would make for an easy start. If all went well, this could be a good base to build on for regions where data could be harder to obtain. 

With a simple google search of 'inurl' and 'filetype:pdf', I was able to extract PDFs of each country's budget records for the past ten years. I've put all of these in the 'pdfs' folder above. I then went through manually to spot Taiwan's (or the PRC's) rate each year. 

## Analysis
The spreadsheets were converted to CSV and parsed with pandas, then turned into a line chart in Flourish, converted to animate on ai2html, and then added to a scrollama animation.

## How did I grow?
One plus that came out of a dead end, was learning how to use Camelot, for tables from Palau's PDFs - the text was unselectable, the tables had no grid lines, with rows that did not align with each other and columns that did not match up across multiple pages. However I was able to get one table of data cleaned and polished using Camelot. 

## What would I have liked to have done?
I looked at Palau's data and wept. They collate the aid given them by Taiwan in the form of the work projects funded by them, listing ongoing work projects by quarter, with no indication of when the money was first issued - sifting through 40 PDFs for this information, project code by project code, was too much for available time and resources. If done properly, it would take a team.

I would have loved to use MapBox or Flourish to place each island on an interactive map, to show the reader where each island is.

I would have liked to do more analysis: how does aid correlate to GDP of each country? Why does Tuvalu get less than the others, Nauru more? 

As I said at the start, this is one piece of a much bigger puzzle. Taiwan currently has 13 allies - I was looking at just four. 