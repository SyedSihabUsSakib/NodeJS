**NodeJS**

- Event based architecture (as uses callback functions to send client the response)
- **JS** runtime built with Chrome's V8 **JS** engine which can run in the server side also
  +Chrome's V8 engine only had access to the DOM but with NodeJS we can do alot more
- Its not a programming language
- But **JS** is a programming language which brings dynamic functionality to the website
- Chorome's v8 engine(built with c++) + Ryan Dahls C++ code == NodeJS # So basically NodeJS is nothing but a C++ program
- **JS** is a single threaded language
  - So **NodeJS** operates like its single thread accepts only the requests from the client but never waits for the response. Thats why it can handle multiple requests from client at a single time
  - It has two methods: 1. Asynchronous (Uses call back funtions) 2. Non-Blocking I/O
  - That is why **NodeJS** is not suitable **for highly CPU intensive task** but suitable for I/O intensive task (getting data from backend etc.)
- **Event Loop** is kind of a while loop who takes each of the tasks and assigns to the external system(workers-->**Thread Pool**) which ultimately forwards the request to the server and gets the respons and via call back it resend the response to the client
- After 10.5 version NodeJS introduced multithreading (worker thread)
  - Worker Thread is created by **LibUV** library which is built using **C Language** which contacts with **Kernel** which has multiple thread and contacts with OS
