> [!NOTE]
> Welcome and thanks for joining us!
> 
> Attendees can either listen to this workshop OR follow through the steps. We recommend following through the steps before joining the session and sharing your github handle with us beforehand for the best workshop experience.

# Setup
1. Get Visual Studio Code
   - https://code.visualstudio.com/download
   - For Mac users - Go to `About This Mac` to check the processor and download the suitable one
2. Java
   - Check Java version, open a terminal, and execute cmd `java -version`. If you have Java version >=17, you can jump to Step 3 directly.  
   - Download Java 17 Installer
     - Mac User: https://www.oracle.com/ca-en/java/technologies/downloads/#jdk23-mac, download `x64 DMG Installer` or `M64 DMG Installer` depends on the processor.
     - Windows User: https://www.oracle.com/ca-en/java/technologies/downloads/#jdk23-windows, download `x64 Installer`
   - Follow the prompt wizard, and install Java
3. Maven
   - Download Maven 3.9.9
      - Download the `Binary zip archive` from https://maven.apache.org/download.cgi#files
      - Unzip the archive, and copy the full path to the bin folder. Example: /Users/yuan/apache-maven-3.9.9/bin
      - **Mac User**
        - a. Open Terminal, execute `env`, and find the environment variable `PATH` value. 
          - Example:  PATH=/Users/yuan/anaconda3/bin
        - b. Now **append** the maven path to the Maven bin folder to the existing `PATH` value, and use `:` to separate paths. 
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
      - **Windows User**
         - Add the full path to the `bin` folder to the environment variable
         - ![4 - Searching for System Env Vars](https://github.com/user-attachments/assets/bd76489e-6049-43e0-a78a-3ba8d39b7994)
         - ![5 - System Properties](https://github.com/user-attachments/assets/59dea08d-db83-47c1-a7ce-9433a03c2624)
         - ![6 - Existing Env Variables](https://github.com/user-attachments/assets/97dacf1a-60fb-4bfe-8152-89fc65212740)
         - ![7 - Editing Path](https://github.com/user-attachments/assets/b254bb8c-6b1f-46d1-ab71-009fbeb2c629)
4. Restart VSCode 
5. Get Extensions
   Open Visual Studio Code, click `extensions` icon <img width="39" alt="icon" src="https://github.com/user-attachments/assets/9b07ef8f-1e0b-41b5-84b8-f846af64c0ae">
 Search for the following two, 
   Legend - Legend Language Support (parse, compile, execute), published by FINOS.
      - <img width="449" alt="Screen Shot 2024-10-03 at 1 55 20 PM" src="https://github.com/user-attachments/assets/e3242256-3336-4a1f-806f-c98f7145f25b">
   
6. Clone repo
   - Create a new folder `legendghc24` and clone this repository `git clone https://github.com/legendGHC24/instructions.git` or directly download the zip folder.
     
7. Check if Legend Extension works
   - Open `co2.pure`, code text colour should change
   - <img width="328" alt="codecolor" src="https://github.com/user-attachments/assets/a8281ddf-7ad1-4403-be93-e8c738f635cf">
   - Check `output` panel (wait for 2 minutes)
   - <img width="1174" alt="output" src="https://github.com/user-attachments/assets/bbd99ad3-12bb-4fb1-b951-1cc47f73d381">
   - Execute the function at the very end of `co2.pure`
   - <img width="737" alt="execute" src="https://github.com/user-attachments/assets/e3b66773-b557-4578-9ea9-9864b924b505">
   - If you see the result, then you are all set! Congratulations!


# Start the workshop
1. Introduction to Legend
2. Understand the data ([source](https://github.com/owid/co2-data))
   1. `owid-co2-data.csv`: Complete data on CO2 and Greenhouse Gas Emissions by Our World in Data.
   2. `owid-co2-codebook.csv`: A description and source for each column in the data.
3. Basic data modeling
   1. Start with `co2.pure` and Class `co2`
   2. Think of a property you would like to query.
   3. Modify the co2 class to include more properties.
   4. Once everything is compiled, hit `Execute` to see your property fetched.
4. Advanced data modeling
   1. Start with `association_query.pure`, class `country` and `co2Emissions`
   2. Think of a class you would like to add,
   3. Add the new class and new association
   4. Create a query function to fetch more data.
5. Wrap-Up and Conclusion
