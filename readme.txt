This repo can be used to setup a visual studio project with cmake.

The aim is to try and build something minimal that will replicate
the issue with have with Vs freezing when googletests are clicked
in the test explorer somewhere between iversions 16.11.20 (no issue)
and 16.11.22 (vs freezes)

In order to create the project you should

- Download cmake-3.20.3-windows-x86_64.zip from https://cmake.org/files/v3.20/ and
   unzip inside the repo and the rename the folder to cmdist
- Download googletest tag 'release-1.11.0' from https://github.com/google/googletest/tree/release-1.11.0
   and extract in the repo
- create a directory called 'build' inside the repo
- Open a VS2019 x64 command prompt, chnage to the repo directory and run gen.bat

You should now have a solution file called vsfreezetest.sln inside the build directory.
Open this isnide visual studio, and build the solution.

There should be 4 googltests in the test explorer.
