# ESEP Grade Calculator

This library is a simple utility to calculate your grades. Each assigment type has different weights.

Runtime requirements:
Golang 1.24+

Run unit tests:
```
cd grade-calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade-calculator/
go test -coverprofile=coverage.txt ./...
```

Example usage:
```go
gc := NewGradeCalculator()
gc.AddGrade("open source assignment", 100, Assignment)
gc.AddGrade("exam 1", 100, Exam)
gc.AddGrade("essay on ai ethics", 100, Essay)

gc.GetFinalGrade() //returns "A"
```
