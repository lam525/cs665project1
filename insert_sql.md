insert_sql.md
the file to have SQL statements to populate tables.

INSERT INTO Cinema (CinemaName, CinemaAddress, CinemaZipcode, CinemaPhone)
VALUES 
	(West IMAX, 3350 W Mead, 33202, 344-5555555),
    (Center IMAX, 1234 Ridge, 33101, 333-5551234),
    (South Cinema, 9830 S Maize, 40240, 666-1232222),
    (North Cinema, 2563 N Tyler, 25620, 222-3451234),
    (East theater, 6903 E Hillside, 66890, 555-6785678);

    
INSERT INTO Movie (MovieName, director, starring, genre)
VALUES 
    (Violent Night,Tommy, John, Comedy),
    (),
    (),
    (),
    ();

INSERT INTO Ticket(MovieName, CinemaName, datetime, price)
VALUES 
    (Violent Night, West IMAX, 2022-12-09 15:45:21, 15),
    (),
    (),
    (),
    ();


INSERT INTO Projection(MovieName, datetime, roomNumber,seat)
VALUES 
    (Violent Night, West IMAX,2022-12-09 15:45:21, 17, 6J),
    (),
    (),
    (),
    ();


