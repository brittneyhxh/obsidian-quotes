<%*
const quotesFolder = "Quotes"; // folder OR file name
let quotes = [];

// Read all markdown files in folder
const files = app.vault.getMarkdownFiles()
  .filter(f => f.path.startsWith(quotesFolder));

for (const file of files) {
  const content = await app.vault.read(file);

  // Extract blockquotes
  const matches = content.match(/^>[\s\S]*?(?=\n\n|$)/gm);
  if (matches) quotes.push(...matches);
}

if (quotes.length === 0) {
  tR += "> No quote found.";
} else {
  const random = quotes[Math.floor(Math.random() * quotes.length)];
  tR += random;
}
%>
