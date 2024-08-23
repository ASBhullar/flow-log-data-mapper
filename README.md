# Flow Log Tagger

This project provides a solution for parsing flow log data, tagging each entry based on a predefined lookup table, and generating detailed reports on the tagged data. The goal is to automatically categorize flow log entries by matching the destination port and protocol with entries in a lookup table.

## Table of Contents

1. [Setup Instructions](#setup-instructions)
    - [Prerequisites](#prerequisites)
    - [Step-by-Step Setup](#step-by-step-setup)
6. [Running the Program](#running-the-program)

## Setup Instructions

### Prerequisites

Ensure you have the following installed on your system:

1. **Java Development Kit (JDK)**: Version 8 or later.
2. **Text Editor or IDE**: Optional, but recommended for editing and reviewing code.

### Step-by-Step Setup

1. **Clone the Repository**

   Download the project from GitHub using the following command:

   git clone https://github.com/asbhullar/flow-log-data-mapper.git

2. **Prepare Your Input Files**

   - **Flow Log File**: A text file containing your network traffic logs (e.g., `flowlogs.txt`).
   - **Lookup Table File**: A CSV file defining the tags (e.g., `lookup_table.csv`).

3. **Compile the Program**

   Navigate to the project directory and compile the Java source files:

   javac -d bin src/*.java

## Running the Program

Once compiled, you can run the program with the following command:

java -cp bin Main flowlogs.txt lookup_table.csv output_directory

Replace `flowlogs.txt`, `lookup_table.csv`, and `output_directory` with your actual file paths. The program will generate two CSV reports in the specified output directory.




