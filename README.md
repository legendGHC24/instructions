

# Getting started

Attendees of the workshop can either listen in to this workshop, OR follow through the steps. We recommend following through the steps before joining the session and sharing your github handle with us beforehand (Setup Step#1) for the best workshop experience.

# Setup
1. Get copilot access - Add your github handle to this page: https://docs.google.com/spreadsheets/d/1QqDxL9qk7N_aGFwiMALmyB7PiKMBS3_ZtNNfv4yaKHk/edit?usp=sharing
2. Get VSCode - https://code.visualstudio.com/download
   For Mac - Go to About this mac - check your chip. For me, it was Apple Chip and I downloaded .zip in a new folder called "legendghc24". Double clicked to finally get VSCode started.   
3. Go to Extensions in VSCode, search and install following:
      (i)  Legend under FINOS - Legend Language Support (parse, compile, execute)
      (ii) Github Copilot - Install and sign in to your github. Sign in with the github handle you provided in Step 1. Once signed in, you will automatically get access to copilot via organisation legendGHC24.
4. Make sure versions of following are correct -
     (i) Java - version > 17. https://www.java.com/en/download/ 
5. Clone this repository in the same folder "legendghc24" - https://github.com/legendGHC24/instructions.git
6. Make sure that co2_ducdb.pure file is getting parsed by Legend Compiler (meaning, the color of code changes and code lens commands are visible)

# Start with workshop!

1. Elaborate on CO2 dataset - https://github.com/owid/co2-data 
2. Download 
3. Set the problem - Contextual Queries need to be done (what's the emmisions of US in the year 2024) without having the data consumers to worry about the physical table and where and how it is stored. (what's the EmmissionXYZ12o, em1234 from "CO2")? Super abstract, conflicting columns names which is true for real business use cases as well. Real data is messy. 
4. Think of a query to do. Few examples to start with -
   (i) Give me all countries in this data
   (ii) write a Finos Legend query to fetch all unique countries in this data
   (iii) Update the model with one more column for co2-growth_pct
   (iv) Think creatively of classes to create for all 80 columns. 
   (v) Update the pure model to have more classes with association. 
   (vi) Create a join query finally. 
5. Use Copilot to showcase how data modelling with Legend is useful. 
   What is a data model (use #file co2_duckdb.pure)? Why data modelling? Complicated business use cases? 
   #file: .csv
6. Explanation of Legend concepts in co2_duckdb.pure. Users select the code snippets and ask Copilot Chat - "#selection explain this" 
7. Close our workshop with explaining how real business use cases can get really complex.  
   Uniform mapped graph for the entire product. 
   More transparent
   better understanding for badly named columns
