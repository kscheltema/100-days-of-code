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
 
  ### Day 13: July 9, 2022 
 **Today's Progress:**
 **Thoughts:**
 **Link to work:** 
