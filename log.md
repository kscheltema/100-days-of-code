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
**Link to work:** ![image](https://user-images.githubusercontent.com/82137766/176489510-6fe00679-8bdc-467f-828a-5afa02ac9d11.png) ![image](https://user-images.githubusercontent.com/82137766/176489737-ea6b1d93-5321-4957-b87e-fa68030d8603.png)
![image](https://user-images.githubusercontent.com/82137766/176489805-6599c522-ba39-468c-901e-2986d2af4efd.png)


### Day 4: June 30, 2022 
**Today's Progress:** 
**Thoughts:**
**Link to work:**
