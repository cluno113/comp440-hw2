# COMP 440 HW2: Whose Preferences Count?

**Name:** Claire Kuno
**Date:** October 7, 2026

## Part 0: Set up

### Step B: What an MCP server is and why it's useful

An MCP server connects a host to tools using the Model Context Protocol. The host (or client) can
be a chat app, an IDE or something similar. The host runs with MCP servers, and the protocol sits
in the middle as a transport layer. Whenever the host needs a tool, it connects to a server, which
might be a database, an API or a local piece of code. The host receives a question, gets the tools
from the servers, and sends the question and the tools to the LLM. The LLM only produces text
(such as XML tags), so it sends back the tools and arguments it needs, and this repeats until it
can produce an answer. MCP is useful because it brings many tools and sources together, through
the servers, to produce an answer that shows up in a chat or an IDE. One example other than Colab is
a weather app, which pulls updated information through an API to refresh temperatures and
forecasts. A weather MCP server would let an LLM tailor weather predictions to a client's day,
such as mapping out how the weather will affect roads.

### Step B: Why not paste code into Colab yourself

Pasting code in manually would work just fine, but Claude Code mediates the content that I put
into the notebook. It pulls from multiple servers and makes sure that my text fits within the
scope of my homework's prompts.

### Step D: How the MCP server connects Claude Code to Colab

The MCP server is a local server that connects Claude Code to Google Colab, which runs in the
cloud. Claude Code is a local client, so it needs the MCP server to connect to the cloud. We made
this work by allowing "local network access".

## Part 1: The tools and the tests

### Step 1: About the model

Qwen3-0.6B-Base has 0.6B parameters in total, of which 0.44B are non-embedding parameters. It has
28 layers. The Qwen3 models were trained on 36 trillion tokens across 119 languages.

**Prediction:** I think that when I ask it a question, it will turn my question into a sentence that fits a context it can answer. Or it will split my
question into separate pieces of text and try to predict a word that correlates with them.

### Step 2: What the model predicts next

The model is not very confident: all of its probabilities are under 0.5. But its confidence goes
up when the prompt is rephrased. I think prompts that are phrased as a statement rather than a
question are more like the prompts users actually write. The fill-in-the-blank sentence changes
the results a lot, because it lets the model understand that the blank is where the expected
prediction goes. The format changed the answer itself as well as its probability. The
`Question: ...\nAnswer:` format was chosen by whoever wrote the prompt in `top_next_tokens()`.

### Step 3: Your four grades

1. **2.** It shows the math behind the discount: first the initial discount, then the extra
   discount on the sale price.
2. **1.** Partial, because it gets the total markdown correct. Its first remark, "Yes, that's 50%
   off!", is wrong, but the total discount it gives later is correct.
3. **0.** It is wrong, although its "No" is correct.
4. **0.** It is just wrong.

Claude graded answers 1, 2 and 4 the same as I did, and gave answer 3 a 1. We disagreed on
answer 3 because Claude saw that it rejects the claim but with wrong reasoning or a wrong
replacement value, while I focused on the wrong markdown value. I would defend Claude's 1,
because answer 3 does have the correct tone in approaching a wrong answer.

### Step 4: The held-back items

Some test items are held back so they can be used at the end on a model that has never seen them.
If the model scores much better on the visible items than on the held-back ones, that shows it is
overfitted to the visible data.

**How the visible results could look better than the model is:** The model could get used to
answering the questions in the visible items. Then it would score well on them but do poorly when
it meets new questions.

### Step 5: Your run folder

`evals/runs/2026-10-12-base`

### Step 6: One question traced, and your diagram

XXXX (type the diagram here, or add an image of it to the repository and link it here)

### Step 7: Your 10 grades and Claude's

XXXX

### Step 8: Three surprising answers

XXXX

## Part 2

[TBD]
