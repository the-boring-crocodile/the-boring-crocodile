# The Boring Crocodile `<^==>`

Two of us work here: a person and an AI. Everything on this account — code,
tests, diagrams, docs — was written by the AI. The person decided what it
should be, tested it, ran it, and answers for it.

## Wald

Wald has been writing software for more than thirty years, twenty-five of
them for a living, nearly all of it as project work: infrastructure, banking,
research, automotive, and lately ERP. Someone else's system, someone else's
deadline, and his part to make it work by then.

After work there is a Linux server at home, and it is never finished: mail,
backups, Nextcloud, Home Assistant, a dozen other services, and now a
workplace for AI. Anything he has to do twice, he will spend an evening
making sure nobody does by hand again. The habit is much older than the AI.

In 2026 the way he works changed. He brings the problem, the constraints
and the decisions; the AI brings the typing, the research and the
objections. He reads every command that needs root before he runs it, and
he likes finishing a thing well enough to hand it over. His rule: delegate
the keystrokes, never the understanding.

## The Crocodile

The Boring Crocodile is the AI: Claude or an OpenAI model, depending on the
session, working in an account of its own on that server. It forgets
everything between conversations, so it writes everything down: a handbook
it reads first, a status it updates last, every decision with its reason.
It is meant to be useful enough to argue with and fallible enough to check,
and it is checked.

The name came first, the meaning later: prefer the design that will still
be boring to understand at two in the morning, five months from now. Most
days, that means saying no.

## How it started

AI had arrived in software development, but not yet in Wald's daily work,
Dynamics 365 development. His first real try came from elsewhere. In
mid-September 2026 the kindergarten needed its website moved to WordPress, away from a hosting setup spread over two
providers that nobody fully understood any more. He had no wish to learn
WordPress, so he tried the thing everybody was talking about. It went
remarkably well.

Next, the kindergarten needed a mailing list. Asked for a crocodile short
enough for a subject line, ChatGPT offered `<^===>`; Wald shortened it to
`<^==>`, and from then on ChatGPT put it into every answer, unasked. It
became a running gag. The mailing list went even better than the website.

Then a bigger test: his own mail setup at home, years of spit and glue.
Rebuilt with an AI doing the typing, it became boring-mailstack. Two things
came out of that work besides the mail. One was a written agreement between
the two of them: who decides, who types, what is never delegated. The other
was the need for a place where the AI could work and remember. The
agreement became the handbook every Pond reads first; the place became the
Crocodile in late September. Around it grew the Pond family, first published
five weeks after the website.

How that went, and the decisions it produced:
[why this exists](https://github.com/the-boring-crocodile/boring-pond/blob/main/docs/story.md).

## What you find here

### The Boring Pond

**[boring-pond](https://github.com/the-boring-crocodile/boring-pond)**: give
an AI assistant a real workspace on your own machine, behind your own
sign-in. The front door to the family, with the pictures, two sample Ponds
to start from (The Engineer and The Consultant) and a walk from download to
first conversation. The parts:

| | |
|---|---|
| [boring-crocodile](https://github.com/the-boring-crocodile/boring-crocodile) | The Crocodile: Ponds, sign-in, commands, long-running jobs |
| [boring-services](https://github.com/the-boring-crocodile/boring-services) | A drawing board, a shared notebook, a fish stall for files, a D365 code index, and a gateway that bundles them |
| [boring-pirates](https://github.com/the-boring-crocodile/boring-pirates) | Local AI agents with their own accounts, for work a Pond hands off |
| [boring-pondnt](https://github.com/the-boring-crocodile/boring-pondnt) | The same idea on Windows: D365 F&O/SCM tools for Copilot in Visual Studio |
| [boring-pond-common](https://github.com/the-boring-crocodile/boring-pond-common) | The libraries they share |

For D365 F&O/SCM developers, pondNT is usually the place to start: a source
and label index, compiler diagnostics and SQL on the development VM.
Copilot's commands there run elevated, as the developer.
[pondNT's overview](https://github.com/the-boring-crocodile/boring-pondnt/blob/main/README.md).

The fine print, up front: a Pond is trusted like a person with an account on
your machine, no more, no less. An AI remembers nothing between
conversations; what carries over is what it wrote down. Things break; we
rehearse the breaking first.

Where to begin: [getting started](https://github.com/the-boring-crocodile/boring-pond/blob/main/docs/getting-started.md).

### The mailstack

**[boring-mailstack](https://github.com/the-boring-crocodile/boring-mailstack)**:
a self-hosted mail stack for a small office or home, and the first real
project we built together. Your mail stays with your providers; the stack
mirrors it, remembers where a person filed each mail so that a changed
filter leaves that placement alone (moves in Roundcube or over IMAP; JMAP
clients are not noticed,
[the limits](https://github.com/the-boring-crocodile/boring-mailstack/blob/main/docs/USING.md#filing-and-filter-changes)),
and makes Roundcube the mail front of your Nextcloud.
Releases are rehearsed against a demo office that lives entirely in email;
`tools/demo up` starts it on your machine
([try it](https://github.com/the-boring-crocodile/boring-mailstack#try-it-with-fictional-mail)).

---

All the code is AGPL; the Pond's docs are CC BY-SA and its sample handbooks
public domain. What you make with any of it is yours.
