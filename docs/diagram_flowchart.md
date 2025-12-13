``` mermaid
flowchart TD
    Student[Student 18-25] --> App

    subgraph App[Aplikacja Planowania Nauki]
        Tasks[Lista zadan]
        Calendar[Kalendarz tygodniowy]

        Priority[Priorytetyzacja]
        Reminders[Przypomnienia]
        Pomodoro[Pomodoro]
        AI[AISugestie]

        Stats[Statystyki]
        Data[Baza danych]

        ImportExport[Import Export Sync]
        Backup[Backup]
    end

    Tasks --> Priority
    Priority --> Tasks
    Priority --> Calendar

    Tasks --> Reminders
    Calendar --> Reminders

    Tasks --> Pomodoro
    Calendar --> Pomodoro

    Tasks --> AI
    Calendar --> AI

    Tasks --> Stats
    Calendar --> Stats
    Stats --> Data

    ImportExport --> Data
    Data --> Backup
```
