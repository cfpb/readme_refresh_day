# README Rot Day notes


Starter docs:

- This repo's [README](README.md)
- <https://github.com/cfpb/open-source-project-template>


## Feedback from Marc's intro

- Seph: "A 'quick start', when possible, is very nice to have."
- Wyatt: "An example, when applicable, is great.
  Demo sites, usage examples, etc."
- Kimberly: "What does 'in progress' mean? I read it and think
  'the build is broken and it's experimental'."
- Marc: (relays the story of Qu)
- Chris: "For OAH, it's mainly that the content is not final."
- Kim: (raises the issue of badges)
- Marc: "Definitely add Travis integration if it's missing and appropriate."
- Irina: (suggests dependency badges, as well)
- Marc: "Other potential badges: Coveralls"

25 people = about 7 groups

Numbered off to 7

Sticky notes on the table: Asterisks need to be done, others optional.


## Presentations

### capital-framework

(The capital framework documentation site.)

- Smooth sailing, easy to set up.
- Added an issue about a missing `postinstall` hook.
- Observation from Marc: README mentions Homebrew... does it require a Mac? :)
- Questions about how in-depth we go with getting dependencies installed?

### regulations-parser

- Followed instructions and it worked extremely well,
  though Jerry would like to make a few changes to the initial Python script.
- And there were some assumptions about environment.

### owning-a-home

- Got through everything except the tests.
- Made a bunch of updates and clarifications to the language.
- Added step numbers to a lot of places that were just paragraphs.
- Interesting challenges around internal/external audience,
  and how to write this for folks who don't have access to our API.
  - Suggest adding Grunt stub-api task. (Issue added.)
- Biggest thing found: dependencies weren't clear. Wasn't clear that FEWDs need
  back-end dependencies, too.
- Steven to test updates.
- Marc: "Is virtualenv listed as a requirement?" No.
  Should add statement about this being a best practice.
- (listen back to audio for comment from Marc about Bower)

### owning-a-home-api

- README was originally just a little bit on what it was, and how to run tests.
- Just a pair of Django modules, but not a whole Django project, so it needed
  a fair bit of clarification on that.
- Added section on what each module actually does.
- Dug into the source code to figure it out.
- Still need to spend more time in the code to figure out what the parameters
  should be and how to validate them.
- Added more details on testing.
- Opened several different issues.
  - Version numbers are different everywhere.
  - There's no information on the form of the data that the API needs.
  - MySQL is needed to run the tests.
- (short discussion on work needing to be done to standardize versioning)

### clouseau

- Pretty good to begin with.
- What is a "silly git inspector"? Wasn't well explained.
  Intro has been improved.
- Split up the sections to some degree. Separated dependencies.
- Some clarifications made to the Basic Usage section.
- A little formatting cleanup.
- New fellows' laptops had the `clouseau` binary available everywhere,
  but older machines didn't. "Fresh VM" instructions needed to prepend `bin/`
  to the commands.

### sheer

- "What does it do? Why should you use it?" Hard to think of it
  from an outside perspective.
- README has some of this, but needed a lot of clarification.
- Demo site is just another repo; not that helpful.
- Java 1.7 is a dependency if you don't have root access,
  but there's a workaround.
- Didn't have time to make a PR, but filed a bunch of issues.

### cms-toolkit

- Documentation was already very good. (Has a TOC!) Just a few language tweaks.

### cfgov-refresh

- "What is it?" Not very extensive.
- Overall, pretty good. Made some language/order tweaks.
- Added a screenshot.
- Made a distinction between what is needed to just get it running and what
  is needed to develop on it.
- Clarifications on virtualenv usage. (A dependency for Sheer, but not
  extensively discussed here.)
- Clarifications on GovDelivery for external people.
- Suggested improvement for Grunt command flow.
- Tests moved above "Working with templates"
- Suggested possibly moving template information to separate file or to
  Sheer docs.
- Not yet hooked to Travis, but we should.

### mapusaurus

- Main issue: half public/half internal. Lots of internal stuff we can't share.
- README is mainly about how to set up server to create the API endpoint.
- Repo is both the API creation and setting up the Django app.
  One main task of this group was to clarify that in the README.
- Ran into issues setting up PostGIS and which add-ons are needed.
  Internally, this is solved via UnityBox.
  Hans tried doing this on a blank Ubuntu box to see how it went. Got close,
  but wasn't able to complete it in time.
- Travis and Coveralls badges added.
- Still needs more clarification work.
  Assuming lack of database would be a good idea.
- Maybe include Vagrantfile in repo? Can we make UnityBox public?
