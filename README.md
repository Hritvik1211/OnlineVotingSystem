# Online Voting System

## Project Overview

This project provides a secure and automated solution for electronic voting using web technologies and blockchain principles. It is designed to allow eligible voters to participate in elections online with transparency, auditability, and privacy. The system leverages Python and Flask for backend services and incorporates a basic blockchain implementation to enhance vote integrity and security.

## Directory Structure and Key Files

- **main.py**: The core web application, built using Flask, handles voting workflows, user authentication, dashboard presentation, and administrative controls. Key modules include voter registration, casting votes, and result tabulation. It interacts with other modules to ensure voting eligibility, securely records votes, and provides real-time status updates. The app also supports a basic token-based authentication system.

- **test.py**: Implements a simplified blockchain for holding voting records. It validates voters' eligibility (minimum age), encrypts voter and vote data using SHA-512, and adds each vote as a secured block linked to the prior vote. The blockchain ensures data integrity and provides a simple prototype for tamper-resistant vote storage.

- **utils.py**: Contains utility functions to support operations in the system, such as data processing, formatting, or other helper routines (details assumed typical for such a file).

- **requirements.txt**: Lists the Python library dependencies needed to run the project (including Flask, presumably).

- **blockchainfolder/**: Placeholder for additional blockchain source code or modules. It suggests future extension for the blockchain voting functionality.

- **dbfolder/**: Intended for database code or scripts, handling persistent data management for the app.

- **templates/**: Houses HTML template files used to generate the web interface for various pages (e.g., home, voting, results, configuration).

- **static/**: Contains static resources such as CSS stylesheets, images, and JavaScript files used by the web frontend.

- **Online-Voting-System_ppt[1].pptx**: A project presentation (PPT file) outlining goals, architecture, and implementation details.

- **.gitignore**: Lists files and folders ignored by Git for cleaner version control.

## Main Features

- **Voter Validation**: Ensures only eligible users (age ≥ 18) participate.
- **Secure Voting**: Each vote is stored as a block in a blockchain sequence, encrypting vote details.
- **Candidate Selection**: Offers a set of choices representing major parties and NOTA.
- **Voting Summary**: Outputs the full blockchain for audit and review after voting closes.
- **Web Interface**: Linear and interactive voting flows via Flask web app.
- **Admin Controls**: Admin access for managing and supervising election activity (as designed in main.py).
- **Extensibility**: Folders for future blockchain and database features.

## Quickstart

1. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the Application**
   ```bash
   python main.py
   ```

3. **Access the Web UI**
   Visit `http://localhost:5000` by default.

## Blockchain Voting Flow Example

- Prompts voter for age; only eligible voters proceed.
- Voter inputs name and chooses a party.
- Each vote is encrypted and linked in a blockchain for transparency.
- At session end, prints a readable chain of all voter entries.

## Credits

Developed by [Hritvik1211](https://github.com/Hritvik1211).  
For further details, see the included project presentation.

---

*This project provides an educational foundation for secure digital voting. For production use, further security, cryptographic rigor, and audit measures are recommended.*
