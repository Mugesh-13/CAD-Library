📘 Project Documentation: Knowledge House
🏷️ Project Title
Knowledge House – A Library Management Platform

🎯 Target Audience
Educational Institutes,Public Libraries

👤 Team Size
1 (Solo Developer)

💰 Budget
₹0 (Zero)

⏳ Timeline
1 Month

🏢 Type
Business to Business (B2B)

✅ Project Overview
Knowledge House is a digital Library Management System designed to help educational institutions and public libraries manage books, users, transactions, and space availability. It simplifies the librarian's tasks by automating  issue/return operations, and providing a searchable digital catalog.

🔧 Core Features
👤 User Management
User Registration
  Allows new librarians to register for an account.

User Login
  Secure login functionality for authorized access.

📚 Book & Library Management
Add Space Availability in Library
  Manage available reading/study spaces in the library.

Add Books
  Add new books with details like title, author, ISBN, category, and quantity.

Search and Filter Books
  Search books by title, author, category, or availability.

Update/Delete Book Details
  Modify or remove books from the library database.

View All Books
  Display the complete book catalog for quick browsing.

Trending Books
  Highlight books with the highest issue count or popularity.

🔁 Book Transactions
Issue Book to Member
  Record when a book is issued to a member, with due date.

Return Book
  Mark a book as returned and update the system.

Fine Amount Calculation
  Automatically calculate late return fines based on due date.

---Model Class--
Registration for Librarian :-
int id;
String name;
String email;
String password;
String confirm_password;
long dob;
long mobile_no;

Library:-
int id;
String name;
String address;
long open_time;
long close_time;
long contact_no;
Map<String,Integer> storage;

Books:-
int book_id;
String book_name;
String author_name;
String genre;
int No_of_copies;
String ISBN_number;
int year_of_publish;
List<User> users;

Member :-
int id;
String name;
String email;
String department;
long mobile_no;
double fine_amount;
List<Books> book;

Transaction:-
int transaction_id;
int book_id;
Long date_of_issue;
Long return_date;
Long due_date;
boolean book_status;

Storage:-
Map<Integer,Member> member;
Map<Integer,Librarian> admin;
Map<Integer,Books> books;
Map<Integer,Transaction> transaction;





















