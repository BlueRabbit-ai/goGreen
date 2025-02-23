# Git Commit Generator

This is a Node.js script that generates random Git commits within a specified date range. It is useful for creating a simulated Git history for testing, experimentation, or learning purposes.

## 🚀 Features

- **Custom Date Range**: Specify any start and end date for the commits.
- **Randomized Commits**: Generates a specified number of commits with random dates within the range.
- **Sequential Processing**: Ensures no Git conflicts by processing commits one at a time.
- **Interactive Prompts**: Easy-to-use command-line interface for inputting dates and commit count.
- **Progress Tracking**: Displays real-time progress during commit creation.

## 📌 Prerequisites

Before running the script, ensure you have the following installed:

- **[Node.js](https://nodejs.org/)** (v16 or higher recommended)
- **Git** (configured with your repository)

## 📥 Installation

Clone this repository or download the script:

```bash
git clone https://github.com/BlueRabbit-ai/goGreen.git
cd goGreen
```

Install the required dependencies:

```bash
npm install
```

## ▶️ Usage

Run the script:

```bash
node index.js
```

Follow the prompts:

1. Enter the start date in **YYYY-MM-DD** format (e.g., `2024-12-01`).
2. Enter the end date in **YYYY-MM-DD** format (e.g., `2025-02-23`).
3. Enter the number of commits to generate (e.g., `100`).
4. Wait for the script to complete. It will:
   - Generate random commits within the specified date range.
   - Push the commits to your Git repository.

### Example Output:

```bash
Enter start date (YYYY-MM-DD): 2024-12-01
Enter end date (YYYY-MM-DD): 2025-02-23
Number of commits to generate: 100

Generating commits...
Commits created: 100/100

Done! Created 100 commits in 12.345 seconds
```

## ⚙️ Configuration

- **Repository**: Ensure you are in a Git repository before running the script.
- **Date Range**: The script validates the date range and ensures the end date is after the start date.
- **Commit Count**: You can generate any number of commits, but keep in mind that larger numbers will take longer to process.

## 📦 Dependencies

This script uses the following Node.js libraries:

- [`jsonfile`](https://www.npmjs.com/package/jsonfile) - For writing JSON data to a file.
- [`moment`](https://www.npmjs.com/package/moment) - For date manipulation and formatting.
- [`simple-git`](https://www.npmjs.com/package/simple-git) - For interacting with Git programmatically.
- [`random`](https://www.npmjs.com/package/random) - For generating random numbers.

## 🔍 Notes

- **Ethical Use**: This script is intended for educational and testing purposes. Do not use it to misrepresent activity on public repositories.
- **Performance**: The script processes commits sequentially to avoid Git conflicts, so it may take some time for large numbers of commits.
- **GitHub Contributions**: Generated commits will appear on your GitHub contribution graph if pushed to a remote repository.

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
