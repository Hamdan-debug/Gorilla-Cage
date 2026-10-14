# Gorilla-Cage
A minimalist business investment game where Class 9 maths decides who wins.
You are the Gorilla, an investor with ₹50,00,000 of fictional capital. Twelve entrepreneurs enter
the cage, one at a time, each with a pitch, a set of numbers and an asking price. Read their
financials, solve the maths, and decide: Invest, Negotiate, or Reject. Good calls grow your net
worth. Bad ones cost you.
Inspired by Shark Tank and built around the CBSE Grade 9 Mathematics syllabus. The maths is
part of how you play, not an optional quiz. You have to answer each pitch's question before you
can make a decision.
Features
12 fictional business pitches across food, fashion, education, hardware, agritech, logistics,
SaaS and more. Each has its own turnover, expenses, market potential, risk level and
asking price.
Three difficulty tiers. Pitch order is shuffled within each tier every run, so the game stays
replayable and gets harder as you go.
Investment dashboard for every pitch: turnover, expenses, profit, profit margin, market
potential, investment requested, equity offered and implied valuation.
Financial analysis panel showing investment as a percentage of turnover, the estimated
payback period, the probability of success, expected return, and estimated values in the
success and decline scenarios.
Negotiation system. Enter your own amount and equity, watch the implied valuation
update as you type, and get a decision from founders who have fixed, hidden limits.
Outcomes based on evidence. A weighted probability decides between two projected
scenarios, and your decision score depends on whether your choice matched the numbers,
not on luck.
Turnover vs profit scatter graph (coordinate geometry) that plots every business you have
seen this run.
Portfolio screen showing cash, total invested, wins and losses, portfolio value, ROI, and
live statistics on the businesses you have seen.
End screen with final net worth, best and worst investment, maths score, business score
and total score.
High scores saved locally with 
localStorage.
Dark, minimalist interface with a single neon-green accent, tabular figures and responsive
layouts for desktop, tablet and mobile.
Mathematics Covered (CBSE Class 9)
How it appears in the game
Topic
Percentages & Profit/Loss
Linear Equations in Two
Variables
Profit, profit % on expenses, profit margin on turnover, percentage change in turnover
Revenue = 
500x, Expenses = 
200x + 3000: find the minimum number of units needed to
reach a target profit
Statistics
Probability
Mean profit margin, median profit, highest and lowest turnover across businesses
Success and decline probabilities, expected value of an investment
Number Systems
Coordinate Geometry
Working with rupees, lakhs, decimals and rounding
Reading a business's position on the turnover (x) vs profit (y) graph
Key formulas
Profit            
Profit %          
Profit margin     
If you answer wrong, you lose a few points and get the working steps. You can also open a hint
and try again.
= Turnover − Expenses
= (Profit ÷ Expenses) × 100
= (Profit ÷ Turnover) × 100
Implied valuation = Investment ÷ (Equity ÷ 100)
Payback period    
= Investment ÷ (Profit × Equity ÷ 100)
Expected value    
How to Play
= P(success) × success value + P(decline) × decline value
1. Open the game and click Enter the Cage.
2. Study the pitch: the description, the financial dashboard, the analysis pills and the graph.
3. Solve the Math Check to unlock your decision.
4. Choose Invest, Negotiate or Reject.
5. Review the outcome and why the Gorilla judged your call the way it did.
6. Repeat for all 12 pitches, then see your final results.
Scoring
+Correct calculations, investing in businesses with healthy margins, negotiating fair
valuations, diversifying, and choices that match the evidence
−Wrong answers, trying to invest more cash than you have, overpaying for equity, and
putting too much capital into high-risk businesses
Running Locally
No installation, build step or server is needed.
1. Download or clone this repository.
2. Open 
index.html in any modern browser.
That's it. The whole game (HTML, CSS, JavaScript and data) is in one file and runs offline.
git clone https://github.com/<your-username>/gorilla-cage.git
cd gorilla-cage
open index.html        
# macOS
# start index.html     
# Windows
# xdg-open index.html  # Linux
Tech Stack
HTML for structure
CSS for styling (custom properties, grid, responsive layouts)
Vanilla JavaScript for game logic, the financial model, maths generators and scoring
SVG for the logo and the scatter graph
No frameworks, no dependencies
Code structure (inside 
index.html)
1. Utilities and reusable financial formulas (
fin.*)
2. Business pitch data, kept separate from the interface
3. Maths question generators
4. Game state
5. Screens and rendering
6. Decision engine (invest, negotiate, reject) and the shared projection model
7. Scoring
8. High scores (
localStorage, wrapped in try/catch)
Disclaimer
All businesses, founders and financial figures are fictional and exist only for educational
gameplay. Projected values are estimates, not guarantees, and nothing in this game is financial
advice.
License
MIT. Free to use, modify and share for learning.
