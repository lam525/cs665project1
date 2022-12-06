crud_sql.md
the file to perform CRUD using SQL

--insert, add a movie
INSERT INTO Movie (MovieName, director, starring, genre)
VALUES  ('She Said','Maria', 'Carey', 'Biography');


--update the price of the movie if 10 tickets are sold 
UPDATE Ticket
SET price = 20.00
WHERE MovieName IN (SELECT MovieName FROM Ticket GROUP BY MovieName HAVING COUNT(*) > 10);


--select movies that are available in West IMAX
SELECT MovieNAME FROM Ticket 
WHERE CinemaName = "West IMAX";

--select cinemas that play movie Black Panther: Wakanda Forever
SELECT CinemaName FROM Ticket 
WHERE MovieNAame = "Black Panther: Wakanda Forever";

--select movies and locations that only cost 10 dollar, join table
SELECT MovieName, CinemaName,CinemaAddress, price FROM Ticket, Cinema 
WHERE price = 10.00;


--remove the movie if only 3 tickets are sold
DELETE FROM Movie
where MovieName in (SELECT MovieName FROM Ticket GROUP BY MovieName HAVING COUNT(*) <=3);

--trigger, delete cinema
CREATE TRIGGER cinema_down
AFTER DELETE 
ON Cinema
FOR EACH ROW
UPDATE Movie
SET CinemaName = NULL
WHERE CinemaName NOT EXISTS (SELECT CinemaName FROM Cinema);






