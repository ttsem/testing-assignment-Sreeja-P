1. Calculator Unit Tests

Functional Tests:
TC01: Add two positive numbers
TC02: Add negative numbers
TC03: Subtract two numbers
TC04: Multiply two numbers
TC05: Divide two numbers

Edge cases:
TC06: Divide by zero
TC07: Large number calculation
TC08: Decimal number calculation

2. Calculator Service Tests

Calculate():
TC09: Perform Add operation and return result
TC10: Perform Subtract operation
TC11: Perform Multiply operation
TC12: Perform Divide operation
TC13: Invalid operation should throw exception


History Handling
TC14: New calculation is added to history
TC15: History is saved after calculation
TC16: History appends new record correctly


History Limit
TC17: History below 10 entries → append normally
TC18: History exactly 10 → remove oldest and add new
TC19: History exceeds 10 → maintain only last 10


GetHistory()
TC20: Returns existing records
TC21: Returns empty list when no history


ClearHistory()
TC22: Clears all records
TC23: Saves empty list after clearing


3. XmlHistoryRepository (Persistence Tests)

Save()
TC24: Save valid records to XML
TC25: Save enforces max 10 record limit
TC26: Save overwrites existing file


Load()
TC27: Load valid XML file
TC28: Load empty XML file
TC29: Load when file does not exist


Error Handling
TC30: Load corrupt XML file
TC31: Handle invalid file path


Data Integrity
TC32: Data matches after Save & Load
TC33: Timestamp is preserved correctly

