# csharp-patient-management-system

A console-based **Clinical Patient Management System (CPMS)** built in C# (.NET 8). The application allows healthcare administrators to manage a fixed-size patient registry directly from the terminal — adding, removing, searching, displaying, and exporting patient records.

---

## 📋 About the Project

This project was developed as part of a second-year programming assessment (Q2, Y2, 2025). It demonstrates core object-oriented programming principles in C#, including class design, static methods, array manipulation, file I/O, and console-based user interaction.

The system stores up to **10 patient records** (configurable via a constant) and can optionally pre-load patients from a CSV file (`10_patients.txt`) on startup.

---

## 🚀 Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- A terminal (macOS/Linux) or Command Prompt / PowerShell (Windows)

### Clone the Repository

```bash
git clone https://github.com/your-username/csharp-patient-management-system.git
cd csharp-patient-management-system
```

### Build the Project

```bash
dotnet build Question_1/Question_2.csproj
```

### Run the Project

```bash
dotnet run --project Question_1/Question_2.csproj
```

---

## 🖥️ How to Use

On launch, the system attempts to pre-load 10 patients from `10_patients.txt` (if present). A menu is then displayed:

```
1. Add Patient
2. Remove Patient
3. Search Patient
4. Display All Patients
5. Print Patient Information to File
6. Exit

Enter your choice:
```

| Option | Description |
|--------|-------------|
| **1. Add Patient** | Prompts for name, age, and medical condition. Stores the patient in the next available array slot. Displays an error if the array is full. |
| **2. Remove Patient** | Prompts for a patient name. Removes the matching record or displays a "not found" message. |
| **3. Search Patient** | Prompts for a patient name. Displays full details (name, age, medical condition) if found, or an error if not. |
| **4. Display All Patients** | Lists all current patient records. Notifies the user if no records exist. |
| **5. Print to File** | Exports all patient records to `patient_information.txt` on the current user's Desktop. |
| **6. Exit** | Displays a farewell message and closes the application. |

> **Input validation** is included — non-integer input and out-of-range choices are handled with descriptive error messages.

---

## 📁 Project Structure

```
CSharp-CPSM-Q2-Y2-2025/
├── Question_2.sln
├── Requirements.txt
├── README.md
└── Question_1/
    ├── CPMS.cs          # Patient class with all management methods
    ├── Program.cs       # Entry point — menu loop and user interaction
    └── Question_2.csproj
```

---

## 🛠️ Built With

- **C#** — Primary language
- **.NET 8** — Target framework
- **System.IO** — File reading and writing
- **Console I/O** — User interface

---

## 📄 License

This project was created for educational purposes.

