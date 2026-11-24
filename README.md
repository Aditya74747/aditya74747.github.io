# Aditya Ghatage, portfolio

**A machine learning engineer's portfolio, written as a model card.**

Turning data into decisions, and models into products. This site is my model card: what I've
trained on, how I was evaluated, and my known limitations.

Live site (once published): https://aditya74747.github.io/

## The idea

Machine learning models ship with a *model card*: an overview, the training history, evaluation
results and an honest list of limitations. This site does the same for me.

- **Model overview:** who I am, in four minutes
- **How I work:** raw data in, a grounded answer with a source out (the dots dodge your cursor)
- **In numbers:** four figures, each with its source
- **Work delivered:** Leejam Sports, Accenture and Skyrise Education
- **Projects:** MCP Agent Database, a privacy-first RAG assistant, a legal
  contract analysis AI and an AutoParts inventory system, with a scroll chapter where the agent
  stops and asks for approval
- **Research and recognition:** registered software copyright, co-authored paper, M.Sc.
- **Feature set:** my skills, which start as unlabelled dots and cluster themselves into five branches
- **Off duty:** three photos outside the lab, captioned like test results
- **Known limitations:** the funny part
- **Next steps:** how to reach me

A switch at the top flips the whole site between the light **Human view** and a dark, amber
terminal **Model view**, where every section title is rewritten as code.

## How it's built

Plain HTML, CSS and JavaScript in one file (`index.html`), no frameworks and no build step.
Photos and fonts live in `assets/`. It respects the reduce-motion setting and works on phones.

## Publish it on GitHub Pages

1. Create a public repository named **`aditya74747.github.io`** on GitHub.
2. Upload everything in this folder (`index.html`, `README.md`, `.nojekyll`, `assets/`).
3. In the repository, open **Settings → Pages**, set the source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`, and save.
4. After a minute the site is live at https://aditya74747.github.io/

## Run it on your computer

Double-click `index.html`, or start a small local server in this folder and open
http://localhost:8000:

```bash
python -m http.server 8000
```

## Make changes

- **Text:** search `index.html` for the sentence and edit it in place.
- **Photos:** replace the files in `assets/` with new ones of the same name. The hero photo
  (`aditya-hero.webp`) is a cut-out with a transparent background.
- **Colours:** `:root` near the top of the `<style>` block holds the Human view colours,
  `:root[data-mode="dev"]` holds the Model view colours.
- **Model view titles:** each heading has a `data-dev="..."` attribute with its code version.
- **Projects from GitHub:** every public repo on github.com/Aditya74747 that isn't a fork or archived
  gets a card automatically, newest first, after the four hand-made cards. The card uses the
  repo's description, topics, language and website. To keep a repo off the site, add the topic
  `hide-from-portfolio` to it on GitHub. The hand-made cards are listed in `SKIP` in `index.html`.

## Credits

The design is based on my friend [Kush Vankawala's portfolio](https://kushrvankawala.github.io/).
Adapted and built with help from Claude by Anthropic. Fonts (Bricolage Grotesque, Hanken Grotesk,
Martian Mono, Caveat) are open source under the SIL Open Font License; their licences are in
`assets/fonts/`.

© 2026 Aditya Ghatage. The photos and personal content on this site are mine.
