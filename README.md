CREATE TABLE Book_Store (id INTEGER PRIMARY KEY, item Text,name INTEGER, author INTEGER, price INTEGER, aisle INTEGER ); 

INSERT INTO Book_Store VALUES (3, "book", "it starts with us", "colleen hoover", "13", "1");
INSERT INTO Book_Store VALUES (4, "book", "it ends with us", "colleen hoover", "15", "2"); 
INSERT INTO Book_Store VALUES (5, "book", "we were liars", "emily lockhart", "21", "3");
INSERT INTO Book_Store VALUES (6, "book", "one of uds is lying", "brian leslie parker", "17", "4");
INSERT INTO Book_Store VALUES (7, "book", "one of us is next", "brian leslie parker", "19", "5");
INSERT INTO Book_Store VALUES (8, "book", "they both die at the end", "adam silvera", "8", "6");
INSERT INTO Book_Store VALUES (9, "book", "our little lies", "sue watson", "9", "7"); 
INSERT INTO Book_Store VALUES (10, "book", "deadly little secret","laurie faria stolarz", "10", "8");
INSERT INTO Book_Store VALUES (11, "book", "deadly little lies", "laurie faria stolarz", "9", "9"); 
INSERT INTO Book_Store VALUES (12, "book", "deadly little voices", "laurie faria stolarz", "9", "10"); 
INSERT INTO Book_Store VALUES (13, "book", "verity", "colleen hoover", "16", "11");
INSERT INTO Book_Store VALUES (14, "book", "the mother in law", "karen king", "11", "12"); 
INSERT INTO Book_Store VALUES (15, "book", "the stranger in my bed", "karen king", "15", "13"); 
INSERT INTO Book_Store VALUES (16, "book", "the perfect stepmother", "karen king", "17", "14");
INSERT INTO Book_Store VALUES (17, "book", "bleed", "laurie faria stolarz", "15", "15");

SELECT * FROM Book_Store ORDER BY price;
SELECT aisle, SUM(price) FROM Book_Store GROUP BY author
