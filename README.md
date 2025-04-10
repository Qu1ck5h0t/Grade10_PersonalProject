# Qu1ck5h0t's Grade 10 Personal Project
### Disclaimer: The code in this repository is only given as a record of my past coding experience. While you may use this code in your own projects, I do NOT endorse the use of this code in real money trading nor am I responsible for any resultant losses if you do.
## Context 
IB's Middle Years Programme is a curriculum similar to GCSEs (or middle school in most countries) that students aged between 11-16 take before the infamous diploma programme that I am taking as of time of writing (16-18). In the final year of MYP, students are expected to undertake a personal project in anything that they are interested in, where at the end of the process they'll present the personal projects to other students and parents at an exhibition. 

I've always loved coding and finance, so I decided to combine the two interests for my personal project, which is how I ended up with a trading bot. This took me exactly 7 hours to code from scratch, which is not bad considering that I was a total noob at coding back then (relative to now anyway).
## How it works
The strategy that this bot uses is fairly simple, it's called two sma crossover strategy. To begin, the price of bitcoin over the last 24 hours is received from Kraken's API. From the price data, two simple moving averages are calculated using the formula SMA=(A1+A2+A3+...An)/n for An is equal to the price of an asset at period n, and n being the number of periods. 

While most strategies using SMA's are longer term strategies that use multiple days for SMAs, I had to shorten the time frame to make movements and indicators more noticable for a live audience, so I semi-arbitrarily picked 1 hour and 4 hour time periods for my SMAs. Note that this is not the best idea for day trading due to the fact that SMAs are typically used for eliminating noise in short term movements for long term holding. 

The idea is that when the two SMAs cross over, a signal is sent depending on which SMA would be above the other. If the longer period SMA goes from being below to above the shorter period SMA, the signal would be a bearish (short) signal, and vice versa. Below is an image that demonstrates what it looks like in practise, where the blue line is a given longer period SMA than the red line.

![image](https://github.com/user-attachments/assets/1e12e3da-5496-4ecb-b2e6-89d96bda6e68)

While I would've liked to make the code send signals to a trading API, I was not of legal age to trade at the time of coding this project so I was unable to access any trading APIs that I could connect the script to.

## Final words
This was a pretty fun project and the day of the exhibition was a very memorable day for me, though I'm often given more credit than I actually deserve as this strategy is not a novel strategy by any means, nor am I the first person to code a bot using it. I do not intend to touch this repository as I intend to simply make this an archive reminiscent of my earlier years. I may, however, use this code for my own projects in the future that may or may not be public. I learnt a lot from this experience and I honestly should've uploaded this sooner, but I'm glad I did regardless. Below is the only photo I have from the exhibition, we all had to put our displays together on the day of the exhibition so it looks a bit scuffed (not that it isn't actually scuffed). 
![image](https://github.com/user-attachments/assets/1ea25b22-0e39-4bf7-8559-57d855afb8a2)


