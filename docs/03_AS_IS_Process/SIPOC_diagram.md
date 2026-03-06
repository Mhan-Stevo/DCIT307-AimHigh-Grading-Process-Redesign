# SIPOC Diagram
## Student Grading and Report Generation Process
### Aim High School Complex

The SIPOC diagram provides a high-level overview of the grading process by identifying Suppliers, Inputs, Process steps, Outputs, and Customers.

```mermaid
flowchart LR

subgraph Suppliers
A1[Teachers]
A2[Students]
A3[Exam Office]
end

subgraph Inputs
B1[Student Scores]
B2[Exam Scripts]
B3[Assessment Records]
end

subgraph Process
C1[Enter Scores in Excel]
C2[Save Subject Sheets]
C3[Submit Files to Admin]
C4[Consolidate Subject Results]
C5[Calculate Totals and Averages]
C6[Rank Students]
C7[Generate Report Cards]
C8[Print Reports]
end

subgraph Outputs
D1[Student Reports]
D2[Class Rankings]
D3[Academic Performance Records]
end

subgraph Customers
E1[Students]
E2[Parents]
E3[School Administration]
end

A1 --> B1
A2 --> B2
A3 --> B3

B1 --> C1
B2 --> C1
B3 --> C1

C1 --> C2 --> C3 --> C4 --> C5 --> C6 --> C7 --> C8

C8 --> D1
C6 --> D2
C5 --> D3

D1 --> E1
D1 --> E2
D3 --> E3
```