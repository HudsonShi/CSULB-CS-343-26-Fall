# Mermaid UML and Database Demos

These examples use English labels and are ready to paste into Markdown files that support Mermaid.

## 1. Library Database Schema (ER Diagram)

```mermaid
erDiagram
    MEMBER ||--o{ LOAN : borrows
    BOOK ||--o{ LOAN : appears_in
    MEMBER {
        int member_id PK
        string full_name
        string email UK
        date joined_on
    }
    BOOK {
        int book_id PK
        string isbn UK
        string title
        string author
        string status
    }
    LOAN {
        int loan_id PK
        int member_id FK
        int book_id FK
        date borrowed_on
        date due_on
        date returned_on
    }
```

## 2. Bank Transfer Workflow (Activity / Flowchart)

```mermaid
flowchart TD
    Start([Start]) --> Enter[Enter recipient and amount]
    Enter --> Valid{Is the input valid?}
    Valid -- No --> Fix[Show validation error]
    Fix --> Enter
    Valid -- Yes --> Funds{Enough balance?}
    Funds -- No --> Reject[Reject transfer]
    Reject --> End([End])
    Funds -- Yes --> Review[Show transfer summary]
    Review --> Confirm{User confirms?}
    Confirm -- No --> Cancel[Cancel transfer]
    Cancel --> End
    Confirm -- Yes --> Debit[Debit sender account]
    Debit --> Credit[Credit recipient account]
    Credit --> Record[Create transaction record]
    Record --> Notify[Send confirmation notification]
    Notify --> End
```

## 3. Bank Transfer Interaction (Sequence Diagram)

```mermaid
sequenceDiagram
    actor Customer
    participant App as Banking App
    participant Auth as Authentication Service
    participant Ledger as Account Ledger
    participant Notify as Notification Service

    Customer->>App: Submit transfer request
    App->>Auth: Verify session and 2FA code
    Auth-->>App: Authentication result
    alt Authentication failed
        App-->>Customer: Show access denied message
    else Authentication passed
        App->>Ledger: Check balance and reserve funds
        alt Insufficient balance
            Ledger-->>App: Reservation rejected
            App-->>Customer: Show insufficient funds message
        else Funds available
            Ledger-->>App: Reservation accepted
            App->>Ledger: Post debit and credit entries
            Ledger-->>App: Transfer completed
            App->>Notify: Send transfer receipt
            Notify-->>Customer: Confirmation email or push message
            App-->>Customer: Show successful transfer
        end
    end
```

## 4. Object-Oriented Banking Model (Class Diagram)

```mermaid
classDiagram
    class Customer {
        -String customerId
        -String fullName
        +requestTransfer(amount, recipient)
    }
    class Account {
        <<abstract>>
        -String accountNumber
        -Decimal balance
        +credit(amount)
        +debit(amount)
        +getBalance() Decimal
    }
    class CheckingAccount {
        -Decimal overdraftLimit
        +debit(amount)
    }
    class SavingsAccount {
        -Decimal interestRate
        +applyInterest()
    }
    class Transfer {
        -String transferId
        -Decimal amount
        -TransferStatus status
        +execute()
        +cancel()
    }

    Customer "1" --> "1..*" Account : owns
    Customer "1" --> "0..*" Transfer : initiates
    Transfer "1" --> "1" Account : sender
    Transfer "1" --> "1" Account : recipient
    Account <|-- CheckingAccount
    Account <|-- SavingsAccount
```

## 5. User Login with Two-Factor Authentication (Sequence Diagram)

```mermaid
sequenceDiagram
    actor User
    participant Web as Web App
    participant Identity as Identity Service
    participant Email as Email Service

    User->>Web: Enter email and password
    Web->>Identity: Validate password
    alt Invalid password
        Identity-->>Web: Invalid credentials
        Web-->>User: Display login error
    else Valid password
        Identity->>Email: Send one-time password
        Email-->>User: Deliver OTP
        User->>Web: Enter OTP
        Web->>Identity: Verify OTP
        alt OTP is valid
            Identity-->>Web: Issue access token
            Web-->>User: Open dashboard
        else OTP is invalid or expired
            Identity-->>Web: Reject OTP
            Web-->>User: Ask for a new OTP
        end
    end
```

## 6. To-Do List Application (Class Diagram)

```mermaid
classDiagram
    class User {
        +String userId
        +String name
        +createTask(title)
    }
    class TaskList {
        +String listId
        +String name
        +addTask(task)
        +removeTask(taskId)
    }
    class Task {
        +String taskId
        +String title
        +TaskStatus status
        +Date dueDate
        +markComplete()
    }
    class Tag {
        +String name
        +String color
    }

    User "1" *-- "1..*" TaskList : owns
    TaskList "1" *-- "0..*" Task : contains
    Task "0..*" --> "0..*" Tag : labeled with
```

## 7. Book Borrowing Process (Activity / Flowchart)

```mermaid
flowchart LR
    Member[Member requests a book] --> Search[Find the book]
    Search --> Available{Available now?}
    Available -- No --> Queue[Offer a reservation]
    Queue --> Done([Finish])
    Available -- Yes --> Eligible{Member may borrow?}
    Eligible -- No --> Explain[Explain borrowing restriction]
    Explain --> Done
    Eligible -- Yes --> CreateLoan[Create loan record]
    CreateLoan --> Update[Set book status to checked out]
    Update --> Receipt[Send due-date receipt]
    Receipt --> Done
```
