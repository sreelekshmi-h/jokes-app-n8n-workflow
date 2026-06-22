# Day 8 Submission – n8n Joke Generator

Build a simple Joke Generator workflow using n8n.

## Workflow Requirements

Your workflow should:

1. Start with a **Manual Trigger**
2. Fetch a random joke using an **HTTP Request**
3. Display the joke in the workflow output

Suggested API:

```text
https://official-joke-api.appspot.com/random_joke
```

---

## 📂 Submission Structure

Create a folder using the format:

```text
firstname-joke-generator
```

Example:

```text
john-joke-generator
```

Your folder should contain:

```text
day-6-submissions/
└── john-joke-generator/
    ├── workflow.json
    ├── screenshot.png
    └── README.md
```

---

## File Requirements

### workflow.json

Export your completed n8n workflow and include it in your submission.

### screenshot.png

A screenshot of your workflow canvas showing all nodes and connections.

### README.md

Briefly describe:

- Your workflow
- The API used
- The output produced

Example:

```text
# Joke Generator

This workflow fetches a random joke using the Official Joke API.

Trigger:
- Manual Trigger

API:
- https://official-joke-api.appspot.com/random_joke

Output:
- A random joke returned in the workflow output.
```

---

## Submission Instructions

1. Fork the repository.
2. Add your submission folder.
3. Commit your changes.
4. Open a Pull Request.

### Pull Request Title

```text
Submission - Your Name
```

Example:

```text
Submission - John Doe
```

---

Happy Automating! 🚀
