Start a personal build project. Produce the planning artefacts, sized to the project, then set up the repo. Do not wrap a weekend job in enterprise process.

$ARGUMENTS

The point is to make the thinking visible: what change the project is for, what it will not do, and how I will know it worked. The sizing step is the discipline. A full PRD on a two-hour build is process for its own sake, and it reads as someone who cannot right-size their own work.

Work through the steps in order. Write each artefact to a file, do not just discuss it.

## Step 1: Size the project

Estimate the size and confirm it with me:

- XS / S, hours to a single weekend: one-pager only.
- M or larger, several weekends or real users other than me: one-pager, plus a short measurement plan and acceptance criteria.

User stories are for handing work to a team that needs shared acceptance criteria. On a solo build I am the engineer, so acceptance criteria on the one-pager do the same job. Skip user stories unless the project has other contributors.

## Step 2: One-pager

Write `docs/one-pager.md` with these rows:

- Outcome: one sentence. The change in the world, not the feature list.
- Problem: the specific problems this addresses, as plain lines.
- Hypothesis: one statement in the form "Building X will reduce / increase / improve Y."
- Features: the proposed features, as plain lines.
- Metrics: measure the outcome, not the features. Name the concrete thing being counted, not an abstract metric label.
- Non-goals: what v1 will not do, and what has been cut to keep it small.

The Non-goals row is not optional and must not be empty. It is where scope discipline shows.

## Step 3: Scope

Write a short scope section: In, Out, Cut for v1. The "Cut for v1" list must have at least one real item that it would have been reasonable to include.

## Step 4: Measure and limit

- Pick the single outcome metric from the one-pager. One, not a dashboard.
- State the v1 boundary in one line: what "done" means for the first release, and what is explicitly deferred.

## Step 5: Kick off

- Initialise the repo, create the structure, first commit containing the one-pager.
- Draft a README stub: what the project is, in my voice.
- Add the next three concrete actions somewhere I will see them.

## Voice

Any prose this produces that I will publish (README, one-pager Outcome and Problem rows, project description) follows my writing style. Load my style guide first if I have one; the `draft` skill does this. Short sentences by default. British English. No em dashes, use commas or a new sentence. Complicate flat claims rather than stating them flat, and name the limits of what the project does.

## Attribution

When the project builds on someone else's concept or framing:

- Credit them by name at first mention, with a link to the original source.
- Quote their own words directly, in quotation marks, rather than rewording their explanation as if the framing were mine.
- Keep any quoted extract short, a sentence or two. Brief, marked, and sourced is the copyright-safe form. Do not reproduce long passages.
- My own words carry everything else: what I have adapted, why, and what my version does differently.
