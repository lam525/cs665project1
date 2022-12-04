create_sql.md
the file to have SQL statements to create all tables.

CREATE TABLE Cinema (
        CinemaName VARCHAR(20), 
        CinemaAddress VARCHAR(50), 
        CinemaZipcode VARCHAR(5), 
        CinemaPhone VARCHAR(15)
        PRIMARY KEY (CinemaName)
);

CREATE TABLE Movie (
        MovieName VARCHAR(50), 
        director VARCHAR(50), 
        starring VARCHAR(5), 
        genre VARCHAR(10)
        PRIMARY KEY (MovieName)
);

CREATE TABLE Ticket (
        MovieName VARCHAR(50), 
        CinemaNamee VARCHAR(20), 
        datetime DATETIME, 
        price DECIMAL(10,2)
        PRIMARY KEY (MovieName, CinemaName)
);

CREATE TABLE Ticket (
        MovieName VARCHAR(50), 
        CinemaNamee VARCHAR(20), 
        datetime DATETIME, 
        price DECIMAL(10,2)
        PRIMARY KEY (MovieName, CinemaName, datetime)
);

CREATE TABLE Projection (
        MovieName VARCHAR(50), 
        CinemaNamee VARCHAR(20), 
        datetime DATETIME, 
        seat VARCHAR(5),
        PRIMARY KEY (MovieName, CinemaName,datetime)
);
