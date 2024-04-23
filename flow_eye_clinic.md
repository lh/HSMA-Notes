
```mermaid
graph TD;
    Start --> Triage;
    Triage --> |Urgent Care| EyeCasualty;
    Triage --> |Non-Urgent| NurseTreatmentRoom;
    EyeCasualty --> Examination;
    Examination --> |Order Tests| OphthalmicImagingRoom;
    Examination --> |Order Tests| VisualAcuityRoom;
    OphthalmicImagingRoom  --> WaitingRoom;  
    VisualAcuityRoom --> WaitingRoom;
    WaitingRoom --> Examination;
    WaitingRoom --> VisualAcuityRoom;
    WaitingRoom --> OphthalmicImagingRoom;
    ReviewExamination --> Diagnosis;
    Diagnosis --> Treatment;
    Treatment --> End;
    End --> WriteCaseNotes;
    NurseTreatmentRoom --> End;
    Treatment --> WaitingRoom;
    WaitingRoom --> |Tests Completed| ReviewExamination;
```