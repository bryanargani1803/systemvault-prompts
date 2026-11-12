---
layout: default
title: "How to Use AI for Review Mining: Find What Buyers Want in Their Own Words"
description: "Review mining with AI: one copy-paste prompt turns customer reviews into counted themes, exact quotes and the words buyers use. Real run included."
date: 2026-11-12
---
*A plain 'summarize these reviews' prompt gives you a pleasant paragraph. A review-mining prompt gives you counts, quotes and headlines.*

Most people pick a product idea, build it for a week and only then ask what buyers think. The buyers have already told you. They wrote it in the reviews of the thing that is already selling, in their own words, for free.

*Drafted with AI assistance from this week's research, then checked and edited.*

A method @THEECOMKING shows in a YouTube video about digital products makes this a separate step before you build. The AI reads real reviews of similar products and writes down who the buyer is, what bothers them and what they wish for. Below is that step as a prompt for any chat tool, run on eight made-up reviews so you can see exactly what comes back.

### Why guessing the buyer costs you a week

When you guess, you build for the buyer in your head. That person wants everything, has no budget limit and never gets confused. Real buyers get stuck on page two and write a one-star review about it.

Reviews are the cheapest research there is. They are written by people who spent money, so they are not polite survey answers. They say what annoyed them, usually in one sentence.

The hard part is reading fifty of them and seeing the pattern. That is a job an AI does well, if you ask it the right way. (When the answer comes back vague, the [fix-it list](https://systemvault123.gumroad.com/l/ai-prompt-playbook-free?utm_source=blog&utm_medium=organic&utm_campaign=2026-11-12-medium-ai-review-mining-prompt) shows how to repair it.)

### The eight reviews we used

These are invented, for an invented product: a spreadsheet template that tracks invoices for freelancers. Nothing here is a real review of a real product. We kept them short, the way most reviews are.

```
1. Great layout but I could not figure out how to add a new client. Had to watch a video.
2. Love the colours. Wish it came with a Notion version, I don't use Excel.
3. Finally something that doesn't need a subscription. But the instructions were one page and confusing.
4. The invoice tab is fine. I spent an hour setting up the tax tab and still don't trust the totals.
5. Too many tabs for what I need. I only invoice 3 clients.
6. Works great once it's set up. Setup took me an evening though.
7. Wish it had a quick-start for people who are not good with spreadsheets.
8. Nice design, no complaints about price. The tax tab was the only part I skipped.
```

Take thirty seconds and form your own view. What would you build if you had only these? Keep that answer, because we will compare.

### The summary prompt gave a pleasant paragraph

The prompt most people send is the shortest one.

```
Summarize these reviews.
[the eight reviews]
```

Output (generated with Claude Sonnet 5.5, 2026-11-12):

```
Customers like the design and the fact that there is no subscription. Several found the setup and instructions confusing, and the tax tab caused trouble for a few. Some would like a simpler version or a Notion version.
```

Nothing in it is wrong. It is also not enough to build from.

How many is several? Which complaint is the biggest? What exactly did people say? You cannot write a headline from 'some would like a simpler version', and you cannot rank three complaints when the summary gives them equal weight.

### The review-mining prompt

The fix is to ask for the things a summary leaves out: counts, exact quotes and a rule about what counts as a pattern.

```
You are a market researcher reading customer reviews. Use only the reviews below. Do not add anything you already know about this product.

1. Group the complaints and wishes into themes. For each theme give a short name, how many of the reviews mention it, and 1 or 2 exact quotes.
2. Do the same for praise.
3. List the exact phrases buyers use that I could reuse in a headline. Copy them word for word. Do not tidy them.
4. Write one sentence: who is the buyer, and what are they afraid of?
5. If only one review mentions something, label it ONE MENTION. Do not call it a trend.

Reviews:
[paste your reviews here]
```

### What came back

We pasted the eight reviews under that prompt in a fresh chat. This is the reply, trimmed to the lines that matter.

Output (generated with Claude Sonnet 5.5, 2026-11-12), trimmed:

```
Complaints and wishes
- Setup and instructions (4 of 8 reviews: 1, 3, 6, 7)
  'I could not figure out how to add a new client'
  'the instructions were one page and confusing'
  'Setup took me an evening though'
  'a quick-start for people who are not good with spreadsheets'
- Tax tab (2 of 8 reviews: 4, 8)
  'I spent an hour setting up the tax tab and still don't trust the totals'
  'The tax tab was the only part I skipped'
- Too many tabs (ONE MENTION, review 5)
  'Too many tabs for what I need. I only invoice 3 clients.'
- Notion version (ONE MENTION, review 2)
  'Wish it came with a Notion version'

Praise
- Design (3 of 8 reviews: 1, 2, 8)
  'Great layout', 'Love the colours', 'Nice design'
- No subscription (ONE MENTION, review 3)

Buyer words for headlines
'figure out how to add a new client', 'don't trust the totals', 'not good with spreadsheets', 'Too many tabs for what I need'

Buyer: a solo freelancer with a few clients who is not confident with spreadsheets. They are afraid of losing an evening to setup and still ending up with totals they cannot trust.
```

Compare it with the summary. The summary said several people were confused. This says four of eight, names the reviews and gives you the sentences. It also refused to call the Notion wish a trend, because only one person asked.

### How to use the result

The count tells you where to aim. Four of eight reviews are about setup, so a simpler first ten minutes beats a prettier template. The design is already praised, so you do not need to change it.

The quotes tell you what to say. 'Don't trust the totals' is better copy than anything you would write at your desk, because it is how the buyer already thinks. Use the idea and keep the exact sentences from the review as your private notes, since a review is someone else's writing.

The ONE MENTION label saves you from the usual mistake, which is building for one loud person. A single wish goes on a list to watch. It does not go into version one.

A simple way to turn the result into a plan is to make three short lists. What to fix comes from the biggest complaint counts, and what to keep comes from the praise.

What to ignore for now is every ONE MENTION. When you can say all three in one breath, you know what you are building.

One follow-up prompt turns the notes into first-page lines. Here it is with a real reply.

```
Using only the buyer words and the buyer sentence above, write 3 first-page lines for a simpler invoice tracker. No invented numbers or promises.
```

Output (generated with Claude Sonnet 5.5, 2026-11-12):

```
1. Add your first client without watching a video.
2. Built for three clients, not thirty tabs.
3. Totals you can check yourself, or no tax tab at all.
```

These are for the made-up product, so the point is the method. Each line answers one complaint from the table, and none promises something the reviews did not ask for.

### Run it on your own market

Pick one product that already sells in the area you are thinking about. Open its page and copy the reviews or comments you can see, ten to thirty if there are that many. Copy only what is public, and keep to the site's rules about copying.

If there are many five-star reviews, add some of the three-star and two-star ones too. Mild complaints are often the most useful because the buyer liked the product enough to explain what was missing.

Paste them under the prompt in a new chat. Check two or three quotes against the originals, because that is how you know the AI did not blend them. Then write the top complaint, the top praise and the buyer sentence on one page. That page is your brief before you build anything.

The method is not limited to templates. It works on reviews of courses, books, apps and prompt packs, and on the comments under a video about any of them. The only rule is that the words must come from people who used the thing.

Once you have the themes, you can ask for a second opinion on them. This follow-up is one we did not run here, because it needs your real reviews to mean anything. Use it on your own data.

```
Now look for reviews that disagree with the themes above. Quote each one. Then tell me which theme is the weakest and why.
```

That last step matters because an AI likes a neat story. Asking for the exceptions keeps the neat story honest, and it often shows a buyer type you had not noticed.

### Where it falls short

Eight reviews is a tiny sample. The counts in this story are fine to show the method, and thirty or more reviews will give you firmer ones. If your count is two, say two, not a majority.

The counts can also slip. Models are good at finding a theme and less reliable at adding up, so look at the review numbers it lists and check that they match.

Last, reviews show what unhappy and happy buyers chose to write. They do not show the people who bought nothing. Treat the result as strong evidence about one product's buyers, not as proof that your idea will sell.

For a test on prompts you find online, see our earlier story: [Is It Safe to Copy Ultimate ChatGPT Prompts? Run This 5-Check Test First](https://medium.com/@bryanargani1803/is-it-safe-to-copy-ultimate-chatgpt-prompts-run-this-5-check-test-first-8f37ec6e4683).

Try it on one real product page today. When you want more prompts, the free [AI Prompt Playbook](https://systemvault123.gumroad.com/l/ai-prompt-playbook-free?utm_source=blog&utm_medium=organic&utm_campaign=2026-11-12-medium-ai-review-mining-prompt) has 73 of them, free to [download](https://systemvault123.gumroad.com/l/ai-prompt-playbook-free?utm_source=blog&utm_medium=organic&utm_campaign=2026-11-12-medium-ai-review-mining-prompt).

Follow for a new copy-paste AI prompt guide every day.
