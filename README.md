> [!NOTE]
> Welcome and thanks for joining us!
> 
> Attendees can either listen to this workshop OR follow through the steps. We recommend following through the steps before joining the session and sharing your github handle with us beforehand (Setup Step#1) for the best workshop experience.

# Setup
1. Get copilot access
   - Add your GitHub handle to this [Google Sheet](https://docs.google.com/spreadsheets/d/1QqDxL9qk7N_aGFwiMALmyB7PiKMBS3_ZtNNfv4yaKHk/edit?usp=sharing)
2. Get Visual Studio Code
   - https://code.visualstudio.com/download (For Mac users - Go to `About This Mac` to check the processor and download the suitable one)
   - x64 Installer	153.92 MB	
https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe ( sha256)
3. Get Extensions 
   1. Legend - Legend Language Support (parse, compile, execute), published by FINOS.
      Make sure you have Java version >= 17 installed. If not, go [here] https://www.oracle.com/java/technologies/downloads/ and download.
      For Windows, choose x64 Installer	153.92 MB	
                     https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe ( sha256), Restart your vscode after installation is done
      Maven Installation - https://maven.apache.org/download.cgi 
   3. GitHub Copilot
4. Sign in
   - Use the GitHub handle you provided in Step 1. Once signed in, you will automatically get access to copilot via organization `legendGHC24`.
5. Clone repo
   - Create a new folder `legendghc24` and clone this repository
6. Make sure `co2.pure` file gets parsed by Legend Compiler (meaning, the colour of code changes and code lens commands are visible)

# Start the workshop
1. Introduction to Legend
2. Understand the data ([source](https://github.com/owid/co2-data))
   1. `owid-co2-data.csv`: Complete data on CO2 and Greenhouse Gas Emissions by Our World in Data.
   2. `owid-co2-codebook.csv`: A description and source for each column in the data.
3. Basic data modeling
   1. Start with `co2.pure` and Class `co2`
   2. Think of a property you would like to query.
   3. Modify the co2 class to include more properties, take the help of GitHub Copilot.
   4. Once everything compiled, hit `Execute` to see your property fetched.
4. Advanced data modeling
   1. Start with `association_query.pure`, class `country` and `co2Emissions`
   2. Think of a class you would like to add,
   3. Add the new class and new association, take the help of GitHub Copilot.
   4. Create query function to fetch the more data.
5. Wrap-Up and Connclusion
