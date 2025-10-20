---
title:  "Computer Science ePortfolio"
mathjax: true
layout: post
categories: computer science 
---

## Table of contents:
* TOC
{:toc}

## Informal Code review of Artifacts

{% include embed.html url="https://www.youtube.com/embed/N3YUCYqg6oA" %}

## Self Assessment, my selfview on my work and process.

### Reflection on the skills throughout the coursework program

During the Computer Science program, I have learned many skills and techniques that have shaped me into a competent and resourceful computer scientist. As the program progressed, the courses became more in-depth, focusing on modern tools and concepts related to software development and algorithms. The initial coursework helped build a solid foundation and provided a general understanding of what the program entails.

Later courses, such as Current and Emerging Trends in Computer Science, covered topics like Artificial Intelligence, Deep Learning, and Neural Networks. While these topics focused on the applied side of AI, they also briefly explored how internal models, neural network layers, and optimizers function mathematically. This included defining functions, both iterative and non-iterative, and understanding their construction.

For me, studying the mathematical side of AI alongside its practical (programming) applications helped me gain a deeper understanding of not only how to use these techniques but also how theory and practice work together in a cohesive process. Reinforcement Learning and Deep Q-Learning, in retrospect, were key examples where I explored the internal workings of models, the use of different training and prediction techniques, the roles of episodes and sampling, and more.

Other coursework, such as Full-Stack Development, helped me understand how modern web-based solutions are designed and developed. The stack used in the course was the MEAN stack, which, in my opinion, is a great introduction to how the back end, database, and front end work together. I learned when to use server-side HTML rendering and when it is best to use single-page applications (SPAs), with the objective of minimizing delays and maximizing user experience. JavaScript is one of the most widely used programming languages in the field, especially in web development, so if I decide to enter the private sector, I will have the foundational knowledge and practical skills to start working without difficulty.

Collaboration is a valuable skill for a computer scientist, and in any professional field. In the 1980s and 1990s, computer solutions were often developed by a single individual. However, as architectures have become more complex and expectations for design quality have increased, software development can no longer be considered a one-person job. Using tools like Jupyter Notebook taught me how to write code that supports collaborative development within a fast-paced development cycle.

Early coursework emphasized the importance of coding standards. Proper use of coding standards and comments helps teams create usable and maintainable code. In addition, following coding paradigms and maintaining thorough documentation provide a design basis for projects, allowing potential design flaws to be identified and corrected early in the development cycle.

Communication with stakeholders is also critical to a project’s success. An unhappy stakeholder means that, even if the technical aspects of the project are solid, the final product may not meet functional expectations. Communicating clearly, using accessible language rather than overly technical terminology, helps stakeholders understand how resources are being used. For example, during an AI model development project, a stakeholder will want to understand how the design is being constructed. The developer must provide clear and simple explanations of the process and reasoning. If the developer fails to communicate effectively, the stakeholder may not realize that the project is diverging from their expectations and therefore may not provide timely feedback.

The coursework in the program maintained a strong balance between theoretical concepts and practical application. Additionally, forum discussions helped me develop my communication skills within the field and fostered a positive, knowledge-focused learning environment. 

Finally, security is a critical skill for any computer scientist. Security concepts were taught in at least two courses. The first focused on developing project examination skills, such as identifying vulnerabilities in dependencies and understanding exploits, like running arbitrary code through HTTP calls. In Full-Stack Development, the use of tokens and secure network communications was explored extensively and in great detail. For example, we implemented JWT (JSON Web Tokens) in RESTful calls to handle credential communication between Angular and Express applications.

### introduction of my Artifacts

There are three artifacts in the current ePortfolio, chosen to demonstrate my full range of skills in software development, algorithms and data structures, and databases. A competent computer scientist must develop proficiency in all three areas.

My artifact for software development showcases the use of the Android API in Android Studio to create industry-standard solutions. Specifically, I first developed a simple inventory app and then enhanced it by adding customer, product, and sales features. It includes an invoicing system and sales statistics with useful graphs that provide a clear picture of the company’s performance.

My artifact for algorithms and data structures demonstrates the use of complex data structures, such as texture data, and advanced algorithms, including the implementation of a Julia set generator (fractal) and the transformation of that data into textures. The base project consisted of a simple 3D composition of primitives with lighting and texturing. To further demonstrate advanced skills in algorithms and data structures, I also developed a thread-safe, stealable thread pool with various supporting classes such as TaskQueue. These classes make use of metaprogramming through templates.

Finally, my artifact on databases initially involved the use of a publicly available dataset from the Austin Animal Center, which was used to create an interactive dashboard. The next iteration involved developing a Twitter scraper using automation tools such as Selenium, then cleaning the data and storing it in a JSON file, which was later added to a secure MongoDB database. The collected tweets were then used as input for K-means clustering (after a simple embedding process). Additionally, the enhanced version incorporated a pretrained model for sentiment detection and a word cloud image renderer. All of this data was integrated into a new, easily navigable, and useful dashboard featuring added tabs and an image slider.

## Artifact One: Software Design and Engineering.

{% include embed.html url="https://www.youtube.com/embed/R_3AAnpJoCY" %}

### Compiling and use guide.

Android Studio is required. Be sure to synchronize the project dependencies and use the API 36.

### Narrative.

The artifact is from the final project of CS360 Mobile Architecture and Programming, developed during the July–August 2025 term. The artifact originally submitted in the CS360 coursework is described as follows:
The solution is called Inventory App, an Android application designed to manage a business’s inventory. It includes a secure login feature and a side menu. The side menu recognizes when a user is logged in and activates the following features:

* Add Inventory
* See All Inventory – An interactive table where all inventory entries are displayed. A row can be selected and automatically deleted.
* Edit Inventory – The user can search for an inventory entry by its ID. Once the entry is found, the user can edit any data field and save the changes.
* Request and Activate SMS Permission – The app requests Android SMS permissions and activates them as needed.

Additionally, all the back-end procedures are handled with SQLite via CRUD operations.

I believe this artifact is a great addition to my portfolio because it showcases the use of a widely adopted tool, Android Studio, and demonstrates features that range from medium to complex within the Android SDK. For example, it incorporates SQLite CRUD operations along with a Navigation Menu and Fragments to create an intuitive UI and UX. This was my initial motivation for including the artifact for enhancement.

The project also has strong potential to evolve into a more complete solution with additional features. For instance, in the enhancement, I used the AutoCompleteTextView component with dropdown selection for creating Products and Invoices. Autocompletion was particularly useful because Products and Invoices are linked with the Inventory table, while Invoices are also linked with the Customer table. The logic is as follows: each Product is associated with inventory, and each Invoice is associated with a customer. With autocompletion and dropdown functionality, instead of manually searching for the ID of a Product or Customer, the AutoCompleteTextView component provides a list of possible matches (for example, customer names).

Additionally, I used DialogFragments to create popup submission forms. For example, in the Add Invoice fragment, users can add Invoice Items. Each Invoice Item includes a product ID (foreign key), quantity, tax rate, item amount before tax, and total amount after tax. This entire process is handled within the popup. If the addition of an Invoice Item is successful, the Invoice main fragment displays a table that includes all previously added items along with the new one.

Another example of my showcased abilities was the implementation of external libraries such as SmartTable and MPAndroidChart. Inventory-related fragments originally used a custom grid table, which was challenging to design and implement. By integrating SmartTable, I was able to streamline development and provide an easier way to implement interactive tables.

Overall, the enhancement expanded the application to cover a broader set of features relevant to a business that manages inventory, including: User Authentication, Inventory, Customers, Products, Invoices, and Sales Analytics.

Personally, enhancing and modifying the artifact has been a real challenge. Even though many features have already been implemented, I would still consider the solution incomplete. The use of SmartTable has greatly supported the development of the enhancement. However, designing the interaction between the Database Manager and the various fragments has proven to be a significant challenge.

Many design considerations had to be taken into account. For example, a product deletion feature was added; however, the system does not completely remove the product entry from the database because many past invoices may reference it. Instead, the Product table includes an additional field called Inactive. When a product is marked as inactive, it can no longer be used to create future invoices, while past invoices that reference it can still be displayed correctly.

Another challenge was the implementation of the Add Invoice feature, for a similar reason: it required designing a solution that would use both the Invoice database table and the Invoice Items table. Developing an effective design took longer than expected. Ultimately, I implemented a popup form solution where each invoice item could be added through a separate form and then displayed in a table. However, this process was time-consuming because I first had to learn how to use DialogFragments effectively.

There were many other design decisions that took longer to plan than to implement. One example was determining the distribution between Table Data and Autocompletion Data, particularly in situations where an AutoCompleteTextView needed to remain synchronized with a data table. Additional challenges arose with autocompletion because numerous callbacks had to be implemented to keep the selection options up to date while also maintaining consistency with the class data that would later be submitted to SQLite.

## Artifact Two: Algorithms and Data Structures.

### Compiling and use guide.

You need Visual Studio (stdc++17 or newer) with C++ integration. The required libraries are in inside the project.

### Narrative.

The present artifact is from the CS-330 Computer Graphics and Visualization course. It originally consisted of a 3D scene composition featuring 3D objects (constructed from primitives), texturing, materials, and lighting. Additionally, it included navigation controls, adjustable navigation speed, and camera perspective options (such as orthographic, front, and top-down views). It was created during Term C-4, June–August.

The artifact was included because it demonstrates various skills in handling complex, low-level libraries. The main library used was OpenGL, along with its methods and implementations for managing communication between the CPU and GPU. This included working with Vertex Array Buffers, Texturing, Shaders, Phong Lighting, and more. Additionally, the project by design required efficient, high-performance code.
In the enhanced version of the project, I added a StealPool (a thread pool with a work-stealing queue) and a Julia Fractal Renderer, implemented on both the CPU and GPU. I also integrated the Dear ImGui library to handle input and improve the user experience.

The most significant enhancement was the implementation of the work-stealing queue, which required advanced C++ programming skills, including templates, functionals, concurrency, and metaprogramming. To support this development, I studied the book C++ Concurrency in Action, which proved to be a challenging yet highly valuable learning experience.

I would argue that the independent research required to learn and apply concurrency and the Dear ImGui library, along with the implementation of various algorithms (with help from the book, of course), was successful. For example, the implementation of a thread-safe queue, whose main feature is preventing mutex locks, worked effectively. However, this process did not come without challenges.

The main challenge I faced was understanding the changes in C++ standards. I initially developed the StealPool using MinGW with the Clang Language Server Protocol, and compilation worked without issues since it was configured with the -std=c++17 standard. However, when I ported the project to MSVC, compilation became a challenge due to differences in how each compiler handles deprecations.

MSVC treats certain deprecated type trait implementations (present in the book I used, due to its age) as errors, whereas GCC only treats them as warnings. Other syntax-related issues, such as copy elision, also caused complications and made it difficult to get the code running. To troubleshoot, I returned to MinGW in a different text editor and compiled my CMake configurations using the MSVC toolchain to precisely identify the problems.

Additional ongoing challenges include texture management, shader implementation, shader compilation, and texture slot handling.

Here is a list of some of the related enhancements I implemented:

* Improved performance through more efficient handling of 3D primitives. The system can now load multiple torus meshes with different configurations to the GPU without the need for reloading.

* Improved performance by resolving a memory leak where textures were continuously loaded and GPU memory was not freed after object deletion.

* The ThreadPool now handles CPU-based fractal rendering with double precision.

* Texture uploading is performed in parallel using the thread pool.

* Texture slots remain consistent and no longer conflict within the main loop.

* Dear ImGui provides a modern, polished interface that enhances the overall user experience.

Finally, the enhanced project still needs some polishing, as there are a few issues that need to be resolved, such as stuttering when the thread pool submits multiple tasks, and low-resolution rendering of the fractal on the GPU.
## Artifact Three: Databases.

{% include embed.html url="https://www.youtube.com/embed/qVLP87AiuuQ" %}

### Compiling and use guide.

The project requires python3 and Jupyter Notebook or Lab.
Before running the dashboard (ProjectTwoDashboard.ipynb), the user need to set a username and password alongside importing the required databases collections. The credential must be updated in the jupyter notebook for correct project data display. 

Inside the mongo shell:
```javascript 
use admin
db.createUser({
  user: "myUser",
  pwd: "myPassword",
  roles: [
    { role: "readWrite", db: "AAC" }
  ]
})
```

Then import csv data into the AAC Animal collection:
```bash 
mongoimport --db AAC --collection Animals \ 
--type csv --file aac_shelter_outcomes.csv --headerline \ 
--username myUser --password myPassword \ 
--authenticationDatabase admin
``` 

Similarly, you can do it for the embedded .json and tweet information. If you already have credentials, just add the role on you user data entry.

### Narrative.

The artifact is the final project for the Client/Server Development course (CS-340), which I completed in the C-4 2025 term (June–August). It consists of an Animal Shelter Database based in Austin (in .csv format) that can be imported into MongoDB, a Python module to connect to the server via PyMongo and perform queries (CRUD operations), and an interactive dashboard featuring various tables and informative graphs.

The inclusion of this artifact in my ePortfolio is justified because it demonstrates my skills with industry-standard tools such as MongoDB, Python, Jupyter, and various Python utilities like PyMongo and Dash. While these tools are often used more in data analytics than in traditional software development, they still have significant applications in the private sector, which adds substantial value to the showcased skills.

For example, in the original project, the CRUD implementations in the Python module demonstrate the practical application of concepts to real-world scenarios, such as database management. Additionally, interactive graphs are essential for presenting processed data and conclusions to non-experts in the field. Customizing interactive graphs, such as a dynamic map of the Austin area, adds significant value.

The artifact has been improved in several ways. First, I wanted to incorporate my own retrieved data, so I developed a Twitter scraper using Selenium and BeautifulSoup. Using this tool, I extracted more than 5,000 tweets related to animal shelters in metropolitan areas such as Austin, New York, San Francisco, and Los Angeles. I then used additional tools in Jupyter to extract data from JSON files, perform data cleaning, and import it into MongoDB.

Other improvements include expanding the dashboard to support more graphs using the processed tweet data. For example, I applied a sentiment analysis model to show the overall public sentiment regarding animal adoption and care. Other processed visualizations include clustering using embeddings and a word cloud.

I learned how Chrome automation works and the intricate problems that arise when scraping a large social media platform like Twitter. I had to be patient because they enforce query quotas, and I used search operators such as until:, since:, OR, and AND, plus the live tweet feed, to collect a varied set of tweets with minimal repetition. I also learned how to save and reload cookies to speed up login while avoiding detection by the platform. Other skills I developed include managing and cleaning JSON data and using pre-trained models to obtain tweet sentiment. The work was challenging and required reading a lot of documentation, but I ultimately succeeded.

