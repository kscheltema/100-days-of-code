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
 
    ### Day 20: July 16, 2022 
   **Today's Progress:** I accepted that the environment to enter as a Junior Deverloper is not great. So In consultation with my Mentor Gary. I have decided to finish the the-complete-junior-to-senior-web-developer-roadmap. So far I have read a bunch of articles linked to the course, and did up to video 7 so far. 
 https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work
 https://zerotomastery.io/blog/developers-edge-how-to-become-a-senior-developer/
   **Thoughts:** It sucks. Life in general. But I need to move forward. 
   **Link to work:** see screenshot(s) in my tweet @KobusScheltema;
