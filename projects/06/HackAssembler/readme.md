# Hack Assembler

This is an assembler for converting the Hack assembly language to the Hack machine code as described on [www.nand2teris.org/06.php](//nand2tetris.org/06.php).

## Usage

```bash
git clone https://github.com/shreyasminocha/nand2tetris.git
cd nand2tetris/projects/06/HackAssembler
ln -s myassembler.sh [PATH TO BINARIES]/assembler
```

```bash
assembler --help
```

## Running tests

```bash
cd path/to/project/06
./test.sh [PATH TO BUILT-IN ASSEMBLER] HackAssembler/assembler.sh */**/*.asm
```
## Documentation

Find `javadocs` generated documentation in the `docs/` folder.
