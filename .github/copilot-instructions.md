# Instructions for Copilot in this repo

This repo is a practice project for Main Street Hardware & Feed, a fictional
family hardware and feed store. The owner, Dale, is not technical. The people
using you are beginners who do not write code. They read your plan, approve
each command, and check your results against Dale's register sheet.

## The data

* `data/raw/` holds Dale's monthly sales exports. Columns: date, item,
  category, quantity, unit_price.
* `data/register_totals.csv` is the store's own monthly report (net sales
  after returns, by category and for the whole month). It is the independent
  source we check against. Never change it.
* Never change any file in `data/raw/`. Write cleaned results to new files.

## Rules for cleaning

1. List every change you make, in plain words, before and after you make it.
2. Never delete a row without telling us which rows, how many, and why.
3. Write dates as YYYY-MM-DD.
4. Never invent, guess or fill in numbers. If something is missing, say so.
5. Use Python with pandas. Put scripts in a `scripts/` folder, keep them short,
   and add a comment above each step that says what it does in plain words.
6. When you run a command, say first what it will do.
7. After cleaning, report: rows before, rows after, and the reason for any
   difference.
8. When asked for monthly totals, use the same layout as
   `data/register_totals.csv` (month, category, units, net_sales, with a
   Month total row) so the two files are easy to compare.

## How to talk to us

* Explain simply, with no jargon. If you must use a technical word, explain it.
* Ask us before guessing anything.
* This repo is public. Never add personal info, passwords or real data.
