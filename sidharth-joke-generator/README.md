# n8n Joke Generator

## Workflow

The following nodes were used:
- Manual trigger (When clicking Execute Workflow)
- HTTP Request (with GET as https://official-joke-api.appspot.com/random_joke)
- Send an Email

## API used

`https://official-joke-api.appspot.com/random_joke`

## Output produced

Output of HTTP Request node:

``` json
[
  {
    "type": "general",
    "setup": "Why do bees hum?",
    "punchline": "Because they don't know the words.",
    "id": 343
  }
]
```

Output of Email node:

``` json
[
  {
    "accepted": [
      "sidharthsgdrive@gmail.com"
    ],
    "rejected": [],
    "ehlo": [
      "SIZE 35882577",
      "8BITMIME",
      "AUTH LOGIN PLAIN XOAUTH2 PLAIN-CLIENTTOKEN OAUTHBEARER XOAUTH",
      "ENHANCEDSTATUSCODES",
      "PIPELINING",
      "CHUNKING",
      "SMTPUTF8"
    ],
    "envelopeTime": 1126,
    "messageTime": 922,
    "messageSize": 416,
    "response": "250 2.0.0 OK  1782145545 d9443c01a7336-2c7436ff46asm86331815ad.35 - gsmtp",
    "envelope": {
      "from": "sidharthvjain@gmail.com",
      "to": [
        "sidharthsgdrive@gmail.com"
      ]
    },
    "messageId": "<d41da2d7-a828-341b-6214-74aa0e8fc23f@gmail.com>"
  }
]
```
