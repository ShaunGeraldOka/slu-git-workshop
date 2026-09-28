# SLU Git and GitHub Hands-on Workshop

Follow these instructions to add your file to this repository.

---

## Preliminary Operations

Check your Git configuration:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Verify that you have the Java compiler installed:

```bash
javac -version
```

---

## Procedure

### 1. Fork the Repository
Click the **Fork** button at the top-right of this GitHub page. This operation creates a copy of the repository in your GitHub account.

### 2. Clone Your Fork
Download your remote repository to your local computer:

```bash
git clone [https://github.com/YOUR_GITHUB_USERNAME/slu-git-workshop.git](https://github.com/YOUR_GITHUB_USERNAME/slu-git-workshop.git)
cd slu-git-workshop
```

### 3. Create a New Branch
Do not work in the `main` branch. Create and switch to your feature branch:

```bash
git checkout -b feature/add-your-name
```

### 4. Create Your Java File
1. Open the `src` folder.
2. Make a copy of `TemplateStudent.java`.
3. Change the name of the new file to your name with PascalCase (Example: `JuanDelaCruz.java`).
4. Open the file and update the class name to match the file name:

```java
public class JuanDelaCruz {
    public static void main(String[] args) {
        System.out.println("Hello, World! My name is Juan Dela Cruz.");
    }
}
```

### 5. Compile and Test
Compile and execute your class:

```bash
cd src
javac JuanDelaCruz.java
java JuanDelaCruz
```

### 6. Stage and Commit
Check status, stage your file, and create a commit:

```bash
git status
git add src/JuanDelaCruz.java
git commit -m "Add JuanDelaCruz.java"
```

### 7. Push to GitHub
Send your branch to your remote fork:

```bash
git push -u origin feature/add-your-name
```

### 8. Open a Pull Request
1. Open your repository on the GitHub website.
2. Click **Compare & pull request**.
3. Verify that your branch points to the workshop `main` branch.
4. Click **Create pull request**.