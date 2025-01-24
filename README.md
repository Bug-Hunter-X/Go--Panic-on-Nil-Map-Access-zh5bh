# Go: Panic on Nil Map Access

This repository demonstrates a common error in Go: panicking due to accessing a nil map.  The `bug.go` file shows the problematic code, while `bugSolution.go` provides a solution.

The issue arises from directly accessing a map's elements (`m["a"]`) without first checking if the map is nil.  If it is, a runtime panic occurs.

The solution involves a simple nil check before accessing the map's elements, ensuring the program handles the absence of the map gracefully.

This example highlights the importance of defensive programming in Go, particularly when dealing with maps and other potentially nil values.