# 🤝 Contributing Guide — IntelliPay Project

Welcome to the IntelliPay team!  
Please read this guide before contributing to keep our project clean, consistent, and easy to maintain.

---

# 📁 Repository Structure

```
services/
  auth-service/
  wallet-service/
  analytics-service/
  frontend/

contracts/
infra/
scripts/
docs/
```

Each teammate owns a specific service.  
Never mix files across services unless assigned.

---

# 🌿 Branching Rules

We use:

- `main` → stable, demo-ready code  
- `develop` → integration branch  
- `feature/<service>-<task>` → active work  
- `hotfix/<fix-name>` → urgent fixes  
- `release/vX.Y.Z` → milestone builds  

### How to create a feature branch:
```
git checkout develop
git pull
git checkout -b feature/<service>-<feature-name>
git push -u origin feature/<service>-<feature-name>
```

---

# 🧑‍💻 Code Contribution Steps

### 1. Create a feature branch ✨  
Follow naming rules.

### 2. Write code following folder structure  
Never place files outside your microservice.

### 3. Run locally  
Use:
```
docker compose up --build
```

### 4. Add docs if API changes  
OpenAPI files under `/contracts`.

### 5. Commit using conventional commits  
Examples:
- `feat(wallet): add transfer endpoint`
- `fix(auth): wrong JWT expiration`
- `chore(frontend): update layout`

### 6. Push your branch  
```
git push origin feature/<branch>
```

### 7. Create Pull Request  
Use PR template.

---

# ✔️ Pull Request Requirements

Your PR **must** include:

- Clear title (conventional commit format)
- Description of changes
- Screenshot/video if UI change
- Testing instructions
- Updated documentation (if necessary)
- No console logs, no unused imports  
- At least **one reviewer approval**

---

# 🔍 Code Review Guidelines

Reviewers check:

- Logic correctness  
- API consistency  
- File placement  
- Naming conventions  
- Security checks  
- Frontend usability (if UI PR)  
- No breaking of other services  

---

# 🛠 Testing Guidelines

Minimum required:

- Unit tests for critical functions  
- Manual testing on local Docker  
- Endpoint testing via Postman  

---

# 🚢 Release Flow

1. Merge all completed features into `develop`
2. Create release branch:
```
git checkout -b release/v1.0.0
```
3. Test end-to-end  
4. Merge `release` → `main`  
5. Tag version  
6. Update changelog  

---

# ❗ Rules to Avoid Conflicts

- Never commit directly to `main`  
- Always merge PR → `develop`  
- Delete feature branch after PR merge  
- Keep your branch small and focused  

---

# 🏆 Team Responsibilities

| Member | Role | Folder |
|--------|------|---------|
| B Kalyan | Lead + Infra | infra/, scripts/, docs/ |
| srikanth yadav | Auth | services/auth-service/ |
| sathish reddy | Wallet | services/wallet-service/ |
| Sravani Gudepu | Frontend | services/frontend/ |
| Donuru Madhumathi | Analytics/ML | services/analytics-service/ |

---

Thank you for contributing to IntelliPay!  
Let’s build something awesome together 🚀
