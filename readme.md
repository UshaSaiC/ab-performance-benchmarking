Site used for ab benchmarking - https://dummy.restapiexample.com/

Basic command -
ab [options...] URL

In options -
-c -> concurrent clients
-n -> number of requests to run
URL -> URL to be tested on

Get -
ab -c 10 -n 2000 http://dummy.restapiexample.com/api/v1/employee/1 > ./output/get.txt

Post -
ab -p ./input/post.json -c 10 -n 2000 http://dummy.restapiexample.com/api/v1/create > ./output/post.txt
-p -> post a json