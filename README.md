# 🧪 Go Tests Handbook

**Red, Green, Refactor** — A Go project demonstrating **Test-Driven Development (TDD)**, making it easy to learn and write effective test cases in Go.  
This repository is structured like a **handbook** with examples ranging from basic tests to integration and benchmarks.

---

## Project Structure

```bash
go-tests-handbook/
├── README.md
├── go.mod
├── 01_basic_tests/
├── 02_table_driven_tests/
├── 03_mocks/
├── 04_integration_tests/
├── 05_benchmark_tests/
└── docs/

```

- **01_basic_tests/** → Simple tests to get started
- **02_table_driven_tests/** → Idiomatic Go table-driven tests
- **03_mocks/** → Unit tests with mocking (`testify/mock`, interfaces)
- **04_integration_tests/** → Database / HTTP / file integration tests
- **05_benchmark_tests/** → Performance benchmarks with `go test -bench`
- **docs/** → Notes on TDD, mocking, and Go testing best practices

---

## Running the Tests

Run all tests in the project (recursively) with:

```bash
go test ./... -v

```

## Explanation

./... → run tests in current directory and all sub-packages

-v → verbose mode, shows:

Which package is being tested

Which tests ran

Which tests passed

Example output:

=== RUN TestSum
--- PASS: TestSum (0.00s)
PASS
ok github.com/deepakkt/go-tests-handbook/01_basic_tests 0.123s

TDD Cycle: Red, Green, Refactor

Red → Write a failing test first

Green → Write minimal code to make the test pass

Refactor → Clean up code and tests

This repo demonstrates this cycle step by step.

## Learning Goals

- How to write unit tests in Go
- Using table-driven tests (idiomatic Go style)
- Creating and using mocks
- Writing integration tests (databases, APIs)
- Measuring performance with benchmarks
- Following the TDD workflow effectively

## Contributing

**Contributions are welcome!**

- Fork this repo
- Create a feature branch (git checkout -b feature/your-example)
- Commit your changes (git commit -m "feat: add new test example")
- Push to your branch and open a PR
- See CONTRIBUTING.md for details.

## License

This project is licensed under the MIT License

## About

This is a learning-focused project to master Go testing and TDD while keeping the repo clear and beginner-friendly.
Built with by Deepak K T.
