## About me

![metal](https://img.shields.io/badge/music-heavy%20metal-black?logo=musicbrainz)
![history](https://img.shields.io/badge/interests-history-brown)
![whisky](https://img.shields.io/badge/drink-whisky-8B4513)
![foodie](https://img.shields.io/badge/foodie-yes-orange)

I build low-drama, high-quality software. Everything else I like is intense, old, or fermented.
People call me Jonur — it’s a long story.

### My professional story

I’m a Staff Engineer based in London, currently working mainly in the React / TypeScript / Node.js space, with a strong interest in architecture, AI-driven UX, and building things that don’t collapse under their own weight a year later.

These days my work sits less in “shipping isolated features” and more in shaping platforms: defining front-end foundations, setting standards, writing RFCs, unblocking teams, and rebuilding systems that have reached the end of their useful life. I tend to get pulled into the messy, cross-team problems — the ones where requirements are fuzzy, ownership is unclear, and the solution needs both technical depth and a lot of communication.

I’m currently a Staff Application Engineer at Bluefish AI, where I own product surfaces end-to-end — from an ambiguous ask through architecture to production. I write the RFCs that are reshaping how the product is configured org-wide, act as first responder on critical incidents, and I’m usually the person Product and Design escalate to when a requirement doesn’t have a clean answer yet.

Before that, I spent four and a half years at Tractable working across Pocket AI, the Inspection Portal, and the Auto Platform Product (APP). That included running AI models client-side with TensorFlow.js, migrating Pocket AI to a multi-tenant static React setup for low-bandwidth global performance, rebuilding large React applications from scratch, and designing shared libraries used across multiple teams. I was also heavily involved in defining testing strategy, localisation, analytics, and front-end architecture across the organisation — and helped unlock a chunk of new revenue along the way by embedding Pocket AI into partner products.

I care a lot about code quality, but not in a dogmatic way. I’m opinionated about structure, testing, and long-term maintainability because I’ve seen what happens when those things are ignored. I’m a big believer in boring, predictable systems that let teams move fast without breaking production — and in writing things down so the same mistakes aren’t repeated.

Before all that, I worked across a mix of product companies and consultative environments (Ladbrokes, Whitbread, Photobox), and earlier still I co-founded a small web agency in Greece. That mix has been useful — it's given me practice moving between code, architecture discussions, and conversations with product and design.

If you want a more formal breakdown of roles, tech stacks, and projects, my <a href="https://linkedin.com/in/dimitrisdamilos">LinkedIn</a> has the full timeline — this is the human version.

## Open source & side projects

### Open source

#### [react-super-switch](https://www.npmjs.com/package/react-super-switch)

[![npm version](https://img.shields.io/npm/v/react-super-switch)](https://www.npmjs.com/package/react-super-switch)
[![gzip size](https://img.shields.io/bundlephobia/minzip/react-super-switch)](https://bundlephobia.com/package/react-super-switch)
![dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)
![react](https://img.shields.io/badge/react-17%2B-blue)
![typescript](https://img.shields.io/badge/typescript-fully%20typed-blue)

Deterministic conditional rendering for React: from a set of mutually exclusive options, exactly one view renders.

Conditional rendering usually starts as a few `{condition && <View />}` lines and slowly turns fragile: two views render at once, priority is implied by order, and negated conditions get unreadable. `react-super-switch` makes the options explicit instead, with an optional priority and a default fallback, and fails loudly in development when the setup is wrong.

```tsx
<SuperSwitch>
  <Option condition={isLoading}>
    <Spinner />
  </Option>
  <Option condition={hasError}>
    <ErrorState />
  </Option>
  <Option default>
    <Results />
  </Option>
</SuperSwitch>
```

Ships at under 1KB min+gzip and is intended to be dropped into real-world codebases without ceremony.

[npm](https://www.npmjs.com/package/react-super-switch) · [Code](https://github.com/Jonur/react-super-switch)

### Small apps

Small apps I build to solve very specific problems of my own. Each one does a single job, runs on my own time and budget, and stays around for as long as it’s useful. They all live at **[apps.jonur.io](https://apps.jonur.io)**.

#### Apps

In daily use. Each one exists because something annoyed me enough.

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://metalradar.jonur.io"><img src="https://apps.jonur.io/thumbs/metalradar.jpg" alt="Metal Radar" width="400"></a><br>
      <a href="https://metalradar.jonur.io"><b>Metal Radar</b></a><br>
      <sub>metalradar.jonur.io</sub><br>
      A quiet daily digest of tours, festivals, albums and lineup news for the bands I follow.
    </td>
    <td width="50%" valign="top">
      <a href="https://giglog.jonur.io"><img src="https://apps.jonur.io/thumbs/giglog.jpg" alt="Giglog" width="400"></a><br>
      <a href="https://giglog.jonur.io"><b>Giglog</b></a><br>
      <sub>giglog.jonur.io</sub><br>
      Every gig I’ve been to and the ones still to come. Now part of Metal Radar, where the gig history carries on.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://gnt.jonur.io"><img src="https://apps.jonur.io/thumbs/gnt.jpg" alt="Greek National Teams" width="400"></a><br>
      <a href="https://gnt.jonur.io"><b>Greek National Teams</b></a><br>
      <sub>gnt.jonur.io</sub><br>
      Upcoming Greek national team games in basketball, football and water polo.
    </td>
    <td width="50%" valign="top">
      <a href="https://costie.jonur.io"><img src="https://apps.jonur.io/thumbs/costie.jpg" alt="Costie" width="400"></a><br>
      <a href="https://costie.jonur.io"><b>Costie</b></a><br>
      <sub>costie.jonur.io</sub><br>
      A real-time meeting cost calculator. Client-side only, nothing leaves your browser.
    </td>
  </tr>
</table>

#### Websites

Sites I built for people I know.

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://www.eleanagkogka.design/"><img src="https://apps.jonur.io/thumbs/eleanagkogka.jpg" alt="Eleana Gkogka" width="400"></a><br>
      <a href="https://www.eleanagkogka.design/"><b>Eleana Gkogka</b></a><br>
      <sub>eleanagkogka.design</sub><br>
      Portfolio of product designer Eleana Gkogka.
    </td>
    <td width="50%" valign="top">
      <a href="https://www.maria-athanaseli.com/"><img src="https://apps.jonur.io/thumbs/maria-athanaseli.jpg" alt="Maria Athanaseli" width="400"></a><br>
      <a href="https://www.maria-athanaseli.com/"><b>Maria Athanaseli</b></a><br>
      <sub>maria-athanaseli.com</sub><br>
      Personal trainer, Pilates instructor and exercise nutritionist.
    </td>
  </tr>
</table>

#### Legacy

Still online, no longer needed. Kept around because the work is worth showing.

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://aowformationshare.jonur.io"><img src="https://apps.jonur.io/thumbs/aowformationshare.jpg" alt="AoW Formation Share" width="400"></a><br>
      <a href="https://aowformationshare.jonur.io"><b>AoW Formation Share</b></a><br>
      <sub>aowformationshare.jonur.io</sub><br>
      Formation sharing helper for Art of War: Legions.
    </td>
    <td width="50%" valign="top">
      <a href="https://aowranking.jonur.io"><img src="https://apps.jonur.io/thumbs/aowranking.jpg" alt="AoW Ranking" width="400"></a><br>
      <a href="https://aowranking.jonur.io"><b>AoW Ranking</b></a><br>
      <sub>aowranking.jonur.io</sub><br>
      Hero and troop tier lists for Art of War: Legions.
    </td>
  </tr>
</table>
