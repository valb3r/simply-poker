# simply-poker

# API sequence diagram (primary flow)
```puml
@startuml
Client -> "API gateway" : request
"API gateway" -> "Game engine"
"Game engine" -> "Rule engine" : action+context
"Rule engine" -> "Game engine" : rule to execute
"Game engine" -> "API gateway"
"API gateway" -> "Client" : response
@enduml
```

