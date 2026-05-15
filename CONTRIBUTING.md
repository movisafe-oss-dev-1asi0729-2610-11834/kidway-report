# **Contributing Guidelines - KidWay Report (MoviSafe Startup)**

This document defines the *collaboration rules, workflow, and responsibilities* for all team members working on the KidWay Report repository.

---

## **Team Organization**

The team is composed of **5 members**. Each member is assigned a primary chapter:

- Member 1 → *Chapter 1: Introduction*
- Member 1 → *Chapter 2: Requirements Elicitation & Analysis*
- Member 2 → *Chapter 3: Requirements Specification*
- Member 3, 4 → *Chapter 4: Product Design*
- Member 5 → *Chapter 5: Implementation*

### **Responsibilities**

- Each member is responsible for their chapter
- Members can support others
- Communicate before editing shared sections

---

## **Branching Model (GitFlow)**

We use a simplified GitFlow strategy:

- `main` → Final delivered versions ***(DO NOT WORK HERE)***
- `develop` → Integration branch
- `feature/*` → Work branches
- `release/*` → Delivery preparation

### **Branch Examples**

- `feature/chapter-1-introduction`
- `feature/chapter-2-interviews`
- `feature/chapter-3-user-stories`
- `feature/chapter-4-design`
- `feature/chapter-5-implementation`

---

## **Workflow (Mandatory)**
### **1. Update repository**

```bash
git checkout develop
git pull origin develop
```

### **2. Create branch**

```bash
git checkout -b feature/your-task-name
git push -u origin feature/your-task-name
```

### **3. Work on your section**

- Only edit your assigned files
- Follow `/docs` structure
- Avoid conflicts with teammates

### **4. Commit changes**

```bash
git commit -m "feat(chapter-2): add interview analysis"
```

### **5. Push changes**

```bash
git push origin feature/your-task-name
```

### **6. Pull Request**

- From `feature/*` → `develop`
- At least *1 review required*
- Resolve conflicts before merge

---

## **Release Process**
### **Create release branch**

```bash
git checkout -b release/tb1
```

### **Final steps**

- Fix formatting
- Validate links/images
- Ensure completeness

### **Merge**

- `release/*` → `main`
- `release/*` → `develop`

---

## **Commit Convention**

We follow *Conventional Commits*:

- `feat:` → New content
- `docs:` → Documentation
- `fix:` → Corrections
- `chore:` → Maintenance
- `refactor:` → Improvements

### **Examples**

- `feat(chapter-1): add startup profile`
- `docs: update table of contents`
- `fix(chapter-2): correct interview data`
- `chore: reorganize assets`

---

## **File Organization**

- All content → `/docs`
- Assets → `/assets`
- Use `.md` format

### **Rules**

- Keep structure consistent
- Use clear filenames
- Avoid duplication

---

## **Important Rules**

- Always `git pull` before working
- Never commit to `main` or `develop`
- Use Pull Requests
- Avoid editing same file simultaneously
- Keep commits small and clear

---

## **Collaboration**

- Support teammates when needed
- Communicate changes
- Maintain consistency across chapters

---

## **Conflict Resolution**

If conflicts appear:

- Pull latest changes
- Resolve manually
- Test document structure
- Commit again

---

## **Evaluation Evidence**

The following will be evaluated:

- Commits
- Branches
- Pull Requests
- Reviews
- Team collaboration

---

## **Final Notes**

- Use English for:
  - Branch names
  - Commits
  - File names

- Maintain a *professional and consistent style*

---

**Goal:** Deliver a structured, collaborative, and high-quality academic report following professional development practices.
