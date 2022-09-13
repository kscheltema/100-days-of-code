# 100 Days Of Code - Log

### Day 1: June 27, 2022 

**Today's Progress:** Finding out what Firebase guides are depreciated. I went for my third development related interview, getting more used to the terms used. 

**Thoughts:** Good YouTubers and course publishers should remove depreciated guides. Since the time wasted trying to learn depreciated code, or nitpicking depreciated from not. Is like putting on a blindfold and looking for a needle. 

**Link to work:** This is Firebase stuff, so best not public as a whole. So will place the edits. 

+import { getFirestore } from "firebase/firestore";
...
+const fireStoreDB = getFirestore(firebaseApp);
...
export {
...
 +fireStoreDB,
 
 added & removed due to depreciated guide:
y/index.html(the file)

### Day 2: June 28, 2022 
**Today's Progress:** I got a return on a console.log from firestore

**Thoughts:** credit to (CRUD Tutorial Using React + Firebase | Firebase 9 and Firestore Tutorial), I am having difficulty remembering how and where to apply key. 

**Link to work:** The commits was trashed, so redit yesterdays commits. 
... I played around with styling based on this Page Component. I saw bugs so removed the code and made a not for a new branch. 
see screenshot in my tweet @KobusScheltema

import * as React from "react";

import { firestoreDB } from "../firebase-config";

import { collection, getDocs } from "@firebase/firestore";

const BlogDetail = () => {

  const [blogItem, setBlogItem] = React.useState([]);
  
  const blogListRef = collection(firestoreDB, "blog_list");
  

  React.useEffect(() => {
    const getBlogItem = async () => {
    
      const dataFB = await getDocs(blogListRef);
      
      console.log("This is Firebase", dataFB);
      
    };

    getBlogItem();
  }, [blogListRef]);
  
  return <div></div>;
  };

### Day 3: June 29, 2022 
**Today's Progress:** Not much is made in terms of progress. Integrating an example to work within existing code-base is the problem. useState has been partially successfully replaced with Redux. the set part of useState is the problem. Since this is not hardcoded but expected to be received from the user. 
**Thoughts:** the working codebase file, is to be shelved, and replaced with a pseudo code base for the relevant file working from a different example. 
**Link to work:** see screenshot in my tweet @KobusScheltema

### Day 4: June 30, 2022 
**Today's Progress:** Based on a guide I redesigned my BlogList and recreated BlogDetail page with all data being retrived from the FireStore.
**Thoughts:** Design probably not the best the function exists, Need to redesign BlogCreate and run anoter test post. 
**Link to work:** see screenshot in my tweet @KobusScheltema

### Day 5: July 1, 2022 
**Today's Progress:** Some CSS victories: Had a a background distorted before now seperate color properties no distortion, rendering images some not suitable with map function and TypeScript happy about it. 
**Thoughts:** Redesigning existing work feels like 2 steps back 1 step forward. 
**Link to work:** see screenshot in my tweet @KobusScheltema


### Day 6: July 2, 2022 
**Today's Progress:** I fixed the icons they all have no background now. Download button moved.
**Thoughts:** Not much done today ;(
**Link to work:**  see screenshot in my tweet @KobusScheltema

### Day 7: July 3, 2022 
**Today's Progress:** More refactor items complete and the impacts managed on the header. Header, Footer and LogoContainer has conditional css based on screen sizes. 
**Thoughts:** Need to work on rendering a singular Blog Item.
**Link to work:**  see screenshot in my tweet @KobusScheltema

### Day 8: July 4, 2022 
**Today's Progress:** Footer, Header and some pages tested for SX, SM, MD and LG. Refactor largely complete, out for comments. 
**Thoughts:** Difficult to make lots of progress with MUI docs is offline. I am in the begining stages of rendering a individual Blog. 
**Link to work:** see screenshot in my tweet @KobusScheltema

### Day 9: July 5, 2022 
**Today's Progress:** Blog Form basics is in place. 
**Thoughts:** I got lost today, and followed a rabit. My mentor helped me back onto the narrow Path. 
**Link to work:** see screenshot in my tweet @KobusScheltema

### Day 10: July 6, 2022 
**Today's Progress:** Tab Pannel on Auth refactor in place. Frameworks and Languages height adjusted sligtily for better presentation on various screen sizes.
**Thoughts:** Need to sort out useFormik bugs.
**Link to work:** see screenshot in my tweet @KobusScheltema

### Day 11: July 7, 2022 
**Today's Progress:** Created a new repository for a Count Down Timer. Implemented fixes for bug related to poor usage of Yup. Overhauled the usage of Formik.
**Thoughts:** Sometimes old code is starring at you and your looking at somethikng different. 
**Link to work:** https://github.com/kscheltema/js_timer.git see screenshot in my tweet @KobusScheltema

### Day 12: July 8, 2022 
**Today's Progress:** So the branch blog_post_firestore was merged after clearing errors and warnings. Then I worked on a Forgot Password functionality.
**Thoughts:** Forgot Password functionality is loadable on npm start, but non-responsive bug and a <p> - children warning. I have to clear this error after I found it and then work on the non-responsive bugs. Identifying an creating an example for sendPasswordResetEmail from FireBase needs credit for this YouTube video. https://www.youtube.com/watch?v=XD3e_DDKBww
**Link to work:** see screenshot in my tweet @KobusScheltema

 ### Day 13: July 9, 2022 
 **Today's Progress:** No noteworthy proggress to report.
 **Thoughts:**  Will try a different branch if a solution doesz not present itself.
 **Link to work:** I am trying to locate an source of an error: trying to locate where 
<fieldset> cannot appear as a descendant of <p>.
 Then I went to a different branch where I am faced with since my older code is not accepted in my choosen platform without a warning. 
 Missing radix parameter.
 
  ### Day 14: July 10, 2022 
 **Today's Progress:** time_js conversion simple solution to "Missing Radix Parameter" in ParseInt(what to convert, how many decimals). The <p> tage with children error was found eventually. Forgot Password is tested and email sent to junk. 
 **Thoughts:** Coppying code can lead to errors. Docs is somethimes written for a basic example. Here Firebase docs is better in that they ellude to what should be within something. 
 **Link to work:** https://codesandbox.io/s/confident-cookies-lom50s?file=/src/App.js see screenshot in my tweet @KobusScheltema
 
    ### Day 15: July 11, 2022 
  **Today's Progress:** Completed my 404 page, Got the id from a onClick, for rendering my Detail page from the List.  
  **Thoughts:** I tried props, Max and YouTube based on Max I should load my data with my ID as reference from my server. Doing this is my new challenge. 
  **Link to work:** see screenshot in my tweet @KobusScheltema; React - The Complete Guide (incl Hooks, React Router, Redux): video 290
 
    ### Day 16: July 12, 2022 
  **Today's Progress:** I was able to fetch a single doc from the FireStore.
  **Thoughts:** (JS filter,find) not a good plan its FireStore thus FireStore functions. The Net Ninja was helpful in the "Getting Started with Firebase 9 #9 - Fetching a Single Document" video https://www.youtube.com/watch?v=lZzd8zurolg
 Need to transform this Object into an Array, difficult to access or manage atm. 

  **Link to work:**  see screenshot in my tweet @KobusScheltema

     ### Day 17: July 13, 2022 
 **Today's Progress:** The different ways to not access known items within a Object. Some Minor CSS for different screen sizes. Active Styling working with no bugs possibly dirty coding. Error and Loading state conditionally implemented on the List Card item and the Detail Card Item. 
 **Thoughts:** Today with help from my Mentor Gary. I stopped trying to independantly save values from a Object and accessing them directly. Lots of CSS. Need my Mentor to review the active styling and possibly propose alternatives. Need to test the List and Detail for various screen sizes, and Body lengths. As always if you know where to find it Max is a great fallback. 
 **Link to work:** see screenshot in my tweet @KobusScheltema; React - The Complete Guide (incl Hooks, React Router, Redux): video 218 - Handling Errors
 
 ### Day 18: July 14, 2022 
 **Today's Progress:** Active Styling bug found and code adjusted. Single Date is recieved from FireStore, converted with toLocaleDatestring inside a useEffect otherwise promise bug. 
 **Thoughts:** Not much was done. A List Dates needs to be converted from the FireStore, current bug no change or change with a console.log.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema;
 
  ### Day 19: July 15, 2022 
 **Today's Progress:** Scoll bug, and related content render over each other was fixed, vertical scroll disabled. Date no more date issues. target="_blank" deployed to open a different page in the browser. 
 **Thoughts:** Struggling to dynamically change the background image for BlogDetail page and change it back when the user moves away. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema;

   ### Day 20: July 16, 2022 
  **Today's Progress:** Conditional styling for BlogDetail page implemented making it vastly different from rest of the Website. 
  **Thoughts:** Still many features to implement in the BlogDetail page to bring it aligned with real life examples. Currently trying to move and display a Hero image when on this page. 
  **Link to work:**  see screenshot(s) in my tweet @KobusScheltema;
 
    ### Day 21: July 17, 2022 
   **Today's Progress:** I accepted that the environment to enter as a Junior Deverloper is not great. So In consultation with my Mentor Gary. I have decided to finish the the-complete-junior-to-senior-web-developer-roadmap. So far I have read a bunch of articles linked to the course, and did up to video 7 so far. 
 https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work
 https://zerotomastery.io/blog/developers-edge-how-to-become-a-senior-developer/
   **Thoughts:** It sucks. Life in general. But I need to move forward. 
   **Link to work:** see screenshot(s) in my tweet @KobusScheltema;

  ### Day 22: July 18, 2022 
 **Today's Progress:** I downloaded and started testing Git Bash. I created a SSH key.
 **Thoughts:** I need to successfully log into the server. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema;
 
 ### Day 23: July 19, 2022 
 **Today's Progress:** I am still testing Git Bash. I was not yet able to log into Digital Ocean from Git Bash.
 **Thoughts:** I need to successfully log into the server. I am Windows and my instructor and mentor is using a Mac.
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema; 
 
  ### Day 24: July 20, 2022 
 **Today's Progress:** I am still testing Git Bash. I was able to add my Identity. I was not yet able to log into Digital Ocean from Git Bash. I started testing PuTTY and was able to generate a key and upload the key to the server. 
 **Thoughts:** I need to successfully log into the server. The error where I am stuck. 
 $ ssh root@{ip address} 
Unable to negotiate with {ip address} port 22: no matching host key type found. Their offer: ssh-rsa,ssh-dss
 With interaction with the server with aid of Twitter, I am required as I understand to do a maiden instalation by the server. This is where I believe my bug lies.  
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema, https://docs.digitalocean.com/products/spaces/quickstart/#upload-and-delete-files https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/to-team/ https://docs.digitalocean.com/products/droplets/how-to/add-ssh-keys/to-existing-droplet/ https://www.chiark.greenend.org.uk/~sgtatham/putty/docs.html
 
   ### Day 25: July 21, 2022 
 **Today's Progress:** I have read and made notes on PuTTy doc Chapter 3 and 4. I was able to upload a repository to Digital Ocean, not tested futher since PuTTY doc not finished. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
    ### Day 26: July 22, 2022 
 **Today's Progress:** I have read and made notes on PuTTy doc Chapter 5 and the last bit of 4. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

     ### Day 27: July 23, 2022 
 **Today's Progress:** I have read and made notes on PuTTy doc Chapter 6 and 7. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
  ### Day 28: July 24, 2022 
  **Today's Progress:** I am finally done reading and making notes on the PuTTY documents, Chapter 8, 9 and 10.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
 ### Day 29: July 25, 2022 
 **Today's Progress:** Having played around with BPuTTY and the Digital Ocean server, the droplet I have see how to not establish a connection. Now everything has to be reestablished. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
  ### Day 30: July 26, 2022 
 **Today's Progress:** A connection to the Digital Ocean server from my computer was established today. Then finished 6 episodes of section 2 in the The Complete Junior to Senior Web Developer Roadmap (2022) course. 
 **Thoughts:** It looks easy enough. Everything to the point of connection is server connection fail or not. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
  ### Day 31: July 27, 2022 
  **Today's Progress:** I have done research on where is best to use which image types in Web Development. My conclusion based on the research was:
•	svg for graphs or diagrams 
•	pdf for display documents 
•	png general web graphics
•	jpeg photos or artwork
  **Thoughts:** I need to put more time into studies in the morning. 
**Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
 ### Day 32: July 28, 2022 
 **Today's Progress:** Worked through some theory on how to reduce images size, while retaining end-user quality. I have created a repository for the first exercise for section 2. 
 **Thoughts:** Having some permission issues that I need to sort out before doing the exercise. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

  ### Day 33: July 29, 2022 
  **Today's Progress:** I have completed the theory on Critical Render Path. I have made some commits to GitHub as examples. 
  **Thoughts:** I broke my GitHub link, another task for tomorrow.
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
  ### Day 34: July 30, 2022 
 **Today's Progress:** I have with some help restored GitHub to display my commits, I have practices Critical Render Path with exercise 3. 
 **Thoughts:** I need to fork a repository and do exercise 4.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
   ### Day 35: July 31, 2022 
  **Today's Progress:** I have cloned a repository num 52 from Udemy course "The Complete Junior to Senior Web Developer Roadmap (2022)"
  **Thoughts:** I have a bug that I need to sort out, this whole not "npm start" is new to me. I need a valid URL to be able to analyse. Possibly have to publish the site on a server?
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

    ### Day 36: August 1, 2022 
  **Today's Progress:** I was able with some help from Net Ninja to set up a Udemy website on GitHub pages. https://www.youtube.com/watch?v=QyFcl_Fba-k "Getting Started with GitHub Pages". Compressing and reducing the size on images on https://tinypng.com/ download time went down from 36.6 seconds to 13.41 seconds. Removed Boostrap requirements loadtime now 12.95 seconds. Removed JQuery loadtime now 10.97 seconds. Compressed other images loadtime now 10.74 seconds.
  **Thoughts:** Squash of css and use of Defer had no clear benefit. Something changed now load time is back on 13.39 Seconds. Solution video next. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

     ### Day 37 August 2, 2022
   **Today's Progress:** Today I finised up until section 4: 65. In that I have practised forking and cloning a repository. I also used GitHub Pages successfully again. 
   **Thoughts:** There is a Error on the {npm install}, will troubleshoot tomorrow. 
   **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

 ### Day 38 August 3, 2022
 **Today's Progress:** Today I finised up until section 4: 79.
 **Thoughts:** Would love to work on a challendge. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
  ### Day 39 August 4, 2022
 **Today's Progress:** Today I finised up until section 4: 93. Today I successfully updated React 16 to the latest version of 18.
 **Thoughts:** So I more aggressively started to code along, made some essentail notes for React. I need to update my code to not be class based. A Error from the latest video i need to pindown. I did do some googleing and troubleshooting. Will seek some different channels for advice tomorrow. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

   ### Day 40 August 5, 2022.
  **Today's Progress:** My update yesterday wasnt minor thus I had to remove node_modules and package-lock.json. I have done these now and also updated React Scripts. I rolled back the attempts to update class based component for Error Boundary.  
  **Thoughts:** ErrorBoundary requires Class based compoents that works in React 18. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
    ### Day 41 August 6, 2022.
   **Today's Progress:** I updated npm modules on my computer. 
   **Thoughts:** The App is now running without warnings or errors, after a restart as well. 
   **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
     ### Day 42 August 7, 2022.
   **Today's Progress:** I was unsuccessful to complete lecture 95 deploying of the App.
   **Thoughts:** The error remains. 
 PS G:\docs\github\section_4_robofriends> npm run deploy
npm WARN config global `--global`, `--local` are deprecated. Use `--location=global` instead.

> robofriends@0.1.0 predeploy
> npm run build

node:internal/modules/cjs/loader:936
  throw err;
  ^

Error: Cannot find module 'G:\node_modules\npm\bin\npm-cli.js'
    at Function.Module._resolveFilename (node:internal/modules/cjs/loader:933:15)
    at Function.Module._load (node:internal/modules/cjs/loader:778:27)
    at node:internal/main/run_main_module:17:47 {
  code: 'MODULE_NOT_FOUND',
  requireStack: []
   **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
 ### Day 43 August 8, 2022.
 **Today's Progress:** I am still unable to complete lecture 95. The only advice that I got from a friend is that GitHub must run from the C-drive, I am having long term problems with said C-drive and the move to the G-drive wa\s part of the fix.  
 **Thoughts:** To continue the Study process I can either work on a different project or Study with Free-Code-Camp. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

  ### Day 44 August 9, 2022.
  **Today's Progress:** Today I studied python opperators, if and else, the power of indenting, and other basics of python.
  **Thoughts:** 13% in 1.1 days would hopefully mean that I would be done within two weeks. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
   ### Day 45 August 10, 2022.
  **Today's Progress:** Today I studied python loop operators and various related key words.
  **Thoughts:** 27% in 2.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
    ### Day 46 August 11, 2022.
  **Today's Progress:** Today I studied python string and open related functions.
  **Thoughts:** 34% in 3.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
     ### Day 47 August 12, 2022.
  **Today's Progress:** Today I studied python Data Structures, Tuples and Regular Expressions.
  **Thoughts:** 48% in 4.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
      ### Day 48 August 13, 2022.
  **Today's Progress:** Today I studied more Regular Expressions and application protocol with Python.
  **Thoughts:** 61% in 5.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
       ### Day 49 August 14, 2022.
  **Today's Progress:** Today I studied the different ways that Python integrates with the web.
  **Thoughts:** 70% in 6.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
        ### Day 50 August 15, 2022.
  **Today's Progress:** Today I studied classes and the related objects in Python.
  **Thoughts:** 82% in 7.1 days would hopefully mean that I would be done within two weeks or less. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
         ### Day 51 August 16, 2022.
  **Today's Progress:** I practised for interviews.
  **Thoughts:** I Forgot some of my JavaScript
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
          ### Day 52 August 17, 2022.
  **Today's Progress:** I practised for interviews, and did some interview tests.
  **Thoughts:** I Forgot some of my JavaScript, I will now do some JavaScript everyday, need to find alternative for FreeCodeCamp. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
           ### Day 53 August 18, 2022.
  **Today's Progress:** I went through some JavaScript Algorithms and Data Structures - Basic Algorithm Scripting in Free Code Camp. 
  **Thoughts:** I tried to carry on with the Python Course there was a problem with the instalation. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

         ### Day 54 August 19, 2022.
  **Today's Progress:** Today I used map and find in JavaScript fCC to use a function recieved in a parameter to find a match or not from an array. Then I carried on with the Python Course. 
  **Thoughts:** 84% in 8 days would hopefully mean that I would be done within two weeks or less with the Python Course. 
  **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
### Day 55 August 20, 2022.
 **Today's Progress:** Today I used map, split, join, uppercase, char and lowercase in JavaScript fCC to capitalise the first letter of each word, check if a variable is Boolean.
 **Thoughts:**  Then I tried in vain to carry on with the Python Course. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
 ### Day 56 August 21, 2022.
 **Today's Progress:** Today I used splice to insert an array within an array, and used a filter and Boolean to remove falsy values.
 **Thoughts:**  I need to resume the Python Course, using a newly found guide. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema..
 
  ### Day 57 August 22, 2022.
 **Today's Progress:** Got some help to setup SQlite. I with FFC made a function that takes an Array and using a number finds one index smaller. Then suggest to use one index larger. 
 **Thoughts:**  I need to resume the Python Course, the lecturer is using a DataBase browser. Need to investigate that. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

   ### Day 58 August 23, 2022.
 **Today's Progress:** I with FFC made a function that checks if all characters of a parameter can be found in another parameter. The second challendge An array was sliced according to the provided size and then storred in an array. 
 **Thoughts:**  I need to figure out DataBase Browser. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
    ### Day 59 August 24, 2022.
 **Today's Progress:** With fCC i made objects and accessed them, use this with objects. In the Python course I used CRUD functions in a SQlite database with DataBase Browser. 
 **Thoughts:**  I am Tired. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

     ### Day 60 August 25, 2022.
 **Today's Progress:** With fCC i made objects with properties and accessed them. In the Python course I did an introduction to Relational Databases and Relationship Building
 **Thoughts:** I didnt spend that much time on studies today, too much real life interferance.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
      ### Day 61 August 26, 2022.
 **Today's Progress:** With fCC i utilised objects with properties. In the Python course I did some Relational Databases and Relationship Building
 **Thoughts:** Doesnt always feel like there is progress. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
       ### Day 62 August 27, 2022.
 **Today's Progress:** With fCC i utilised objects with functions. In the Python I finished it. 
 **Thoughts:** On to the next language to study. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
        ### Day 63 August 28, 2022.
 **Today's Progress:** I did some preparations for the Python practical.  
 **Thoughts:** On to the next language to study, after the Python assesment.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
         ### Day 64 August 29, 2022.
 **Today's Progress:** I installed python v3, and read through the beginers documentation https://wiki.python.org/moin/BeginnersGuide and https://wiki.python.org/moin/BeginnersGuide/Download
 **Thoughts:** On to the next language to study, after the Python assesment.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
          ### Day 65 August 30, 2022.
 **Today's Progress:** I am, working through a guide on Python for Windows. In fCC JavaScript i practised a bit of Object Orientated programing. 
 **Thoughts:** On to the next language to study, after the Python assesment.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
          ### Day 66 August 31, 2022.
 **Today's Progress:** I started coding on a in Python and successfully printed a user input. I also practised Object Oriented Programming in fCC.
 **Thoughts:** Need to add more complexsity. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
           ### Day 67 September 01, 2022.
 **Today's Progress:**  I also practised Object Oriented Programming in fCC. I started the Elixir course on Udemy.
 **Thoughts:** I feel like i know to little about Python to make the jump between the two courses.  
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
            ### Day 68 September 02, 2022.
 **Today's Progress:**  I also practised Object Oriented Programming in fCC. I spend most of my time today figuring out whats wrong with the Elixir code. 
 **Thoughts:** I feel like Windows sucks. Most cources is presented in a Mac then I truggle weaving though Windows problems. That said my code from the instalation command was the problem. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
             ### Day 69 September 03, 2022.
 **Today's Progress:**  I also practised Object Oriented Programming in fCC. I removed Elixir and did re-instalation it did not go as expected. 
 **Thoughts:** Getting nowhere.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

              ### Day 70 September 04, 2022.
 **Today's Progress:**  I practised Object Oriented Programming in fCC. I removed Elixir and did re-instalation the build command worked as expected. Now the run command is the next bug.   
 **Thoughts:** Getting nowhere.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
               ### Day 71 September 05, 2022.
 **Today's Progress:**  I practised anonymous function in fCC. I practised how to run Elixir Code, and learned a bit about Enum with the shuffle method.  
 **Thoughts:** Peercoding helps. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.

                ### Day 72 September 06, 2022.
 **Today's Progress:**  I practised combining functions in fCC. In Elixir I build a deck of cards.   
 **Thoughts:** Didnt get to peercode today ;(
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                 ### Day 73 September 07, 2022.
 **Today's Progress:**  I practised combining functions in fCC. In Elixir I practised Pattern Matching section 2 in the Udemy course "The Complete Elixir and Phoenix Bootcamp". 
 **Thoughts:** putting a underscore before a variable tells the compiler that for Pattern Matching the variable is required. However the variable will not be used. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                  ### Day 74 September 08, 2022.
 **Today's Progress:**  I practised calling a function in fCC. In Elixir I practised Pattern Matching again, then I went on to practise documentation in the Udemy course "The Complete Elixir and Phoenix Bootcamp". 
 **Thoughts:** I did my duty today. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                   ### Day 75 September 09, 2022.
 **Today's Progress:**  I practised calling a function in fCC. In Elixir I redid parts of section 1 and 2, while making notes and practising the code again.
 **Thoughts:** No peercoding today, hence the catch-up on my desktop.
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                   ### Day 76 September 10, 2022.
 **Today's Progress:**  In Elixir I practised some Pattern Matching, then I went on to practise documentation in the Udemy course "The Complete Elixir and Phoenix Bootcamp". 
 **Thoughts:** I ran into a error. Will close and try that again tomorrow, and trouble shoot, and ask help in that order. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                    ### Day 77 September 11, 2022.
 **Today's Progress:**  In Elixir I tried documentation, upon getting the same results i made a post on the forums. The solution is quite simple do not run *{* iex -S mix *}* command. Finally finished the document section by by-passing the terminal commands. Then practising some DocTests.
 **Thoughts:** Sucks when your stuck and have no clear path forward in the present. Next problem open doc terminal command not working on my windows computer. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                     ### Day 78 September 12, 2022.
 **Today's Progress:**  In Elixir I practised DocTests on Windows. On the Mac with peercode I practised Map the Elixir version of a JS Object.
 **Thoughts:** I am moving a bit faster with Elixir 31 done, the JS problem on fCC looks intimidating. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
 
                      ### Day 79 September 13, 2022.
 **Today's Progress:**  In Elixir I completed section 4 and 5, then got stuck on a error in section 6. 
 **Thoughts:** I am moving a bit faster with Elixir 45 done, the JS problem on fCC looks intimidating. 
 **Link to work:** see screenshot(s) in my tweet @KobusScheltema.
