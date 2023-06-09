## Pre-requistes

There should be local instance of elastic search running at - http://localhost:9200

## Google Books Script

This python script calls various google books API and publish it in elastic search index

This python script internally calls the endpoint - https://www.googleapis.com/books/v1/volumes

## Google Books Java Service

This service exposed API using Spring Boot, Spring WebFlux from Elastic search index and with its search feature.

```
curl --location 'http://localhost:8080/api/v1/books?search=Harry Porter'
```

```
curl --location 'http://localhost:8080/api/v1/books/fetchAllBooks
```

## High Level Design for Google Books Search Engine

![image](https://github.com/coding-nomadic/google-books-search-engine/assets/8009104/dc000bbb-9e62-49df-80fb-b950a7af32f2)


## Google Books Engine UI

This is the Search Engine UI built with React JS auto-complete and CSS. It calls the Java API endpoints, renders data on the UI.

![image](https://github.com/coding-nomadic/google-books-search-engine/assets/8009104/dacc88cf-17cc-4db4-8f6c-864fae0d05c3)







