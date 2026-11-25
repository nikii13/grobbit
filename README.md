# Grobbit Compiler

A team compiler engineering project developed in Go for the Grobbit programming language. The compiler translates source programs into LLVM intermediate representation (IR).

## Structure
- `frontend/`: frontend components.
- `backend/`: backend and intermediate code generation.
- `common/` and `gen/`: shared and generated components.
- `tests/`: sample programs and tests.
- [Language reference](GrobbitLangRef_v16.pdf): language specification.

## Build and explore
The Go module specifies Go 1.27 and the ANTLR runtime. Clang is used for native compilation of generated LLVM IR.

```sh
go build -o Grobbit .
./Grobbit tests/icg/test_student.gr
```

See [build.sh](build.sh) for the project's original LLVM/Clang workflow. Generated output and runtime support may require additional setup.

## Credits
Collaborative university project. See [authors.txt](authors.txt) and the original [repository](https://github.com/Kristjan-HR/grobbit) for attribution and commit history.
