db_description.md
A description of your database, including tables, attributes, primary keys, foreign keys, foreign key constraints, FDs, whether in 3NF, and one or two rows of sample data for each table

This database is desiged for a simple online movie ticket booking application. User can use this application to check what movie is avaible at certain time and location.


Cinema(CinemaName, CinemaAddress, CinemaZipcode, CinemaPhone)
Cinema(West IMAX, 3350 W Mead, 33202, 344-5555555)
Cinema will hold the cinema's infomation.
CinemaName is the primary key.
CinemaName -> CinemaAddress,CinemaZipcode, CinemaPhone
They are in 3NF.

Movie(MovieName, director, starring, genre)
Movie(Violent Night,Tommy, John, Comedy)
This object Movie will hold all the infomations of a specific movie.
MovieName is the primary key.
MovieName -> director, starring, genre
They are in 3NF.

Ticket(MovieName, CinemaName, datetime, price)
Ticket(Violent Night, West IMAX, 2022-12-09 15:45:21, 15)
This object Ticket will hold the ticket info.
MovieName, cinemaName,datetime are the primary keys.
MovieName, cinemaName, datetime -> price
They are in 3NF.

Projection(MovieName, datetime, roomNumber,seat)
Projection(Violent Night, West IMAX,2022-12-09 15:45:21, 17, 6J)
This object Projection will hold the seating info.
MovieName, datetime, roomNumber are the primary key.
MovieName, datetime, roomNumber -> seat
They are in 3NF.









