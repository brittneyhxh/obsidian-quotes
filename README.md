# Obsidian Quotes
Store quotes in Markdown files for Obsidian.

Automating daily quotes pulled from MD files in this repository to randomly display on Obsidian whenever a new daily note is created. 

This is a personal project. Quotes are sourced from books I have personally read or have come across - will try to update every year.

> **"A page, turning, is a wing lifted with no twin, and therefore no flight. And yet we are moved."**
>
> — On Earth We're Briefly Gorgeous, Ocean Vuong

<br>

Quotes Markdown file
  - Source of truth for quotes

Quotes folder
  - Collection of quotes in files by source 
  - Not used in practice, but neat way to organize all quotes by book/movie/source

<br>

## Set-up Walkthrough
1. On Obsidian, download the **Templater** plug-in from _Community plugins_
   
2. In the settings:
    - Set up a proper folder for _Template folder location_
    - Toggle on _Trigger Templater on new file creation_

3. Create a **markdown file with all quotes** compiled into one place. Make sure each quote consists of blockquotes '>'. Each quote is seperated by an empty line.
    - As a sample, use the all_quotes.md provided in this repo.
  
4. Create a **template file to retrieve a random quote** once run.
    - As a sample, use the daily_quote.md provided in this repo.
  
5. Create a **template file for daily notes**. Note this is already a core plug-in for Obsidian.
    - As a sample, use the daily_notes.md provided in this repo.
