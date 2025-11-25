# 📝 Pull Request Title
<!-- Example: feat(wallet): add ledger double-entry model -->

## 📌 Description
Provide a clear and concise explanation of what this PR does.

- What feature/bug does it address?
- Which service does it belong to? (auth / wallet / analytics / frontend / infra)
- Why is this change needed?

## 🎯 Related Issue
Fixes: #ISSUE_NUMBER  
(If no issue exists, create one first and link it here.)

---

## ✔️ Changes Made
- [ ] New folder/files added
- [ ] API endpoint updated
- [ ] Logic implemented
- [ ] UI components added
- [ ] Tests updated
- [ ] Documentation updated

---

## 🧪 How to Test Locally
Provide steps to test:

1. `git checkout <branch-name>`
2. Run `docker compose up --build`
3. Hit endpoint: `GET /v1/...` OR open frontend at localhost:3000
4. Expected output:  
   - …
   - …

---

## ⚠️ Breaking Changes?
- [ ] No breaking changes  
- [ ] Yes (explain below)

If yes, describe migration or steps needed.

---

## 👥 Reviewer Notes
Anything specific the reviewer should focus on:

- Edge cases?
- Logic correctness?
- Security considerations?
- UI UX?

---

## 🧑‍💻 Checklist Before Merge
- [ ] Code compiles with no errors
- [ ] Lint passed (if applicable)
- [ ] Unit tests added/updated
- [ ] API contract updated (OpenAPI)
- [ ] No console logs / debug prints
- [ ] PR follows branch naming rules
