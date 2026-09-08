Customer Support Ticket Analyzer

Python Fundamentals -

Project Title:

Customer Support Ticket Analyzer

Problem Statement

Support teams deal with a large number of tickets every day, and going through all of them by hand to spot

patterns or problem areas takes a lot of time. This project builds a small Python program that stores ticket

data, cleans up the free-text issue descriptions, and pulls out a few useful insights - things like how many 

tickets are high priority, which words show up most often,and which complaint is the longest.

What This Project Does

The program works through five steps, one after another:

●Loads 10 sample tickets (ticket number, customer name, issue description, priority) into a dictionary of lists.

●Lets you add more tickets by typing them in - it asks how many, then collects the details for each one and keeps

the ticket numbers going up in order.

●Cleans up the issue descriptions: strips out punctuation, fixes extra spacing, makes everything lowercase, and 

swaps a few shorthand words (like "ok" to "okay

●Searches the cleaned text for keywords such as "poor", "good", "slow" and "excellent", and counts how many tickets

mention each one.

●Puts together a final summary - priority breakdown, the longest complaint, and the full list of unique words used 

across all tickets.

Files in This Repository

●ticket_analyzer.py - the Python script with all five steps.

●Customer_Support_Ticket_Analyzer.ipynb - the same project as a Google Colab / Jupyter notebook.

●README.md / README.docx - this file.

How to Run It

Option 1: Google Colab

Upload Customer_Support_Ticket_Analyzer.ipynb to Google Colab (or open it from Google Drive) 

and run the cells from top to bottom. The cell for adding new tickets is commented out by default

since it needs keyboard input - uncomment it if you want to try adding a ticket yourself.

Option 2: Plain Python

Run the script from a terminal:

python ticket_analyzer.py

It will print the ticket data at each stage (before cleaning, after cleaning, and the 

final summary).

Sample Output:

Using the 10 preloaded tickets, the analysis comes out to:

●Priority split: 4 High, 3 Medium, 3 Low.

●Longest issue description: ticket 2 (Meera) - "slow response very poor service", 5 words.

●30 unique words used across all the cleaned issue descriptions.

Final Summary and Insights


Out of the 10 tickets, 4 come in as High priority, which is the largest single group - so urgent issues make up

a good chunk of what support has to deal with. Looking at the keyword counts, both positive words (good, excellent) 
 
and negative ones (poor, slow) turn up, so the overall sentiment in this sample is mixed rather than clearly good or bad.

The longest complaint belongs to Meera's ticket, and it also happens to lean negative ("slow response,very poor service"),

which suggests that longer, more detailed complaints might be worth reviewing first since they often carry more specific problems. 

The 30 unique words pulled from the cleaned text give a decent snapshot of the recurring themes - words like slow, poor, good, service 

and support show up often enough that they could be used later to auto-tag or categorize new tickets as they come in.

A few ways this could be extended: a bigger slang/shorthand dictionary, a proper sentiment score instead of just keyword counts, and

tracking how long each ticket took to resolve so that could be compared against its priority level.
