# Epsilon-NFA to NFA Converter

This program converts a Non-deterministic Finite Automaton (NFA) with epsilon transitions ($\epsilon$-NFA) into an equivalent NFA without epsilon transitions.

## Prerequisites

- **GCC Compiler**: Ensure you have MinGW or any GCC-based compiler installed.

## How to Run

### 1. Compile the code
Open your terminal in the project directory and run:
```powershell
gcc epsilon-transition.c -o epsilon-transition.exe
```

### 2. Run the program
You can run it manually and type the input, or use the provided `input.txt`:

**Using input redirection (Recommended):**
```powershell
Get-Content input.txt | .\epsilon-transition.exe
```

**Manual execution:**
```powershell
.\epsilon-transition.exe
```

## Input Format
The program expects input in the following order:
1. Number of states.
2. Number of symbols.
3. The symbols (as a string, e.g., `ab`).
4. Transitions for each state and symbol (including epsilon).
5. Start state.
6. Number of final states followed by the final states.

Refer to `input.txt` for a complete example.
