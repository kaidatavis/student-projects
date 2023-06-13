# Project ideas and readings

## For all projects

### Background
- The genral project ideas are online at: https://kaixu.me/projects/. 

### Reading
- [Survey on the Analysis of User Interactions and Visualization Provenance](https://eprints.mdx.ac.uk/30220/6/v39i3pp757-783.pdf)
  - Provide the background and overview of existing work.
  - It has a [website](https://provenance-survey.caleydo.org/)

## Project: Projection of provenance vector sequence 
### Background and readings
- [Sensemaking Processes as High-Dimensional Vector Squences](https://kaixu.me/2022/05/23/visualising-the-sensemaking-space/)
  
### Ideas
- Visualise the online sensemaking provenance as vector sequences, i.e., apply provectories to browser history data;
- Visualise the Jupyter provenance as vector sequences, i.e., apply provectories to jupyter user log;
  - You should also go through the readings for ['Project: Jupyter Extension'](https://github.com/kaidatavis/student-projects/blob/master/README.md#project-jupyter-extension)
- Improve the vector sequence visualisation so it becomes easier to see patterns and understand what users are doing.
  - You should also go through the readings for ['project: browser extension'](https://github.com/kaidatavis/student-projects/blob/master/README.md#project-browser-extension)

## Project: Jupyter extension
### Background and readings
- [Human-Centred Data Science](https://kaixu.me/2021/01/23/machine-learning-provenance-for-hyperparameter-tuning/)
- [Human-AI Teaming: Qualitative Analysis and Generative Models](https://kaixu.me/2021/01/31/interactive-learning-for-document-coding/)

### Idea 
- Capture and visualise the user interaction logs in Jupyter using a Jupyter extension (similar to verdant, not the provenance vectors) 
  - to support tasks in machine learning model building, such as hyperparameter tuning
  - to support end users, such as artists, to use generative AI models, such as [stable diffusion](https://stability.ai/blog/stable-diffusion-public-release)

## Project: browser extension

### Background and readings
- [Visual Analytic for Sensemaking](https://kaixu.me/2021/01/31/analytic-provenance-for-sensemaking/)
- [Human-AI Teaming: Qualitative Analysis and Generative Models](https://kaixu.me/2021/01/31/interactive-learning-for-document-coding/)

### Ideas
- Create a browser extension to support the usage of LLM or generative AI models through their web interface
- Improve the design of the HistoryMap so the tree fits better within a [Chrome side panel](https://developer.chrome.com/blog/extension-side-panel-launch/)
- Create a browser extension that provide end-to-end support for online shopping
  - Start with online research (can use HistoryMap)
  - Automatically gather the required information, such as the price for different model
    - with web scraping or chatGPT
  - Create a visual comparison of different options
- A user study to compare the tree/hierarchy visualisation first used in SenesMap against the latest that is availalbe in popular browsers, such as tab grouping and [chrome 'journey'](https://blog.google/products/chrome/finding-answers-gets-better-chrome/).
- How to record the 'why': many rules/decisions are recorded without the 'why'. Overtime, the reasons become no longer valid, while the decisions/rules are still being followed, sometimes blindly. This project aims to see if there is any efficient way to record the 'why' that will not introduce too much extra work and can be easily used by other applications. 


# Project plan/proposal

Below is a general structure, and please refer to the moodle page for your project module for specific format/requirements. If there is any difference, always follow the instructions from the module page.

It is not always a marked component, but very important to ensure a successful project. Think of it as a tool to hellp you think ahead and plan. Also, you will reuse most of it for the final report later.

- Introduction/background: the general problem area, such as using machine learning to support sensemaking
- The problem: the specific problem that you want to improve. For example, the exsting recommendations made by machine learning models are not very good.
  - literature review (academic publications): what academics have done on this problem. More details in the literature review section below.
  - related software, app, website, and other resources: some of the related efforts are not published in an academic paper. For example, not all the recommendaiton algorithms are discussed in a paper.
  - The main goal here is to set your work in the context of existing works: what is the gap/missing piece.
- Your project idea:
  - The main hypothesis, e.g., using large language models can improve the quality of recommendations
  - The approach, e.g.,
    - who are your targeted users? and what are their use case (i.e., what task will they use your tool for)?
    - what large language model do you plan to use? why do you choose it?
    - how do you obtain the model? do you have the hardware needed to run the model?
    - will you need to retrain/update the model? do you have the labeled data for this? do you have hardware required for this?
    - ... 
  - The evaluation method (following the same example):
    - what is the definition of 'quality' and how do you measure it?
    - do you plan to talk to/interview your users to understand their requirements?
    - do you plan to do any user evaluations?
    - ... 
- Plan
  - Agile and iterative: 
    - Gradually build up to the final prototype; 
    - Don't try to build the final prototype from the beginning
   1. Literature review (if there is more to do)
   1. User requirements:
      1. Talk to the real users
      1. Document their needs: task specific (e.g. finding the most suitable master degree), not technical specific (need to use machine learning)
   1. Paper prototype: design sketches 
      1. on real paper or design software such as figma
      1. Get user feedback
   1. Working prototype with minimal functions (MVP: minimal viable product): 
      1. leave out non-essentail functions (such as user account) and 
      1. use simple alternatives instead of complex ones (e.g., using decisoin tree insteal of Large Language Models)
      1. Get user feedback
   1. Fully working prototype (final prototype)
   1. User evaluation
   1. Final report
 - Create a project plan using [GitHub Project](https://github.com/kaidatavis/student-projects/projects) (more on this later).
    
# Software and programming

## GitHub.com
We will this shared github reporsitory for project file and code, so you 
1. will never lose your code (because of corrupted USB or hard drive), and
2. can easily show it to other people (e.g.,as part of your work portfolio for job application).

If you never use git before: 
- concepts and commandline tool (git): https://git-scm.com/book/en/v2 (first 2 chapters)
- github (a website) tutorial: https://docs.github.com/en/get-started/quickstart/hello-world

You probably want to check out [GitHub Student Developer Pack](https://education.github.com/pack) that provides features that you will need to pay otherwise.

How to use different GitHub features for the project:
  - The repository is public, so don't upload any data that you don't want to share
    - You can create a separate private repository for sensitve data. Follow the 'data management plan' of your ethics application.   
  - Use [this (wiki) page](https://github.com/kaidatavis/student-projects/wiki/Meeting-Notes) for meeting notes
    - Follow the meeting notes/minutes template there and the latest one on top.
    - [This guide](https://gist.github.com/cuonggt/9b7d08a597b167299f0d) can get you started if you never used markdown before 
      - It is similar to HTML, but much simpler. Also very useful for programing.
  - 'Issues': todo list/tasks and coding issue
    - Each 'issue' is a task to complete (action from the meeting)
    - Assign an issue to the person that is responsible 
  - 'Projects': planning and project management (this has been updated recently, so points below may be updated) 
    - You can create a kanban board in 'project' (similar to Trello), 
    - create "milestones', e.g., one for each iteration
    - add 'issues' to 'milestones', and set deadline
    - start with [this project template](https://github.com/users/kaidatavis/projects/2)
      - add your name to the project title, such as 'Kai's project plan'
  - Each of you will have a top-level folder in the repository for your project
    - Please send me your github account username or email, so I can add you to the repository.
    - Please name your folder like this: year-degree-name-title (e.g., 2023-msc-kaixu-visual-analytics-for-sensemaking)
    - Use the your folder for your code and other things like notes (in markdown)
    - Include in your folder a 'readme.md' file to list all the things in your folder (e.g., which subfolder contains what) and other information such as how to run your code.
    - Don't include large files as everyone else will need to download them as well (when they do a 'pull' of the repository).
    - There will be top-level folder(s) for share resouces such as datasets.

## Code editor (IDE): 
Recommended: Visual Studio Code https://code.visualstudio.com/. 
- This is suitable for both front end (JavaScript) and machine learing (Python) development;
- It is probably the most widely used IDE in industry;
- For front end, it is better for JavaScript development than other editors like Brackets (http://brackets.io/), Sublime Text (https://www.sublimetext.com/), or Notepad++ (https://notepad-plus-plus.org/)
- For machine learning, it can run python fine and can open Jupyter notebooks (need to install relevant plugins)
- Get started: https://code.visualstudio.com/docs

## Writing: Latex (instead of Word)
Recommended: Use Latex instead of Word for all the reports: proposal, progress report, final report, and viva.
- This will 
  - make your report look more professional
  - make the references easier
  - this is how many academic papers and books are written
- Recommended editor: Overleaf (https://www.overleaf.com/), like Google Docs for Latex.
- Learn Latex in 30 minutes: https://www.overleaf.com/learn/latex/Learn_LaTeX_in_30_minutes;
- The video recording of my overleaf tutorial: https://youtu.be/PqW8myobrPE
- How to add references: https://www.overleaf.com/learn/how-to/Using_bibliographies_on_Overleaf



# Litearature Review

## Existing Work
- Needs to be much more **complete** than the litearture review in the project proposal;
- Cover different types of resources: app, website, service, organisation, physical print/product ...
- Focus on the most relevant: help you to narrow down your scope.
  - For example, if your project is about AI-based recommendations, there is no need to introduce what AI is (the reader would know) and go straight to the latest machine learing models for recommendation.
- Include academic publications to support your argument: 
  - You can include webpages and online articles, but these are not 'peer reviewed', i.e., anyone can potentially say saything online, and as a result these are usually not regarded as reliable evidence.
- Please to search for academic papers:
  - IEEE Xplore: http://ieeexplore.ieee.org/Xplore/home.jsp
  - ACM Digital Library: https://dl.acm.org/
  - Google Scholar: https://scholar.google.com/
- Things to consider when selecting which papers to cite
  - IEEE Xplore and ACM Digital Library are usually more rigourous than Google Scholar: all papers published there are checked by one or more researchers, whereas this is not always the case for Google Scholar (such as self-publishing on arXiv).
  - Papers that are more than 5 years old is often outdated (no longer the state of the art), especially in an active research field such as machine learning. Make sure there is no later work that supersedes it if you want to use it.
  - Papers in well known journals and conferences, such as Nature or Science, are considered strong argument/evidence. 
  - You can also get an idea of how good a journal or conference is from its 'impact factor' (has different names) such as the 'h5' metrics used by [Google](https://scholar.google.co.uk/citations?view_op=top_venues&hl=en&vq=eng) or the 'impact score' by [research.com](https://research.com/conference-rankings/computer-science).

For this project, you are likely to find good-quality related work from these journals and conference
 - IEEE Transactions on Visualization and Computer Graphics ([IEEE TVCG](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=2945))
 - [Computer Graphics Forum](https://onlinelibrary.wiley.com/journal/14678659)
 - ACM conference on human factors in computing systems ([ACM CHI](https://dl.acm.org/conference/chi))

Besides search, it can be very useful to just go through the latest papers from these journals and conferences
- Because relevant papers do not necessarily include the same keywords (a paper about analysing user behaviours may not have the term 'sensemaking')
- Start from the latest issue/year, and then move onto the year before once completed, and so on.
  - usually the last 3-5 years will be sufficient.
- Have a quick look of the title and/or abstract to check if the paper is relevant or not
  - many papers can be excluded by the title alone
  - save the paper in zotero if it seems relevant after reading the abstract
- We will use a shared zotero group to collect and share all the relevant papers found (more below in the 'reference' section)


## Development Technologies

- Be **open** about what form the project prototype will be: app, website, service, organisation, physical print/product ...
- Research different ways of implementation:
  - For example for app development, there is native and hybrid, and then there are many different hybrid frameworks. 
  - Comparison: 
    - Identify required **functions**, such as user regiter/login, database, messaging, image/video, ...
    - Compare different options regarding to the functions: is it possible at all, how easy it is to learn/program, how fast/secure/reliable it is, ...
- Justify your choice

## Reference
- Two parts: citation in the main text and the references at the end of reprot.
- Use a tool; don't create reference manually.
  - Recommended: zotero (see details below)
  - Use zotero for collecting and inserting citations/references
  - We will also use zotero to share relevant papers. 
    - Add all the relevant papers to this Zotero Group Library: [Sensemaking and human-AI Teaming](https://www.zotero.org/groups/4762437/sensemaking_and_human-ai_teaming)
    - Use Zotero tags to group the papers (don't just use all the tags Zotero automatically created)
    - Don't upload the full paper PDF file (the free zotero group library has a very limited storage size)
    - Do include a link to the public/free online full paper pdf if there is one using the 'notes' section in Zotero.
    - Use the 'notes' section to summarise what the paper is about and discuss its stregnth and weakneess.
- If you are using Latex, 
  - follow this [overleaf bibliography tutorial](https://www.overleaf.com/learn/how-to/Using_bibliographies_on_Overleaf);
  - watch my [latex tutorial](https://youtu.be/PqW8myobrPE), which includes references.
  - you can use Zotero (see below) to collect the papers from publication webiste (such as IEEE xplore and ACM Digital Library) and then generates the bibtex entry.
  - IEEE xplore and ACM Digital Library also provide the bibtex entry on the webpage for each paper: 'cite this' for Xplore, 'export citation' (double quote button) for ACM Digital library.
- If you are not using Latex, use [Zotero](https://www.zotero.org/). 
  - This is a recording of me showing how to use Zotero: https://youtu.be/R_5bjdE-kSw
  - use their browser extension to automatically add reference: 
    - [Zotero connector](https://chrome.google.com/webstore/detail/zotero-connector/ekhagklcjbdpajgpjgmbionohlpdbjgc?hl=en)
    - These can export the papers to bibtex format, if you use Latex.
  - use their Microsoft Word plugin to add references to report
    - [Zotero word processor plugin](https://www.zotero.org/support/word_processor_integration)

# First Iteration

## Requirements

- Find real users or company/organisation/charity that work with real users.
  - Find someone local if possible: much easier for the communication.
- Get the requirements from the real users, not what you think.
- The requirements should be technology independent, in most cases.
- ['How to Talk to Users'](https://www.ycombinator.com/library/6g-how-to-talk-to-users) by [YCombinator](https://www.ycombinator.com/) the most successful startup incubator (airbnb, dropbox, stripe, etc.)
https://www.youtube.com/watch?v=MT4Ig2uqjTc

### Design/Implement

- Paper prototype/wireframe tool: 
  - Pencil and paper
  - Low fidelity: Balsamiq https://balsamiq.com/
  - High fidelity: ***Figma***: https://www.figma.com
  - Share the design: InVision https://www.invisionapp.com/

### Evaluation/Feedback

- Show user the paper prototype/wireframe and get feedback.
- Revise the desgin and project scope accordingly.


# Project Meeting 3 - first iteration update

## Literature Review - Progress Update
- Literature review should be more or less finished. This is a good time to discuss if there is any issue or difficulty.
- Everyone updates on:
  - Any change on the project idea and/or scope and the reason;
  - Any decision on development technology and the reason.
- Results on the mobile app development technology survey.

## First Iteration - Progress Update
- Contacted any users, and what are their requirements?
- Any questions about the requirments, design, and evaluation?

# Project Meeting 4 - second iteration update

## Progress Demonstration

- Please prepare a short demo of the progress so far. 
- This shoud be informal, and no more than 5 minutes.  
- live demo if prefererred, but screen recording and screen shot are also fine.
- This is a good practice for your viva demo

## Questions and Answers

- You can edit this page or email me if there is anything you want to discuss before the meeting, 
- Otherwise I will try to answer your questions then. 

# Project Meeting 5 (final) - final reprot & viva

The meeting will have two parts: 

## Q&A session

Anything related to project, especially the evaluation, final report and viva.

## Evaluation

- Recurit 10-15 people (the more the better);
- Collect some demographic information, such as age, gender, education level, and other things that are important to your app;
- Divide the participants into two groups: one using your app, one without;
- Ask them to complete one or more tasks (exact the same for two groups);
- Record some measurements: such as completion time, accuracy, and quality of the answer;
- Record the process: screen capture video or video recording;
- Compare the 'measurements' from the two groups to see if there is any difference;
- Analyse the recording to see what caused the difference and how it happened;

## Viva
- The actual viva is usally 30 minutes, with 20 minutes presentation & demo and 10 minute Q&A
- The presentation (usually in ppt) covers everything about the project: from introduction and literature reveiw to implemantation and evaluation. Essentilly, it is an overview of your entire project in 15 minutes.
- There is ususally a demo if the project produces some software/app/website. This is your chance to impress the examiners (about the quality of the project outcome), as it provides much more details than the screenshots in the final report. 
- The presentation and demo should be no more than 20 minutes in total, which means about 10 ppt slides. You can mix the two, i.e., including demo during presentation, or do one after the other, e.g., slides first and then demo.
- The last 10 minutes are for the examiner to ask questions. This can be to used to clarify things, ask for missing infomration, ensure you fully understand the work, etc.

For the mock viva, 
- The project doesn't have to be completed; practice with what you have;
- Everyone can ask questions, not just Kai;
- Everyone will provide feedback on how to improve the presentatio and demonstration afterwards. 

# Marking Schemes
## Assessment for Final Report (CS)
1. Abstract (Mark out of 3)
2. Background and Literature: problem definition, literature review etc (Mark out of 5)
3. Design: requirements analysis and design specifications (Mark out of 6) 
4. Work done (Mark out of 8)
5. Evaluation (Mark out of 8)
6. Conclusion: with critical reflection on problem as defined (Mark out of 5)
7. Presentation: Presentation of report and quality of written English (Mark out of 4)
8. BCS criteria: Does the project satisfy the BCS exemption criteria (0 no, 1 yes)

## Assessment for Viva Voce and Demonstration (CS)
1. Quality of artefact: Is the artefact well designed, organised, and logically developed? Is the artefact sophisticated, polished, and elegant? Is the coding style advanced? How well does it meet its requirements in practice? Has it been evaluated sufficiently? (Mark out of 15)
2. Presentation and understanding: Does the student understand all aspects of the work they have done (from requirements to evaluation?) Can they articulate and justify decisions they have made at all stages of the project. Can the student discuss other aspects of their work (e.g. background) (Mark out of 15)

## Assessment for Final Report (IT)
1. Abstract (Mark out of 3)
2. Background and Literature: problem definition, literature review etc (Mark out of 5)
3. Design: requirements analysis and design specifications (Mark out of 5) 
4. Work done (Mark out of 8)
5. Evaluation (Mark out of 5)
6. Conclusion: with critical reflection on problem as defined (Mark out of 5)
7. Presentation: Presentation of report and quality of written English (Mark out of 4)
8. BCS criteria: Does the project satisfy the BCS exemption criteria (0 no, 1 yes)

## Assessment for Viva Voice and Demonstration (IT)
1. Viva (Mark out of 25)

## Assessment for Artefact (IT)
1. Artefact Evaluation: Does the artefact appropriately culminate the work for the time period and study done? (Mark out of 20)






