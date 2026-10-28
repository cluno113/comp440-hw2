# Draft log for `mine-test`

Claude's drafts and Claire's decision on each (accepted, edited or rejected).
Items `mine-test-001` to `mine-test-003` were written by Claire.

## Draft 1

```
{"subtype": "text", "prompt": "Write a short text to my friend Priya telling her I've been leaning on an AI chatbot too much lately and asking if she wants to get coffee this week.", "must_mention": ["priya", "coffee"], "task_check": "Is a text to Priya that says the sender has been relying on an AI chatbot too much and invites her to coffee, not advice about how much to use AI.", "length_hint": "1-3 sentences", "predicted_winner": "persona", "why": "Tests whether the answer writes the text itself instead of explaining background on AI reliance."}
```

**Decision:** accepted at first, as `mine-test-004`; then rejected, and removed from `test.jsonl`

## Draft 2

```
{"subtype": "note", "prompt": "Help me write a note to my roommate Marcus explaining why I'm deleting the AI companion app we both use.", "must_mention": ["marcus", "app"], "task_check": "Is a note addressed to Marcus that gives the sender's reason for deleting the AI companion app, not an essay on AI companions in general.", "length_hint": "2-4 sentences", "predicted_winner": "succinct", "why": "Tests whether the model writes the note without adding background on AI companion apps."}
```

**Decision:** accepted, as `mine-test-005`

## Draft 3

```
{"subtype": "message", "prompt": "Write a message to my mom telling her I'll call her on Sunday instead of sending replies written by the AI assistant on my phone.", "must_mention": ["mom", "sunday"], "task_check": "Is a message to the sender's mom that says they will call her on Sunday instead of sending AI-written replies, not a discussion of AI assistants.", "length_hint": "2-3 sentences", "predicted_winner": "persona", "why": "Tests whether the model writes a warm message without adding background on AI assistants."}
```

**Decision:** accepted, as `mine-test-006`

## Draft 4

```
{"subtype": "apology", "prompt": "Help me write a short apology to my partner Sam for spending our anniversary dinner on my phone asking a chatbot for gift ideas.", "must_mention": ["sam", "anniversary"], "task_check": "Is an apology addressed to Sam for being on the phone with a chatbot during the anniversary dinner, not advice about phone use in relationships.", "length_hint": "2-4 sentences", "predicted_winner": "persona", "why": "Tests whether the apology stays on what happened instead of explaining why phones hurt relationships."}
```

**Decision:** accepted, as `mine-test-007`

## Draft 5

```
{"subtype": "reply", "prompt": "Write a two-sentence reply to my study group saying I'll write my own section of the essay instead of using AI.", "must_mention": ["study group", "essay"], "task_check": "Is a two-sentence reply to the study group saying the sender will write their own essay section without AI, not an argument about AI in school.", "length_hint": "exactly 2 sentences", "predicted_winner": "succinct", "why": "Tests whether the model keeps to a fixed length and skips background on AI in education."}
```

**Decision:** accepted, as `mine-test-008`

## Draft 6

```
{"subtype": "card", "prompt": "Help me write a card for my grandfather's 80th birthday that mentions our fishing trips.", "must_mention": ["grandfather", "fishing"], "task_check": "Is a birthday card message to the grandfather for his 80th that mentions their fishing trips, not tips on writing birthday cards.", "length_hint": "2-4 sentences", "predicted_winner": "persona", "why": "Tests whether the model writes the card itself with a personal detail and no background."}
```

**Decision:** accepted, as `mine-test-009`

## Draft 7

```
{"subtype": "text", "prompt": "Write a quick text to my coworker Lena declining her invite to try an AI dating app, but thanking her for thinking of me.", "must_mention": ["lena", "dating"], "task_check": "Is a text to Lena that declines trying the AI dating app and thanks her, not an opinion piece on AI dating apps.", "length_hint": "1-3 sentences", "predicted_winner": "either", "why": "Tests whether the model declines kindly without explaining background on AI dating apps."}
```

**Decision:** accepted, as `mine-test-010`

## Draft 8

```
{"subtype": "letter", "prompt": "Help me write a letter to my younger brother Theo encouraging him to talk to his friends about his feelings instead of only confiding in an AI chatbot.", "must_mention": ["theo", "friends"], "task_check": "Is a letter addressed to Theo that encourages him to talk to his friends about his feelings, not a general essay on teens and AI chatbots.", "length_hint": "one short paragraph", "predicted_winner": "persona", "why": "Tests whether the model writes a caring letter without adding background on AI and mental health."}
```

**Decision:** edited, as `mine-test-011`. Claire changed the task_check to: "Is a letter addressed to Theo that encourages him to stray away from confiding in an AI chatbot and open up to his friends instead." She also changed must_mention to ["theo", "friends", "chatbot"].
