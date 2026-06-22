# Jokes to Email — n8n Workflow

A small n8n workflow I built that grabs a random joke from the internet and emails it to me. Pretty fun little project honestly.

## What it does

1. **Fetches a joke** from the [Official Joke API](https://official-joke-api.appspot.com/random_joke)
2. **Checks if the response is valid** — if the API is down or returns garbage, it sends me an error notification instead
3. **Filters out short jokes** (setup has to be longer than 15 characters) so the jokes are actually worth reading
4. **Formats everything nicely** with the joke type, setup, and punchline
5. **Sends it to my email** via SMTP

## How the flow works

`Manual Trigger` → `HTTP Request` → `Validation Check` → `Length Filter` → `Format Fields` → `Send Email`

If the API fails, it branches off and sends a heads-up email instead.

## Files

- `Jokes_to_Email.json` — the exported n8n workflow (import this into your n8n instance)
- `MuLearn_Project_Pic1.png` — screenshot of the workflow canvas
- `MuLearn_Project_Pic2.png` — screenshot of the email output

## Setup

1. Import `Jokes_to_Email.json` into n8n
2. Set up your SMTP credentials
3. Update the `fromEmail` and `toEmail` fields to your own address
4. Hit execute and check your inbox!

---

Built as part of the MuLearn Day 8 challenge 🚀
