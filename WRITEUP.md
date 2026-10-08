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

XXXX

## Part 1: The tools and the tests

### Step 1: About the model

XXXX

### Step 2: What the model predicts next

XXXX

### Step 3: Your four grades

XXXX

### Step 4: The held-back items

XXXX

### Step 5: Your run folder

XXXX

### Step 6: One question traced, and your diagram

XXXX (add the diagram image to the repository and link it here)

### Step 7: Your 10 grades and Claude's

XXXX

### Step 8: Three surprising answers

XXXX

## Part 2

[TBD]
