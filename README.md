
## **GitHub Activity CLI 🚀**  

![GitHub](https://img.shields.io/badge/GitHub-Activity%20CLI-blue?logo=github&style=flat-square)  
A simple command-line interface to fetch and display recent activity of any GitHub user. This project demonstrates API integration, JSON handling, and building a CLI tool using **Spring Boot**.

---

## **Features ✨**  
- Fetches **recent activity** of a specified GitHub user.  
- Displays events like **pushes, issues opened, starred repositories**, and more.
- Handles **API failures gracefully**.
- Simple **command-line usage**.

---

## **How It Works 🛠️**  

1. The CLI takes a **GitHub username** as an argument.
2. It makes a request to the **GitHub Events API**:
   ```
   https://api.github.com/users/<username>/events
   ```
3. It **parses** the JSON response and displays the activity on the terminal.

---

## **Installation 🧑‍💻**  

### 1. Clone the repository  
```bash
git clone https://github.com/your-username/github-activity-cli.git
cd github-activity-cli
```

### 2. Build the project  
```bash
mvn clean install
```

### 3. Run the application  
```bash
java -jar target/github-activity-cli-1.0-SNAPSHOT.jar <username>
```

---

## **Usage 💡**  

```bash
# Example usage
java -jar target/github-activity-cli-1.0-SNAPSHOT.jar kamranahmedse
```

**Sample Output:**
```
Pushed to kamranahmedse/developer-roadmap  
Opened an issue in kamranahmedse/developer-roadmap  
Starred kamranahmedse/developer-roadmap  
```

---

## **Project Structure 📂**  

```
github-activity-cli/
│
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── github/
│   │               └── activity/
│   │                   └── GitHubActivityCli.java
│   └── test/  # Add your tests here
│
├── target/   # Maven build output (ignored by .gitignore)
├── pom.xml   # Maven configuration
└── README.md # This file
```

---

## **Technologies Used 🛠️**  
- **Java**  
- **Spring Boot**  
- **Maven**  
- **GitHub API**  
- **Jackson** (for JSON parsing)

---

## **Error Handling 🛑**  
- If the **GitHub username** is invalid or the API fails:
   ```
   Error: Unable to fetch activity. Status code: 404
   ```
- If **no username** is provided:
   ```
   Usage: github-activity <username>
   ```

---

## **Contributing 🤝**  
We welcome contributions! Please follow these steps:  
1. Fork the repository.  
2. Create a new branch: `git checkout -b feature-branch`.  
3. Commit your changes: `git commit -m 'Add new feature'`.  
4. Push to the branch: `git push origin feature-branch`.  
5. Create a **pull request**.

---

## **License 📝**  
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## **Contact 📧**  
Feel free to reach out with any questions or suggestions!  
- **GitHub:** [iOmega17]([https://github.com/iOmega17])

---

## **Acknowledgments 🌟**  
- Thanks to [GitHub](https://github.com/) for the awesome API.
- Inspired by [kamranahmedse](https://github.com/kamranahmedse).

---
