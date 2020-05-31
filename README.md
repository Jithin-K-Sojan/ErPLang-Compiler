# ErPLang-Compiler

This is a compiler built for the language defined according the language specifications file in the Auxiliary_Files Folder. It is a compiler built from scratch in the language C.

The stages of the compiler are mainly: Lexer, Parser, AstGenerator, SemanticAnalyser, IRCodeGenerator and the ASMGenerator. To create an executable for the compiler simply run the makefile in the folder: $ make

This will produce an executable called compiler which you can run with any of the test cases in the semanticAnalysisTestCases or codeGenTestCases as such. $ ./compiler <test-file.txt> <asm-file.asm>

On running the codeGenTestCases(which are semantically correct according to specifications) an asm file will be generated (<asm-file.asm>), which you can execute using the NASM assembler.

The driver is built such that you have to chose the stage upto which you want the compiler to run, it will either run upto that stage and give results specific to that stage, or stop at a previous stage if it encountered and error in it.

For details regarding the project, look into the Language specifications pdf, grammar.txt(Grammar rules for parser), astModified.txt(Abstract Syntax Tree gen rules), SemanticRules.txt(rules for Semantic Analysis) and the coding_details.docx file.
