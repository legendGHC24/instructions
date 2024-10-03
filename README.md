> [!NOTE]
> Welcome and thanks for joining us!
> 
> Attendees can either listen to this workshop OR follow through the steps. We recommend following through the steps before joining the session and sharing your github handle with us beforehand (Setup Step#1) for the best workshop experience.

# Setup
1. Get copilot access
   - Add your GitHub handle to this [Google Sheet](https://docs.google.com/spreadsheets/d/1QqDxL9qk7N_aGFwiMALmyB7PiKMBS3_ZtNNfv4yaKHk/edit?usp=sharing)
2. Get Visual Studio Code
   - https://code.visualstudio.com/download (For Mac users - Go to `About This Mac` to check the processor and download the suitable one)
3. Java
   - Check Java version, open a terminal, and execute cmd `java -version`. If you have Java version >=17, you can skip step 5 directly.  
   - Donwload Java 17 Installer
     - Mac User: https://www.oracle.com/ca-en/java/technologies/downloads/#jdk23-mac, download `x64 DMG Installer` or `M64 DMG Installer` depends on the processor.
     - Windows User: https://www.oracle.com/ca-en/java/technologies/downloads/#jdk23-windows, download `x64 Installer`
   - Follow the prompt, and install Java
4. Maven
   - Download Maven 3.9.9
      - Regardless of whether you are a Mac or Windows user, download the `Binary zip archive` from https://maven.apache.org/download.cgi#files
      - Unzip the archive, and copy the full path to the bin folder 
        - Example: /Users/yuan/apache-maven-3.9.9/bin
      - Mac User
        - a. Open Terminal, execute `env`, and find the environment variable `PATH` value. 
          - Example:  PATH=/Users/yuan/anaconda3/bin
        - b. Now add the full path to the Maven bin folder to the existing `PATH` value, and use `:` to separate paths. 
          - Example: /Users/yuan/anaconda3/bin:Users/yuan/apache-maven-3.9.9/bin
        - c. Open Visual Studio Code
        - d. Press Cmd+Shift+P (or Ctrl+Shift+P) and search for "Preferences: Open User Settings (JSON)". Double click, open `setting.json`
           - e. Add the following code block into the JSON file, replace `PATH` value with your own value
          ```
           "terminal.integrated.env.osx": {
                "PATH": "<updated path value>"
          }
          ```
          Example
          ```
           "terminal.integrated.env.osx": {
                "PATH": "/Users/yuan/anaconda3/bin:/Users/yuan/apache-maven-3.9.9/bin"
          }
          ```
      - Windows User
         - 
          
5. Get Extensions 
   1. Legend - Legend Language Support (parse, compile, execute), published by FINOS.
   2. GitHub Copilot
      - GitHub Copilot Chat will be automatically installed together
6. Check if Legend Extension works
   - Check `output` panel
   - <img width="1174" alt="output" src="https://github.com/user-attachments/assets/bbd99ad3-12bb-4fb1-b951-1cc47f73d381">
   - Open `co2.pure`, code text color should change
   - <img width="328" alt="codecolor" src="https://github.com/user-attachments/assets/a8281ddf-7ad1-4403-be93-e8c738f635cf">
   - Execute the function at the very end of `co2.pure`
   - <img width="737" alt="execute" src="https://github.com/user-attachments/assets/e3b66773-b557-4578-9ea9-9864b924b505">
   - If you see the result, then all set! Congratulations!

8. Sign in
   - Use the GitHub handle you provided in Step 1. Once signed in, you will automatically get access to copilot via organization `legendGHC24`.
9. Clone repo
   - Create a new folder `legendghc24` and clone this repository `git clone https://github.com/legendGHC24/instructions.git` or directly download the zip folder.
   





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
