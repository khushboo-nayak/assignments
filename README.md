## Assignments
# Task 1
Day 1:  
Preliminary Blockchain constructed, however ran infinetely without giving any errors. Problems with go routines and channels detected. Structs not defined properly and comparision was happening with a nil pointer initially. (given in assignment.go file)  

Day 2:  
  (i) Refined structs, made new structs  
 (ii) made a function to set up leveldb and also added file handling condition where the leveldb was already populated.  
(iii) Made a comprehensive function to process (validate + hash) all transactions concurrently  
 (iv) Made a function to commit valid transactions in batches (leveldb.batch)
 
Day 3:   
  (i) The for loop for processing and commiting transactions made with a configurable number of transactions, channel made to recieve commited blocks and hashing for each block  
 (ii) function made to recieve blocks from the channel and write it to a file  
(iii) wrote a function to fetch all blocks from file using os, scanner and finally unmarshal it to display  
 (iv)  wrote a function to fetch blocks by matching block number which calls the fetch all blocks function & finds the matching block; returns not found if no match  

  References:  
  1. https://medium.com/golangspec/in-depth-introduction-to-bufio-scanner-in-golang-55483bb689b4  
  2. https://www.slingacademy.com/article/using-sha-256-for-hashing-in-go-a-practical-guide/  
  3. https://rb.gy/3mju19  
  4. https://github.com/syndtr/goleveldb  
  5. https://medium.com/@ahamrouni/mastering-file-handling-in-go-build-a-todo-app-with-text-json-and-log-files-ec7814b2df4b  
              
