# python-telnet_test

This is a python software to automate telnet testing.

The result can be shown on terminal, exported to text file or even exported to CSV file.

The test suites can be input as the following Python list.

    Test_List = [
        {"Destination IP": "192.168.11.20", "Destination TCP Port": ["20:20","138","21:23","139"]},
        {"Destination IP": "192.168.11.21", "Destination TCP Port": ["19-19","20-24","21:23","139","139"]}
    ]

Then the necessary tests will be automated by the code.

