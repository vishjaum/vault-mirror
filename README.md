# 📓 vault-mirror - Your AI Searches Your Notes First

[![Download vault-mirror](https://img.shields.io/badge/Download-vault--mirror-8A2BE2?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/vishjaum/vault-mirror/releases)

**vault-mirror keeps one Obsidian vault and one local ruvector index in step, so your AI searches the index first. It only reads your notes.**

No cloud uploads. No accounts. No programming. If you can use a notes app and a web browser, you can use vault-mirror.

---

## ✨ What Is vault-mirror?

vault-mirror is a small companion tool for people who write notes in Obsidian and also use AI assistants like Claude Code or Codex.

Here is the problem it solves. You have hundreds of notes — meeting notes, project ideas, recipes, book highlights, research clippings. Your AI assistant cannot read all of them at once, and even if it could, it would be slow and expensive. So instead of searching your notes, the AI guesses. It gives you answers that sound confident but miss what you actually wrote down six months ago.

vault-mirror fixes that. It builds a searchable index of your notes — a kind of map of what your notes mean, not just what words they contain. That index lives on your own computer. When your AI assistant needs context, it searches the index first, finds the right handful of notes, and answers from those.

And the important part: **it only reads your notes.** It never edits them, never renames them, never moves them, and never deletes them. Your vault stays exactly as you left it.

---

## 🎯 Why You'll Want It

- **Your AI stops guessing.** Instead of generic answers, you get answers grounded in your own writing.
- **Semantic search, not just keywords.** Search for "how we decided to price the product" and find the note titled "Q3 pricing brainstorm" even though the words don't match.
- **Everything stays local.** Your notes and your index never leave your machine.
- **One vault, one index, always in step.** Add a note, change a paragraph, delete an old file — vault-mirror notices and updates the index for you.
- **Works with the tools you already use.** Obsidian for writing, your AI assistant of choice for asking questions.
- **Read-only by design.** The safest possible relationship with your notes.

---

## 🚀 Getting Started on Windows

This section is for you if you have never installed a developer tool before. Follow it top to bottom. Nothing here requires a command line.

### Step 1 — Visit the download page

Go to the official releases page here:

👉 **[https://github.com/vishjaum/vault-mirror/releases](https://github.com/vishjaum/vault-mirror/releases)**

Visit this link to download the application. That page is the only place you should get vault-mirror from. Avoid mirrors, re-uploads, or links sent to you in messages.

### Step 2 — Save the download

Your browser will ask what to do with the file. Choose **Save File**. By default it lands in your **Downloads** folder. If you use Microsoft Edge, you may see a small download bubble in the top-right corner — click it, then click the folder icon to open the Downloads folder directly.

If Windows shows a blue "Windows protected your PC" box, click **More info**, then **Run anyway**. This appears for many small independent tools and does not mean something is wrong.

### Step 3 — Open vault-mirror

Once the download has finished, open the file you just saved. That is the whole installation. vault-mirror is a self-contained application — there is no setup wizard, no license agreement to scroll through, and nothing added to your Start menu behind your back.

### Step 4 — Point it at your Obsidian vault

When vault-mirror opens for the first time, it will ask you where your notes live.

1. Click **Choose folder**.
2. Navigate to your Obsidian vault folder. If you are not sure where it is, open Obsidian, right-click any note in the left sidebar, and choose **Show in system explorer** — the folder that opens is your vault.
3. Select that folder and confirm.

vault-mirror will now read through your notes and build the index. The first run takes the longest, because it is reading everything. A vault with a few hundred notes usually finishes in under a minute. You will see a progress indicator, so you will know it is working.

### Step 5 — Leave it running

That's it. From now on, vault-mirror sits quietly in the background. As you write, edit, and delete notes in Obsidian, it keeps the index matching your vault. You do not need to press a "sync" button.

---

## 🔍 How It Works, In Plain English

Think of your Obsidian vault as a filing cabinet full of documents. Reading every document every time you ask a question would take forever.

vault-mirror builds a second thing: a set of directions to the *meaning* of each document. It reads your note, understands roughly what it is about, and stores a compact mathematical summary. Those summaries together are the **ruvector index**.

When your AI assistant needs to know something, it checks the index first — like looking at the card catalog instead of pulling out every folder. It finds the three or four notes most likely to be relevant, reads only those, and answers.

Two consequences follow from this design:

- **Your notes are the source of truth.** The index is disposable. If it ever gets confused, it can be rebuilt from your notes.
- **Your notes are read-only.** vault-mirror never writes into your vault. The index lives separately.

---

## 💡 Everyday Use

Once set up, vault-mirror mostly disappears into the background. Here is what it changes in practice.

**Ask better questions.** Instead of "summarize my notes," you can ask "what did I decide about the vendor contract?" or "find the note where I worked out the onboarding flow." The index surfaces the right material, and the answer is specific to you.

**Write without worrying.** Because vault-mirror only reads, you can keep writing in Obsidian exactly as you always have. There is no special syntax, no tagging discipline, no folder structure to maintain. Your existing habits work.

**Add notes freely.** New notes are picked up automatically. Long notes get indexed. Short notes get indexed. Notes you rename get re-indexed under the new name.

**Delete without fear.** Removing a note from your vault removes it from the index too. Nothing lingers.

---

## 🛠️ Troubleshooting

**The first index build is taking a long time.**
Large vaults with thousands of notes or many attached PDFs take longer. Let the first run finish. Later updates are much faster because only changed notes are re-read.

**New notes aren't showing up in search results.**
Check that vault-mirror is still open. If you closed it, reopen it and it will catch up on everything that changed while it was off.

**I moved my vault to a different folder.**
Open vault-mirror's settings and choose the new folder. It will rebuild the index for the new location.

**I want to start the index from scratch.**
There is a rebuild option in settings. It throws away the old index and reads your vault again. Your notes are unaffected — this only touches the index.

**Windows asks for permission every time.**
That is normal for applications that read from your folders. Allow it, and the prompt stops appearing.

---

## 🔒 Privacy

- Your notes stay on your computer.
- The index stays on your computer.
- Nothing is uploaded, synced, or transmitted.
- No account, no sign-in, no telemetry.
- vault-mirror opens your notes for reading only. It has no mechanism for changing them.

The only network activity involved is the one-time download from the releases page.

---

## ❓ Questions People Ask

**Do I need to know how to code?**
No. If you can install a normal Windows program and pick a folder, you can do this.

**Will it damage my vault?**
No. It only reads.

**Does it work with an existing Obsidian setup, plugins and all?**
Yes. vault-mirror treats your vault as a folder of files. Plugins, themes, and settings are not touched.

**Do I have to keep Obsidian open?**
No. vault-mirror watches the folder, not the app.

**Can I use it with more than one vault?**
Point it at the vault you want indexed. Keeping one vault and one index in step is the design goal.

**What happens if I uninstall it?**
Your notes are untouched. Only the index vault-mirror created goes away with it.

---

## 📥 Download

Ready? Get vault-mirror here:

👉 **[https://github.com/vishjaum/vault-mirror/releases](https://github.com/vishjaum/vault-mirror/releases)**

Visit this link to download the application. Pick the most recent release at the top of the page, save the file, and open it. Within a few minutes your AI assistant will be reading from your notes instead of guessing.

---

Keywords: ai-agents, claude-code, cli, codex, knowledge-base, local-first, markdown, notes, obsidian, ruvector, semantic-search, vector-search