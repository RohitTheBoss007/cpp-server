# cpp-server

HTTP server implemented in C++ without any third party library.

* Only Used "sys/socket.h" "pthread.h" and "mutex" which are standard libraries 

## Features

* Implemented only using GNU C/C++ Library
* Handles GET/POST requests
* Asynchronous request handling
* Multithreaded/Thread Pooling
* Handles over 20,000 concurrent connections.
* Serves over 100,000 requests per second on a modern personal computer

## Compile and Run
```sh
 g++ -pthread main.cpp html_parser.cpp -o server
./server
```
### Run
It is basic dictionary app. With 2 functions add word to dictionary and check if word contains in the dictionary

* Check word if it is in the dictionary  with Get Request 
```sh
http://127.0.0.1/check?name=EXAMPLE_WORD
```
* Add word to the dictionary with Post Request 
```sh
http://127.0.0.1/add
Body should contain raw text => "name=test_word"
```

![](https://i.imgur.com/9H5LdpH.png)




