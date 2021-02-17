# DoThingScript
Create a programmable script to allow users to customize the logic safely
Used with C# applications

# Expected Features
- Support static typed variables/constants
- Primitive types: string, number, integer, boolean, guid
- Pre-defined object initialization
- Built-in functions and pre-defined functions
- Task functions for deferred execution
- Expression
- If then else statement
- Label and goto statement
- Error handling

# Examples

const Context // Predefined constant\
integer i = 1 // Variable\
IgnoreError(SendEmail("Template1", Context.Email)) // Task parameter\
Label Loop: // Label\
Group = GetCustomerGroup(Context.CustomerID) // Pre-defined function\
If (Group = "ABC") and (i > 10 or i < 0) // If conditions\
GetResult = GetRequest("https://test.com/api", Header("AUTH", "1234"))\
PostResult = PostRequest("https://test.com/api", Header("AUTH", "1234"), Header("Key", "Value"), Json("K1", "V1", "K2", "V2")) // Generic parameters handling\
Else // Else statement\
Parameter = NewObject("ObjectName", "Key1", "Value1", "Key2", i) // Generic constructor for object\
SpecialTask(Parameter) // Function\
i = i + 1 // Variable assignment\
GoTo Loop // Go to label statement\
EndIf // End if

Error: // Error handling\
IgnoreError(SendErrorEmail("dan@abc.com"))\
ErrorLog("Error occurred")\
ErrorLog(Exception)
