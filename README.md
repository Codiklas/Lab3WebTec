# Lab3WebTec

## Author
- JOHANNESMEIER Niklas : Niklas.Johannesmeier@edu.ece.fr

## About this repository
This repository contains the Lab 3

    1. Typescript

        1.1 npm install
        1.2 npm start
        
        POST
        2.1 Open Postman
        2.2 Select "Post"
        2.3 Insert with sending "localhost:8080/metrics/1"
        JSON BODY:  [
                    { "timestamp":"1384686660555", "value":"15" },
                    { "timestamp":"1384686667777", "value":"186" }
                    ]
        2.4 The values are now inserted to our LevelDB

        GET
        2.1 Open Postman
        2.2 Select "GET"
        2.3 GET values with sending "localhost:8080/metrics/1"
        Recieve:    [
                    { "timestamp":"1384686660555", "value":"15" },
                    { "timestamp":"1384686667777", "value":"186" }
                    ]
        2.4 You receive these two values we inserted before

        DELETE
        2.1 Open Postman
        2.2 Select "DELETE"
        2.3 DELETE values with sending "localhost:8080/metrics/1" and the values you want to delete
        2.4 The requested entries get deleted