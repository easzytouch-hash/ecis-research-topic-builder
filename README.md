# ECIS Research Topic Builder

A free Claude skill that helps students, lecturers and researchers choose a research topic they can actually finish.

Most postgraduate students start with a problem in mind, not a polished topic. Many have never designed a study before, and most have jobs. This skill takes you from "I have noticed a problem" to a topic that fits your time, your data, your setting and your sample, and that rests on real background research.

Built by [ECIS Ink Services](https://github.com/easzytouch-hash), Gombe, Nigeria.

## What it does

- **Gets to know you first.** It asks about your output (journal article, master's or PhD thesis), your preferred approach (quantitative, qualitative or mixed), the data you can realistically collect, your time, your setting and your likely sample size. It reads your profile back to you before it suggests anything.
- **Suggests topics.** Each option names the study type, the independent and dependent variables (or the qualitative focus), the data needed, the likely analysis, how well it fits your capacity, and the journal articles a thesis could produce.
- **Confirms the gap before it validates.** It searches the literature, grades what already exists (a blog post is not the same as a rigorous study), and lets you decide the direction.
- **Moderates your own topic.** It checks the gap, duplication, feasibility against your real capacity, measurability, relevance, and whether the topic, aim and objectives line up.
- **Advises on supervisor-assigned topics.** It does not rewrite your supervisor's topic. It gives you the gap analysis, relevance, researchability and the different angles you could take, with the data each angle needs.
- **Includes Nigerian and African journals** in its searches, with a credibility check (peer review, indexing, warning signs of predatory publishing).
- **Removes duplicate sources** from every list it compiles. It keeps the most credible, best-indexed and most recent version, and asks you to choose when the same work appears in different editions or volumes.
- **Never invents evidence.** Every paper it mentions must come from a live search in your conversation and carry a link you can open. It labels its own judgement as judgement.

It does not choose your topic for you. You decide, and your supervisor has the final say.

## Install (works on the free Claude plan)

Claude's help centre states that skills are available on the Free, Pro, Max, Team and Enterprise plans, and that all plans can upload their own skills. The requirement is that "Code execution and file creation" is switched on in your settings. See [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

1. Download [`ecis-research-topic-builder.zip`](ecis-research-topic-builder.zip) from this repository. Do not unzip it.
2. In Claude, go to **Customize**, then **Skills**, and upload the zip.
3. Make sure **Code execution and file creation** is on in Settings.

## Add the FastTrack Connector for live literature search (recommended, free)

The skill is designed to work with the **FastTrack Connector**, a free literature search connector built by FastTrack. According to FastTrack, it searches roughly 250 million records from OpenAlex and Semantic Scholar and works on any Claude plan, including the free one. It is what lets this skill find real papers, check for duplication and look at citation records, with links you can open.

To add it:

1. In Claude, go to **Customize**, then **Connectors**.
2. Click **Add**, then **Add custom connector**.
3. Name it `FastTrack Connector`.
4. Paste this URL: `https://literature.researchfasttrack.com/mcp`
5. Choose **No sign-in** and leave any request-header fields empty, then click **Add**.
6. Set the tools to **Always allow**, so Claude does not ask before every search.

Full instructions are on the FastTrack page: https://www.researchfasttrack.com/skill

Without a live search tool, the skill tells you plainly that it cannot verify the literature and tells you what to search for yourself. It will not make up papers. If other tools are connected, such as PubMed or Consensus, it uses those too, and it can use web search to reach African Journals Online and Nigerian university repositories.

## How to use it

1. Invoke the skill, then tell it your research interest, the problem you would like to build a research around, or a draft topic you have in mind, and press enter.
2. It will take it from there. It asks a few questions about you first (your output, your data, your time and your setting), then suggests topics or checks yours.

For example, you can start with:

- "I have noticed a problem with staff turnover in hospitals in my state and I need a research topic for my master's thesis."
- "Is this topic researchable? [your topic]"
- "My supervisor gave me this topic. Help me understand the gap and what data I would need."

If you say "skip the questions", it will carry on and tell you which assumptions it made.

**Best used with:** Claude in Chrome. **Also works well with:** Claude Cowork and Claude Code, when a live browser is available. These are the author's recommendations from his own use.

## Limits

- Literature tools search titles, abstracts and metadata, not every full text. Some publishers withhold abstracts.
- Coverage of Nigerian and African journals, theses and grey literature is incomplete in global databases. A study missing from the results does not prove it does not exist. Check local repositories and your department's project archive too.
- Study counts and citation counts are rough indicators only.
- A long session may reach the usage limits of your Claude plan.
- Final approval of any topic belongs to your supervisor or institution.

## Acknowledgements and what belongs to whom

This skill would not exist in its current form without **FastTrack**.

- The **FastTrack Connector** is built and provided free by FastTrack, developed by Prof David Stuckler. This skill is designed to work with it, and the live literature search described above depends on it. To install the connector, please follow the instructions on the FastTrack page: https://www.researchfasttrack.com/skill

> The Duplication, Feasibility and Impact tests are adapted from the free FastTrack Topic Validator by Prof David Stuckler (https://www.researchfasttrack.com/skill) and are used with permission; they are not covered by this repository's MIT licence. The topic-suggestion, supervisor-topic and African-journal search features are ECIS additions and are not part of the FastTrack method.

FastTrack's own Topic Validator deliberately does not suggest topics. It keeps AI in the critic's seat and pressure-tests a topic the researcher brings, instead of generating one for them. This skill adds topic suggestion and a supervisor mode on top, so please do not read those parts as the FastTrack method.

| Part of this skill | Source |
|---|---|
| Duplication test | Adapted from the FastTrack Topic Validator, used with permission |
| Feasibility test | Adapted from the FastTrack Topic Validator, used with permission |
| Impact test | Adapted from the FastTrack Topic Validator, used with permission |
| Live literature search | The free FastTrack Connector, provided by FastTrack |
| Researcher intake, data-capacity and setting checks | ECIS Ink Services |
| Topic suggestion and building (Mode A), aim-and-objectives guidance | ECIS Ink Services, not part of the FastTrack method |
| Supervisor-assigned topic mode (Mode C) | ECIS Ink Services, not part of the FastTrack method |
| Nigerian and African journal search and credibility checks | ECIS Ink Services, not part of the FastTrack method |
| Duplicate-source removal rules | ECIS Ink Services |

This project is independent and is not endorsed by FastTrack, and ECIS Ink Services is not affiliated with FastTrack. Please visit [researchfasttrack.com](https://www.researchfasttrack.com/skill) to see their work and their other free tools.

## Licence

The [MIT Licence](LICENSE) in this repository applies **only to the original additions made by ECIS Ink Services**. It does **not** cover the FastTrack material: the Duplication, Feasibility and Impact tests are FastTrack's, used with permission, and are not released under an open licence. It also does not cover the FastTrack Connector or the original FastTrack Topic Validator. If you want to reuse or redistribute those parts, please contact FastTrack through their page.

## Feedback

Found a problem or have an idea? Please open an issue on this repository.
