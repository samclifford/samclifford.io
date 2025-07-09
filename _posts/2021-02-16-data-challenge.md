The new Masters of Health Data Science at LSHTM is now in halfway
through its second term in its first offering. I ended up volunteering
to not just module organise for one of the term 2 modules but to teach
into the other (2490 Machine Learning). My module, 2491 Data Challenge,
sees students organising themselves into teams and bidding for the
available projects with our partner organisations.

Over the course of four weeks they meet with the client, scope out the
project, do some exploratory data analysis, formulate a model for
analysis, do some model checking, create some publication-ready plots,
and then create an executive summary, final report, and presentation to
the client.

The project is done under the supervision of an internal LSHTM staff
member who may have some expertise in the topic or likely analysis
techniques that will be used, but this is not necessary. I supervised a
group who were working on linking air pollution data ([as modelled by
DEFRA](https://uk-air.defra.gov.uk/data/modelling-data)) and prescribing
patterns of antidepressants from the
[OpenPrescribing](https://openprescribing.net/) platform.

One of the things I really like about the cohort in the MSc is that they
have a variety of backgrounds, skills and interests. When we were
planning the Masters programme we decided that students coming in should
have strenghts in either the maths/stats of data science, or at least a
semi-quantitative background in health or biology. This has meant that

## Reflective essay

To ensure that students weren’t just given group marks for the overall
grade we put together a reflective essay task. The PGCILT reflective
task was a good template for this, but we needed it to be short enough
that it wasn’t an onerous task. We provided some prompts for their
reflection, such as their prior experience with group work or working
for a client, decision making processes and division of tasks. Informal
chats with students have indicated that they’ve enjoyed the experience
overall and learned a lot from the experience of working with a team
with a varied skill set on a real-world problem.

<!-- * What was your previous experience of group work and how did this compare? Have you worked on a group project with a supervisor? -->
<!-- * How was your team chosen and did you all agree on which project you would pitch for? -->
<!-- * What was your experience of the initial client meeting? Did your understanding of how it went match the feedback given by the client? -->
<!-- * Did you volunteer for tasks that you knew you would be good at or did you seek to try new challenges during the project? -->
<!-- * How well did the team work collaboratively to complete the project? Were people each given a section to complete or did people work in small groups to complete discrete tasks? -->
<!-- * Did the team always agree on a course of action? -->
<!-- * Did you contribute to group discussions as much as you would have liked to? -->
<!-- * Do you feel like you supported your team to the best of your ability? Do you feel like your team supported you according to your needs? -->
<!-- * Have you ever given a presentation to a client before in a professional context? How did this compare? -->
<!-- * Did the conclusion to your report discuss the uncertainties in the analysis and what, if any, additional work would be required to provide a fuller answer? -->
<!-- * Do you have an interest in doing further work on this topic? -->

As part of the reflection on their experience in the module, we ask the
students to fill out a survey on how well each member of their team
contributed to the project. This is based on the approach we took in
SEB113 at QUT but includes a few questions on client engagement and
contribution to the various tasks. We ensure that students know that
while this isn’t an anonymous process, it is a confidential one. This is
the first time I’ve run this with postgraduate students and as rare as
it is for undergraduate students to not contribute to a project it seems
that everyone in 2491 put in a great effort to complete their projects.
I’m very proud of how each group went, and their client presentations
all indicated that a great deal of thought had been put into their
projects and how to present the information.

## Visualisation

I’ve previously taught visualisation with ggplot2 in the 2031
Statistical Computing module as a 90 minute lectorial. This time around
I had a 90 minute session on exploratory data analysis in week 1 and
then a three hour session in week 4 on publication-ready graphics. The
second session was a good opportunity to distill some of the things I’ve
picked up along the way from undergrad to assistant professorship on how
to communicate visually, as well as the mechanics of implementing ideas
in R.

One of the things I really enjoyed diving a bit deeper into was thinking
about how to account for common visual impairments, which was kicked off
by a tweet (below) about how focussing on colourblindness ignores far
more common visual impairments to do with low vision, such as acuity and
contrast-sensitivity (WHO 2020).

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Data visualization cares disproportionately far too much about designing
for colorblindness relative to other disabilities that are more common
(visual impairments included).<br><br>(A thread on disability, race, and
patriarchy in data visualization.)
</p>
— Frank ⌁ (@FrankElavsky)
<a href="https://twitter.com/FrankElavsky/status/1351311898428362754?ref_src=twsrc%5Etfw">January
18, 2021</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

This lead to including a discussion in the slides about how colour must
be chosen deliberately and with a view to using contrast (Stone 2006;
Few 2008) but with sensible colour palettes (Brewer et al. 1997) as well
as the other aspects of a plot geometry we have control over (Kunz and
Hurni 2011). We also had a few slides on how to choose fonts that are
easier to read (France 2020) and to make sure the text annotations are
similar in size to the body text.

It might be necessary to rejig things a little, moving some more of the
theory into pre-lecture reading so that the synchronous learning
sessions make better use of the time we have everyone together. I did
enjoy the outcome of the practical exercise of making the best and worst
graphs from the gapminder data. One group

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">
Each time I deliver the prac on making effective plots I give students a
plot (and code) to critique regarding Tufte's principles of graphical
excellence and Few's and Brewer's notes about use of colour to show
meaning in an interpretable way. Here's what they get.
<a href="https://twitter.com/hashtag/LSHTM2491?src=hash&amp;ref_src=twsrc%5Etfw">\#LSHTM2491</a>
<a href="https://t.co/aPkjUCyJ6m">pic.twitter.com/aPkjUCyJ6m</a>
</p>
— Sam Clifford (@samclifford)
<a href="https://twitter.com/samclifford/status/1357820207922823168?ref_src=twsrc%5Etfw">February
5, 2021</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## References

Brewer, Cynthia A., Alan M. MacEachren, Linda W. Pickle, and Douglas
Herrmann. 1997. “Mapping Mortality: Evaluating Color Schemes for
Choropleth Maps.” *Annals of the Association of American Geographers* 87
(3). Informa UK Limited:411–38.
<https://doi.org/10.1111/1467-8306.00061>.

Few, Stephen. 2008. “Practical Rules for Using Color in Charts.” *Visual
Business Intelligence Newsletter* 11. Perceptual Edge.
<http://www.perceptualedge.com/articles/visual_business_intelligence/rules_for_using_color.pdf>.

France, Tiffany. 2020. “Choosing Fonts for Your Data Visualization.”
*Nightingale*. Medium.
<https://medium.com/nightingale/choosing-a-font-for-your-data-visualization-2ed37afea637>.

Kunz, Melanie, and Lorenz Hurni. 2011. “How to Enhance Cartographic
Visualisations of Natural Hazards Assessment Results.” *The Cartographic
Journal* 48 (1). Informa UK Limited:60–71.
<https://doi.org/10.1179/1743277411y.0000000001>.

Stone, Maureen. 2006. “Choosing Colors for Data Visualization.”
*Business Intelligence Network* 2.
<http://www.perceptualedge.com/articles/b-eye/choosing_colors.pdf>.

WHO. 2020. “Visual Impairment and Blindness Fact Sheet 282.”
<https://www.who.int/news-room/fact-sheets/detail/blindness-and-visual-impairment>.
