## Github Organization: [describe the physical location of all major files and deliverables (code, tests, data, the written report, the presentation video, etc…)]

├───.idea
│   └───inspectionProfiles
├───.vscode
├───build
│   ├───CMakeFiles
│   │   ├───3.22.1
│   │   │   ├───CompilerIdC
│   │   │   │   └───tmp
│   │   │   └───CompilerIdCXX
│   │   │       └───tmp
│   │   ├───CMakeTmp
│   │   ├───main.dir
│   │   │   └───entry
│   │   └───test.dir
│   │       └───tests
│   ├───lib
│   │   └───CMakeFiles
│   │       ├───cs225.dir
│   │       │   └───cs225
│   │       └───lodepng.dir
│   │           └───lodepng
│   └───src
│       └───CMakeFiles
│           └───src.dir
├───cmake-build-debug
│   ├───.cmake
│   │   └───api
│   │       └───v1
│   │           ├───query
│   │           └───reply
│   ├───CMakeFiles
│   │   ├───3.22.1
│   │   │   ├───CompilerIdC
│   │   │   │   └───tmp
│   │   │   └───CompilerIdCXX
│   │   │       └───tmp
│   │   ├───CMakeTmp
│   │   ├───main.dir
│   │   │   └───entry
│   │   └───test.dir
│   │       └───tests
│   ├───lib
│   │   └───CMakeFiles
│   │       ├───cs225.dir
│   │       │   └───cs225
│   │       └───lodepng.dir
│   │           └───lodepng
│   ├───src
│   │   └───CMakeFiles
│   │       └───src.dir
│   └───Testing
│       └───Temporary
├───entry
├───lib
│   ├───cs225
│   └───lodepng
├───src
└───tests
    └───data
        ├───csv
        └───json



## Running Instructions

### Installation:

Clone the repo by running the command below in whatever folder you want to save the project in:
git clone https://github.com/LohitoBurrito/Airport-Project.git

Open up and turn on your cs225 Docker environment.
If you do not have it, follow the instructions here: ___.

Open the folder in VS Code.
Then run the following commands:
cd Airports=Project
mjkdir build
cd build
cmake ..

Now, you have created the build file and are ready to test :)

To test, runt he following commands in the build folder:
make test
./test
(this process will take a while as it parses through around 8k datapoints of airports)

If you want to test specific test cases, run:
make test
./test "test_case_name"
(fill test_case_name with the specified name of the test case)

If you want to run the main program, run the following commands:
make main
./main

You will then be prompted to enter your current latitude and longitude, destination latitude and longitude, as well as the number of baggage you will be travelling with. 
You will receive the status notifications in the console.
Given your current location and destination location, the BFS algorithm will find your start and end airport nodes. If these nodes are the same, the console will print all the connected components to your start airport using Kosaraju algorithm. Otherwise, it will provide the most cost effective route from your start airport to your end airport using Dijstkra's algorithm. 


.idea
  |_
  |_sㄴ 
