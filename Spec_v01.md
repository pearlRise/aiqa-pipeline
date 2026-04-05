# AIQA-Pipeline

## About Document

1. Title    aiqa-pipeline
2. Version  v0.1.0
3. Update   2026.04.05
4. Author   pearlRise
5. Status   WIP

## Details

```sequenceDiagram

    autonumber
    participant W as Workstation
    participant T as Terminal
    participant D as DUT

    W->>T: Transfer TestLogic

    loop TestExecution
        T->>D: capture screen
        T->>T: Analysis
        T->>D: Control UI
    end

    T->>W: Transfer TestResult
    W->>W: Analyze TestResult
    
```