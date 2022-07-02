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

### Day 5: July 1, 2022 
**Today's Progress:** 
**Thoughts:**
**Link to work:**
