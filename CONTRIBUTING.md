### **Basic Git Workflow for Team Members**

1️⃣ **Clone the repository** (if not done yet):

```
git clone https://github.com/LIKELION-CS-Team-2-SP-25/BuckyClass-mobile-ReactNative.git
cd BuckyClass-mobile-ReactNative
```

2️⃣ **Pull the latest changes before starting a new task:**

```
git checkout develop
git pull origin develop
```

3️⃣ **Create a new feature branch:**

```
git checkout -b feature/{feature-name}
```

📌 Example: `feature/chat-ui` for chat feature.

4️⃣ **Write code & commit changes:**

```
git add .
git commit -m "Added basic chat UI"
```

5️⃣ **Push your branch to GitHub:**

```
git push origin feature/chat-ui
```

6️⃣ **Go to GitHub → Open a Pull Request (PR)**

-   Select **"develop"** as the target branch.
-   Assign **reviewers** (as Mentor).
-   Add a **description of the changes**.

7️⃣ **Wait for a code review before merging.**

-   If requested, **make changes** and **push again**:
    ```
    git add .
    git commit -m "Fixed chat UI alignment"
    git push origin feature/chat-ui
    ```

8️⃣ **Once approved, merge into `develop` & delete the branch.**

```
git checkout develop
git pull origin develop
git branch -d feature/chat-ui
```

📌 **Now, the new feature is merged into `develop` and ready for testing!**
