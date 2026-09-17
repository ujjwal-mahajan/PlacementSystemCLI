# PlacementSystemCLI
# Placement Criteria & Management System

A robust, Object-Oriented Java CLI application designed to automate university placement drives. It allows administrators to register students, define company eligibility criteria, automatically filter candidate pools using the Strategy Pattern, and manage recruitment statistics.

---

## Key Features

* **Student Registry**: Manage student profiles including CGPA, active backlogs, department, and skill sets.
* **Dynamic Placement Criteria**: Companies can define minimum CGPA, maximum allowed backlogs, eligible departments, and specific skill requirements using the **Builder Pattern**.
* **Automated Eligibility Evaluation**: Evaluates candidates dynamically via the **Strategy Pattern** while ensuring already-placed students are excluded from subsequent drives.
* **Placement Tracking**: Mark selected candidates as placed and view real-time recruitment statistics.
* **Interactive CLI Interface**: User-friendly terminal interface with input validation and custom exception handling.

---

## Design Patterns & Core Concepts Used

* **Builder Pattern**: Used in `PlacementCriteria` to handle flexible, multi-parameter criteria creation.
* **Strategy Pattern**: Used in `EligibilityStrategy` to isolate evaluation logic and allow future expansion of criteria rules.
* **Custom Exception Handling**: Uses `PlacementException` to capture runtime domain errors (e.g., duplicate IDs, unregistered companies).
* **Java Streams & Collections**: Stream API for filtering eligible candidates and computing metrics.

---

## Getting Started

### Prerequisites

* **Java Development Kit (JDK)**: Version 17 or higher installed.

### Installation & Run Instructions

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/ujjwal-mahajan/PlacementSystemCLI.git](https://github.com/ujjwal-mahajan/PlacementSystemCLI.git)
   cd PlacementSystemCLI
   javac PlacementSystemCLI.java
   java PlacementSystemCLI

   ├── PlacementSystemCLI.java        # Core Application Entry & CLI Menu Interface
└── README.md                      # Project Documentation

└── README.md # Project Documentation
