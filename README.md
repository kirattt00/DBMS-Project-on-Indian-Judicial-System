erDiagram
  CITIZEN ||--o{ CASE : files
  CASE ||--|{ COURT : is-heard-in
  JUDGE ||--|{ CASE : oversees
  LAWYER ||--|{ CITIZEN : represents

  class CITIZEN {
    - Citizen_ID (PK)
    - Name
    - Age
    - Gender
    - Address
  }

  class CASE {
    - Case_ID (PK)
    - Case_Type
    - Case_Date
    - Status
    - Verdict_Date
  }

  class COURT {
    - Court_ID (PK)
    - Court_Name
    - Location
    - Type (Supreme, High, District)
  }

  class JUDGE {
    - Judge_ID (PK)
    - Name
    - Specialization
    - Experience
  }

  class LAWYER {
    - Lawyer_ID (PK)
    - Name
    - Expertise
    - Contact
  }
