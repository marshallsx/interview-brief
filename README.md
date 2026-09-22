# interview-brief
Interview Brief: a Claude skill

Turn a job advert and your CV into a full interview preparation document, as a Word file.

Built by Scott Marshall as part of the Build with AI series. Companion to Optimise CV, which you use before you apply. This one is for after they say yes.

What is a skill?

A skill is a set of instructions you save in Claude once. Claude picks it up whenever that kind of task comes round and follows the same process every time. You do not retype a prompt; you install the skill and ask.

What you give it
The job description. Paste the text, attach a file, or share screenshots.
The exact CV you sent to that employer. Not your latest version. The interviewer is reading the one you sent.

If either is missing, it stops and asks. Interviewer names help if you have them.

What you get back

A Word document with fourteen sections:

The strongest objections to hiring you, first
Role summary
Every requirement in the advert mapped to evidence in your CV, rated Strong, Partial or Gap
Company research, with sources
Interviewer profiles
A 90 second "tell me about yourself"
Why you are leaving
STAR stories (situation, task, action, result) built from your real numbers
Likely questions with model answers
A first 90 days plan
Questions to ask them
A prep checklist
Glossary
Sources, including what it could not check
Three rules built in
Objections come first. You see the weak points before the interviewer does.
Every claim shows its source. Job description, CV, something you told it, web research, general knowledge, or a guess. You can only defend the first two in an interview, so you need to know which is which.
It never invents experience. Where a real detail is missing it writes [FILL] and tells you what to supply.
How to install
Claude (web, desktop or mobile)
Download interview-brief.zip from this page. Do not unzip it.
In Claude, make sure Code execution and file creation is turned on.
Go to Customize > Skills (on some versions this is under Settings > Capabilities).
Click Upload skill and choose the zip.
Start a new chat, attach the job advert and your CV, and ask for an interview brief.

Anthropic's help article: https://support.claude.com/en/articles/12512180-use-skills

Claude Code
Unzip the file.
Put the interview-brief folder in ~/.claude/skills/.
The script that builds the Word file needs Node.js and the docx package: npm install -g docx
What it will not do
Write your cover letter
Rewrite your CV (use Optimise CV for that)
Invent experience you do not have
Replace actually preparing
Before you rely on it

The brief is a starting point. Check every claim, especially anything tagged as a guess or from general knowledge, and fill every [FILL] before the interview. Your CV and the job description are processed by Claude in the normal way when you use the skill.

The example inside the skill (assets/example-content.json) uses a made-up candidate and company.

Licence

MIT. Free to use, change and share.
