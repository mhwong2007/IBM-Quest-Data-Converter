# IBM-Quest-Data-Converter
This program will convert the synthetic data generated by IBM Quest Data Generator to Weka compatible csv format

# Usage
`java DataConverter [option] [input file] [output file]`

`java DataConverter -help` for more information

## Convert From IBM Quest Ascii Data to Weka Compatible CSV (Relational Data)
IBM Ascii Data Format:
```
CustId	TransId	Item
1	1	898
1	1	987
2	2	1
```

Weka Compatible CSV (Relational Data)
```
898, 987, 1
t, t,
, , t
```

## Convert From Conventional CSV (Transactional Data) to Weka Compatible CSV (Relational Data)
Conventional CSV (Transactional Data)
```
898, 987
1
```

Weka Compatible CSV (Relational Data)
```
898, 987, 1
t, t,
, , t
```

## Convert From IBM Quest Ascii Data to Conventional CSV (Transactional Data)
IBM Ascii Data Format:
```
CustId	TransId	Item
1	1	898
1	1	987
2	2	1
```

Conventional CSV (Transactional Data)
```
898, 987
1
```

## Separate IBM Quest Ascii Data with Comma
```
CustId	TransId	Item
1	1	898
1	1	987
2	2	1
```
```
CustId, TransId, Item
1,	1,	 898
1,	1,	 987
2,	2,	 1
```

# Option
Option:

	-a	 Convert ascii data from IBM Quest Data Generator to Weka compatible csv
	-b	 Convert conventional csv to Weka compatible csv
	-c	 Convert ascii data from IBM Quest Data Generator to conventional csv
	-d	 Separate ascii data from IBM Quest Data Generator with comma
