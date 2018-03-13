<link rel="stylesheet" href="{{baseUrl}}/css/main.css">

<include src="../common/header.md" />

<div class="website-content">

# TE3201 Software Engineering

* [Lectures](#lectures)
* [Project](#project)
* [Learning Materials](#learning-materials)
* [Exam](#exam)
* [Grading](#grading)
* Multiple Repo!

## Lectures 

TUE 1800-2130 in E3‐06‐02

* :worried: No webcast (Reason: the lecture venue does not have the webcast facility)

* The lecture will be broken into small segments (about 30 minutes) of fairly independent parts so that late comers can still follow the remainder of the lecture.

* First 15 minutes will be a recap of previous lecture or free-flow discussion so that those slightly late will not miss the beginning of the lecture proper.

* Python topics will be in the 2nd half of the lecture so that those not interested in learning Python can leave early.

<include src="learningMaterials.md" />

## Project

To be done in individually, or teams of 2-3 members.

**Programming language**: The recommended language is Python but another Object-Oriented language (e.g. Java, C#, C++, ...) is acceptable if there is consensus among team members.

### Software to build

You will be building a personal assistant chat-bot software named _PAC_ (_PAC_ is a temporary name; you should give a different name to your own chat bot)
 
**_Basic_ Functionality**:

1. PAC interface can be text-based (i.e., no need for a graphical UI)
1. PAC helps with storing and retrieving at least **one type of data** that is useful to the user. Some examples of different types of data (you can pick one of them): details of contacts, todo items, appointments, deadlines, reminders, technical terms to remember, etc. Here is an example interaction between a user and a PAC that deals with TODO items:
   ```
   >> Hi, I'm PAC. What can I do to help you with your TODOs?
   
   add Return library book
   >> TODO added: Return library book
   
   list
   >> Here are the list of TODOs you have:
   1. Return library book
   2. Do TE3201 exercises
   3. Call back Jina
   
   delete 2
   >> TODO deleted: Do TE3201 exercises
   
   are you single?
   >> Sorry. I did not understand your request.
   
   help
   >> Here are the requests I understand.
   add {TODO description} : adds a TODO to the list
   list : lists all TODOs
   ...
   
   ```

1. There is **no need for PAC to be able to understand natural language** sentences. It is fine for the user requests to need to follow a strict format. Defining the request format is part of the project. The example interaction given above is just an example only. Hint: try to design a request format that is easy to remember and type.
1. PAC should support **adding, deleting, listing, searching** (by keyword) of data items.
1. _Persistence_: The data should be **stored in the hard disk** so that restarting PAC should not cause a loss of data entered in a previous session. 
   1. The data files should be in a human-readable format such as `.csv` (recommended), `xml`, `json`, plain text, etc.


Basic functionality given above counts as 2 _units_ of functionality. On top of that, you are required to add some more _additional functionality_ (of your own choice). The total amount of functionality required is given below.

Team size | Total amount of functionality
--------- | -----------------------
1-person  | 3-4 units
2-persons | 4-5 units
3-persons | 5-6 units

**_Additional_ Functionality**:

Some suggestions for _additional functionality_:
* More attributes for data items e.g., priorities, tags, birthdays
* Multiple data item types e.g., support saving TODOs, appointments, and deadlines
  * Support connections between data items e.g., ability to assign a TODO to a contact
* Multi-user support e.g., assume the software is installed in a common computer in your office and allow multiple users to interact with it
* More ways to query data e.g., find contacts that has a birthday in next 2 days, find all TODOs with high priority, etc.
* Any other feature (get approval from prof before implementing)

### Constraints

1. You should not use relational/SQL databases e.g., MySQL
1. The software should work in a Windows computer that has the latest releases of Java, .NET, and Python 3.
   1. If your software need other software to be installed (e.g., third-party libraries), please get prof's permission first.

### Deliverables

* **Week 8** (mid-term submission): 10%
  * Deadline: Week 8, Tuesday 6pm
  * Functionality: at least most of the basic requirements are fulfilled (you may leave out the _persistence_ requirement)
    * Submission: demo during lecture in week 8
  * Documentation: 
    * Sections to include:
      * Cover page: Include product name, names of team members 
      * User stories: Give user stories to cover all current and future functionalities
      * Use cases: Give 2-3 use case descriptions. Choose use cases that require most number of steps or most complicated.
      * Non-functional requirements: Give 5-10 NFRs for the project. Try to include a diverse range of NFRs.
      * Activity Diagrams: Give at least one activity diagram related to the product e.g., an AD that explains a workflow of how the user uses your product or an algorithm in the code. You can use any drawing software (e.g. PowerPoint), or hand-sketch and photograph/scan the diagrams.
    * Submission: upload to IVLE as a `.docx` or `.pdf` file. File name should contain team member names. e.g., `John Doe, Sarah Tan, Viet Ngoc.docx`

* **Week 13** (final submission): 30%
  * Functionality: all functionality
    * Submission: Upload to IVLE, demo during lecture in week 13
  * Documentation: TBD


## Exam

* Total: 2 hours
  * Part 1: MCQ (1 hour)
  * Part 2: Essay (1 hour)
* Open book

## Grading
 
* Project: 40%
* Exam: 60%

</div>

