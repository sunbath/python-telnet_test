# python-telnet_test

This is a python software to automate telnet testing.

The result can be shown on terminal, exported to text file or even exported to CSV file.

The test suites can be input as the following Python list.

    Test_List = [
        {"Destination IP": "192.168.11.20", "Destination TCP Port": ["20:20","138","21:23","139"]},
        {"Destination IP": "192.168.11.21", "Destination TCP Port": ["19-19","20-24","21:23","139","139"]}
    ]

The necessary tests will be automated by the code and output as follows:

╒════════════════════╤════════════════════════════════╕
│ Source IP:         │ 192.168.11.4                   │
├────────────────────┼────────────────────────────────┤
│ Testing Start Time │ 2018-12-28 00:13:54.252952 HKT │
├────────────────────┼────────────────────────────────┤
│ Testing End Time   │ 2018-12-28 00:13:59.768170 HKT │
├────────────────────┼────────────────────────────────┤
│ Completed in       │ 0:00:05.515218                 │
╘════════════════════╧════════════════════════════════╛
╒══════════════════╤════════════════════════╤══════════════════════╤════════════════════════════════╕
│ Destination IP   │ Destination TCP Port   │ Telnet Test Result   │ Test Time                      │
╞══════════════════╪════════════════════════╪══════════════════════╪════════════════════════════════╡
│ 192.168.11.20    │                        │                      │                                │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 20                     │ Telnet Failed        │ 2018-12-28 00:13:54.386906 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 21                     │ Telnet Succeeded     │ 2018-12-28 00:13:54.437872 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 22                     │ Telnet Succeeded     │ 2018-12-28 00:13:54.512037 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 23                     │ Telnet Failed        │ 2018-12-28 00:13:54.607889 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 138                    │ Telnet Failed        │ 2018-12-28 00:13:54.698637 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 139                    │ Telnet Succeeded     │ 2018-12-28 00:13:54.750570 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│ ---              │ ---                    │ ---                  │ ---                            │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│ 192.168.11.21    │                        │                      │                                │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 19                     │ Telnet Failed        │ 2018-12-28 00:13:55.753849 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 20                     │ Telnet Failed        │ 2018-12-28 00:13:56.757332 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 21                     │ Telnet Failed        │ 2018-12-28 00:13:57.760337 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 22                     │ Telnet Failed        │ 2018-12-28 00:13:58.762968 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 23                     │ Telnet Failed        │ 2018-12-28 00:13:59.767203 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 24                     │ Telnet Failed        │ 2018-12-28 00:13:59.767706 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│                  │ 139                    │ Telnet Failed        │ 2018-12-28 00:13:59.768053 HKT │
├──────────────────┼────────────────────────┼──────────────────────┼────────────────────────────────┤
│ ---              │ ---                    │ ---                  │ ---                            │
╘══════════════════╧════════════════════════╧══════════════════════╧════════════════════════════════╛
