CalculatorApp.sln
│
├── CalculatorApp/
│   ├── Interfaces/
│   │   ├── ICalculator.cs
│   │   ├── IHistoryRepository.cs
│   │   ├── ICalculatorService.cs
│   │
│   ├── Models/
│   │   └── CalculationRecord.cs
│   │
│   ├── Services/
│   │   ├── Calculator.cs
│   │   ├── CalculatorService.cs
│   │   └── XmlHistoryRepository.cs
│   │
│   └── CalculatorApp.csproj

├── CalculatorApp.Tests/
│   │
│   ├── Unit/
│   │   ├── CalculatorTests.cs
│   │   ├── CalculatorServiceTests.cs
│   │   └── XmlHistoryRepositoryTests.cs
│   │
│   ├── Integration/
│   │   └── CalculatorIntegrationTests.cs
│   │
│   ├── TestData/
│   │   ├── sample-history.xml
│   │   ├── max-entries.xml
│   │   └── corrupt.xml
│   │
│   ├── Helpers/
│   │   ├── TestFileHelper.cs
│   │   └── TestDataFactory.cs
│   │
│   ├── TestDoubles/ (optional)
│   │   └── MockFactory.cs
│   │
│   └── CalculatorApp.Tests.csproj