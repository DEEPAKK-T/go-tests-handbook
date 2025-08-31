Red, Green, Refactor — A Go project demonstrating test-driven development, making it easy to learn and write effective test cases in Go.

go-tests/
├── README.md
├── 01_basic_tests/
├── 02_table_driven_tests/
├── 03_mocks/
├── 04_integration_tests/
├── 05_benchmark_tests/
└── go.mod

# Steps to run the tests

go test ./... -v

# ./...

./...

./ => current directory (repo root).

... => recursive wildcard in Go.

Together ./... means “run tests in this directory and all its sub-packages recursively”.

# -v : Stands for verbose.

By default, go test only shows output if a test fails.

With -v, it prints:

Which package is being tested

Which tests ran

Which tests passed
