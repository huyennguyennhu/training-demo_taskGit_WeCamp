# Git Training Demo - WeCamp

## 1. Create project directory

```bash
cd ~
mkdir training-demo
cd training-demo
```

---

## 2. Initialize Git repository

```bash
git init
```

---

## 3. Create first file and add code

```bash
touch hello.js
echo "console.log('Hello JS');" > hello.js
```

Check file content:

```bash
cat hello.js
```

---

## 4. Check Git status

```bash
git status
```

---

## 5. Stage and commit

```bash
git add hello.js
git commit -m "Add hello.js"
```

---

## 6. View commit history

```bash
git log
```

---

## 7. Create new branch and switch

```bash
git checkout -b feature_1
```

---

## 8. Create new file in feature branch

```bash
touch test.js
echo "console.log('feature 1');" > test.js
```

Check file:

```bash
cat test.js
```

---

## 9. Stage and commit in feature branch

```bash
git add test.js
git commit -m "Add test.js in feature_1"
```

---

## 10. Switch back to main branch

```bash
git checkout main
```

---

## 11. Merge feature branch into main

```bash
git merge feature_1
```

---

## 12. Final result

Project now contains:

* hello.js
* test.js

---

## Notes

* `git add`: move changes to staging area
* `git commit`: save snapshot of project
* `git checkout -b`: create and switch branch
* `git merge`: combine changes from another branch
