insert_sql.md
the file to have SQL statements to populate tables.

INSERT INTO Cinema (CinemaName, CinemaAddress, CinemaZipcode, CinemaPhone)
VALUES 
	('West IMAX', '3350 W Mead', '33202', '344-5555555'),
    ('Center IMAX', '1234 Ridge', '33101', '333-5551234'),
    ('South Cinema', '9830 S Maize', '40240', '666-1232222'),
    ('North Cinema', '2563 N Tyler', '25620', '222-3451234'),
    ('East theater', '6903 E Hillside', '66890', '555-6785678');

    
INSERT INTO Movie (MovieName, director, starring, genre)
VALUES 
    ('Violent Night','Tommy', 'John', 'Comedy'),
    ('Strange World', 'Don Hall', 'Nik', 'Animation'),
    ('Black Panther: Wakanda Forever', 'Ryan', 'Letitia Wright', 'Action'),
    ('The Menu', 'Mark', 'Anya Taylor-Joy', 'Horror/Comedy'),
    ('Devotion', 'J. D. Dillard', 'Glen Powell', 'Action');

INSERT INTO Ticket(MovieName, CinemaName, datetime, price)
VALUES 
    ('Violent Night', 'West IMAX', 2022-12-09 15:45:21, 15.00),
    ('Strange World', 'Center IMAX', 2022-12-06 14:30:10,15.00 ),
    ('Black Panther: Wakanda Forever', 'West IMAX', 2022-12-05 22:55:21,20.00),
    ('The Menu', 'Center IMAX', 2022-12-07 13:25:00, 10.00 ),
    ('Devotion', 'Center IMAX', 2022-12-08 23:25:00,15.00 );


INSERT INTO Projection(MovieName, CinemaName datetime, roomNumber,seat)
VALUES 
    ('Violent Night', 'West IMAX',2022-12-09 15:45:21, 17, '6J'),
    ('Strange World', 'Center IMAX', 2022-12-06 14:30:10, 6, '3K' ),
    ('Black Panther: Wakanda Forever', 'West IMAX', 2022-12-05 22:55:21,5, '9H'),
    ('The Menu', 'Center IMAX', 2022-12-07 13:25:00, 3, '8J'),
    ('Devotion', 'Center IMAX', 2022-12-08 23:25:00,11, '5F');
   

