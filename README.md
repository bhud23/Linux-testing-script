# Linux-testing-script
A Bash script for testing the IO correctness of an executable based on a provided sample executable.

Compile this into an executable and store in in your bin directory to access it whenever.

Run program as follows:

./runSuite suiteOfTests.txt ./programToTest ./sampleProgram

- the file suiteOfTests.txt is a list of file names (not including extensions)
- for each file name in suiteOfTests.txt, there must be an corresponding .in and .args files (which can optionally be blank)
- for each test in the test suite, if the results of running ./programToTest does not match the results of ./sampleProgram an error will be produced