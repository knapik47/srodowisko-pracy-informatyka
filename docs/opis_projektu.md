graph TD
    %% Definicja stylów
    classDef main fill:#e1f5fe,stroke:#01579b,stroke-width:2px,color:#01579b;
    classDef feature fill:#ffffff,stroke:#333,stroke-width:1px;
    classDef user fill:#f1f8e9,stroke:#33691e,stroke-width:2px;

    Start(Aplikacja wspierająca planowanie nauki) --> Target[Odbiorcy: Studenci 18-25 lat]
    
    Target --> PainPoints{Rozwiązuje problemy}
    PainPoints --> P1[Brak struktury]
    PainPoints --> P2[Przeciążenie informacjami]

    Target --> Features[Kluczowe Funkcje]
    subgraph "Narzędzia Organizacji"
        Features --> F1[Lista zadań]
        Features --> F2[Kalendarz tygodniowy]
        Features --> F3[Przypomnienia]
    end

    subgraph "Optymalizacja Pracy"
        Features --> F4[Priorytetyzacja zadań]
        Features --> F5[Statystyki postępów]
    end

    %% Przypisanie stylów
    class Start main;
    class Target user;
    class F1,F2,F3,F4,F5 feature;
