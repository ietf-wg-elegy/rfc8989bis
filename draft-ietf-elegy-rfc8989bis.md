---
title: Nominating Committee Eligibility
abbrev: RFC8989bis
docname: draft-ietf-elegy-rfc8989bis-latest
category: bcp

ipr: trust200902
area: General
workgroup: ELEGY
keyword: Internet-Draft
obsoletes: 8989
updates: 8713

stand_alone: yes
smart_quotes: no
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: M. Duke
    name: Martin Duke
    organization: Google LLC
    email: martin.h.duke@gmail.com

normative:

informative:


--- abstract

The IETF Nominating Committee (NomCom) appoints candidates to several IETF
leadership committees. RFC8713 provides criteria for NomCom membership that
attempt to ensure that NomCom volunteers are members of the loosely defined
IETF community, by requiring in-person attendance in three of the past five in-
person meetings. In 2020 and 2021, the IETF had six consecutive fully online
plenary meetings that drove rapid advancement in remote meeting technologies and
procedures, including an experiment that included remote attendance for NomCom
eligibility. This document updates RFC8713 by defining a new set of eligibility
criteria from first principles, with consideration to the increased salience of
remote attendance.

--- middle

# Introduction

{{!RFC8713}} defines the process for the selection of the Internet Architecture
Board (IAB), Internet Engineering Steering Group (IESG), IETF Trust, and one
IETF LLC Director. A key actor in the process is the Nominating Committee
(NomCom), which nominates a single candidate for each open position, subject to
confirmation by other bodies.

NomCom voting members are volunteers that have met certain eligibility
requirements. The actual NomCom is selected at random from the pool of eligible
volunteers. Thus, it is important that members of the pool be IETF participants
likely to have knowledge of IETF processes and practices. There are restrictions
to ensure that no more than two volunteers with the same primary affiliation are
chosen.

{{Section 4.14 of RFC8713}} requires that volunteers must have attended three of
the previous five meetings. In practice, this has meant that the volunteer
picked up their registration badge at an in-person meeting. Current members of
the Internet Society Board of Trustees and bodies for which the NomCom nominates
members are ineligible.

{{?RFC8989}} specified an experiment in the wake of six consecutive fully online
meetings from 2020 to 2021, where the historic interpretation of the requirement
would have resulted in no eligible volunteers. It extended the attendance
requirement to define meeting attendance as including logging in to at least one
session of a fully-online IETF meeting.

RFC8989 also created two other tracks to obtain eligibility: (1) serving as a
working group chair or secretary in the past three years, and (2) author or
editor of an IETF Stream RFC in the past five years, including internet-drafts
in the RFC Editor queue.

This document discusses some of the first principles that inform the design of
NomCom eligibility, and makes recommendations on how the process of
qualification based on attendance should work.

This document replaces the attendance criteria in the first two paragraphs of
{{Section 4.14 of RFC8713}} with criteria based on those in {{?RFC8989}}, and
obsoletes RFC8989 to make it clear that that document has been superseded. All
other text in {{RFC8713}}, including the other paragraphs of Section 4.14,
remains unchanged.

# NomCom Principles

The NomCom is intended to be composed of randomly selected members of "the
community." For many years, in-person attendance was a reasonable proxy for the
commitment associated with being a member. Two days of travel and an attendance
fee is a relatively large expenditure of time and money. Additionally, in-person
attendance is thought to increase personal familiarity with candidates for
leadership positions and with the spirit of the IETF, although there is no
mechanism to ensure any interactions.

A basic principle is that the community should govern itself, so volunteers
must have a demonstrated commitment to the IETF. Limiting the number of
volunteers sponsored by any one organization avoids the potential for mischief
that disrupts IETF operations or works against the interests of the community as
a whole.

However, attitudes to business travel evolve, and remote meeting technology
continues to improve, to the extent that many longstanding community members
choose to participate remotely. A requirement for in-person attendance has
always excluded some from qualification from the NomCom, due to cost or personal
reasons. Further, the NomCom has completed two cycles using entirely online
tools.

Counting remote attendance lowers the barriers to entry. As the IETF is
committed to having a no-fee remote option ({{?I-D.ietf-shmoo-remote-fee}}) the
only required investment is to log on once per meeting at a specific time
(sometimes a locally inconvenient hour). While this document does not formally
impose a requirement for the NomCom to function entirely remotely, including
remote-only attendees in the pool is likely to effectively require a remote
component to NomCom operations.

Finally, overly restrictive criteria work against getting a broad talent pool.

# Criteria

The following text replaces the first two paragraphs of
{{Section 4.14 of RFC8713}}:

Members of the IETF community must satisfy the conditions in one of three paths
in order to volunteer. Any one of the paths is sufficient, unless the person is
otherwise disqualified under {{Section 4.15 of RFC8713}}.

Path 1:
The person has registered for and attended three out of the last five IETF
meetings, either in-person or online. In-person attendance is as determined by
the record keeping of the Secretariat. Online attendance is based on being a
registered person who logged in for at least one session of an IETF meeting.

Path 2:
The person has been a Working Group Chair or Secretary within the three years
prior to the day the call for NomCom volunteers is sent to the community.

Path 3:
The person has been a listed author or editor on the front page of at least two
IETF Stream RFCs within the last five years prior to the day the call for
NomCom volunteers is sent to the community. An Internet-Draft that has been
approved by the IESG and is in the RFC Editor queue counts the same as a
published RFC, with the relevant date being the date the draft was added to the
RFC Editor queue. For avoidance of doubt, the five-year timer extends back to
the date five years before the date when the call for NomCom volunteers is sent
to the community.

# Security Considerations {#security-considerations}

## NomCom Capture

The most potent threat associated with NomCom eligibility is that an
organization or group of coordinating organizations could attempt to obtain a
majority of NomCom positions, in order to select an IETF leadership in support
of an agenda that might be self-serving and against the interests of the
community as a whole.

Note that {{!RFC8713}} lets the NomCom Chair decide the NomCom voting
requirement, so a simple majority may be inadequate. However, seven of ten forms
a quorum, so at worst seven NomCom members working together can almost certainly
impose their will.

Whatever the merits of admitting remote attendees, it reduces the minimum cost
of creating a NomCom-eligible volunteer from three in-person trips of around
five days each over the course of at least eight months, to zero financial cost
and the time required to log in three times over at least eight months. Some
organizations might not be deterred in either case, while others might now find
such an attack to not be feasible.

### A Surge of Volunteers

A large number of legitimate volunteers makes it quite difficult to control six
of ten NomCom slots. Setting aside limitations on the number of selections from
any organization, basic probability shows that to have even a 50% chance of
controlling six or more NomCom positions, an attacker needs roughly 60% of the
volunteer pool. For example, if there are 300 "legitimate" volunteers, an
attacker must produce 365 volunteers to exceed a 50% chance of NomCom capture
(see {{capture-math}}).

A sudden surge in the number of volunteers, particularly of people that no one
recognizes as a part of the community, is an early-warning sign for the
community, leadership and the IETF Secretariat to further investigate. The
community should monitor and assess a sudden increase in the number of online
registration fee waivers awarded in accordance with
{{Section 4 of I-D.ietf-shmoo-remote-fee}}.

While loosening eligibility criteria lowers the cost to an attacker of producing
eligible volunteers, it also increases the number of legitimate volunteers that
increases the difficulty of an attack.

### The Two-Per-Organization Limit

The two-per-organization limit in {{RFC8713}} complicates such an attack.  To
circumvent it, an organization must either (1) coordinate with at least two
like-minded organizations to produce a NomCom majority, (2) incentivize members
of other organizations (possibly through a funding agreement) to support its
agenda, or (3) propose candidates with false affiliations.

While the IETF does not routinely confirm the affiliation of volunteers, as part
of an investigation it could eliminate volunteers who have misrepresented said
affiliation. Publishing the list of volunteers and affiliations also gives the
community an opportunity to review the truth of such claims.

Assuming that 300 legitimate volunteers are all from different organizations,
three conspiring organizations would need 771 volunteers (257 per organization)
for a 50% chance of NomCom capture (see {{capture-math}}).

### One Year of Participation

Attendance at three meetings requires at least eight months of waiting. Given
the volume of volunteers necessary to capture the process, an attack requires a
surge in attendees over the course of a year. Such a surge might trigger a
community challenge to the list of eligible volunteers, and/or a leadership
investigation to detect suspicious behavior (e.g., logging in to a single
session and then immediately logging out). In the event of abuse of process, the
leadership would then have months to adjust policy in response before the NomCom
cycle begins.

## Disruptive Candidates

Note that the counting remote participation towards NomCom eligibility allows
for a single individual to mount an attack that previously required
coordination. By registering for remote attendance to IETF meetings using a
number of different identities over a year, an individual can make each of those
identities NomCom eligible and then serve under any one of them that is selected
for the NomCom. Once selected, an individual could seek to disrupt the process
or prevent the timely conclusion of its work. Less severely, an attacker could
simply improve their chances of being selected for NomCom.

This attack is much harder to detect or prevent than equivalent attacks were
previously, as it does not require coordination among multiple attendees.
While the attacker cannot be sure of fee waivers for some or all of the
different identities, the lower cost for remote participation also makes this
attack more feasible than it would have been under prior rules.

However, the voting member recall procedure in {{Section 5.7 of RFC8713}} exists
to allow removal and replacement of disruptive figures.

## Additional Remedies

Additional changes to the process to further obstruct attacks against the
NomCom are beyond the scope of this document. However, a challenge process
against volunteers with a suspicious reported affiliation, or that might be
aliases of a single volunteer, could trigger an investigation.

Similarly, the challenge to the random selection described in
{{Section 4.17 of RFC8713}} can explicitly include appeals against the data
used to qualify the volunteer, rather than the randomization process.

# IANA Considerations

This document has no IANA actions.

--- back

# NomCom Capture Calculations {#capture-math}

{{security-considerations}} offers some mathematical results for the probability
of NomCom capture. This appendix shows the work.

Note that the number of combinations of b items chosen from a population of a
item is often expressed as

~~~math
\binom{a}{b} = {\frac{a!}{(a-b)!b!}}
~~~
{: #peq1 artwork-align="center" }

## No per-organization limit

The first computation assumes there is no limit of two per organization,
or equivalently, no organization produces more than two volunteers.

Let L be the number of "legitimate" volunteers (i.e. those not allied with an
attacker" and A be the number of attacking volunteers. Then there are

~~~math
\binom{L+A}{10}
~~~

ways to select a NomCom. The number of outcomes where attackers capture the
NomCom is

~~~math
\sum_{i=6}^{10}\left[\binom{A}{i} \binom{L}{10-i}\right]
~~~
{: #peq2 artwork-align="center" }

and the probability of capture is therefore

~~~math
\sum_{i=6}^{10}{\frac{\binom{A}{i} \binom{L}{10-i}}{\binom{L + A}{10}}}
~~~
{: #peq3 artwork-align="center" }

For L = 300, this probability crosses 50% at A = 365.

## Two per Organization

Assume that the population of L is drawn from L different organizations (this
assumption is unfavorable to the attacker). Assume also that there are three
conspiring organizations. Then no more than 6 members can be drawn from A.

Let B be the number of nominees per attacking organization, so that A = 3B.

The number of combinations to pick exactly N attackers, N <= 6, is

~~~math
C(N) = \binom{L}{10 - N} \sum_{i=0}^{min(N,2)}\left[\binom{B}{i} \sum_{j=0}^{min(2,
N-i)}\left(\binom{B}{j} \binom{B}{min(2, N-i-j)}\right)\right]
~~~
{: #peq4 artwork-align="center" }

And the probability of capture is

~~~math
{\frac{C(6)}{\sum_{i=0}^{6}C(i)}}
~~~
{: #peq5 artwork-align="center" }

For L = 300, the A required to exceed a 50% probability of capture is 771.

# Change Log

> **RFC Editor's Note:** Please remove this section prior to
> publication of a final version of this document.

## Since draft-duke-elegy-rfc8989bis-00

* Added more security considerations
* Editorial improvements

## Since draft-duke-gendispatch-rfc8989bis-00

* Matched normative section to RFC8989
* Added security considerations and appendix

# Acknowledgments

Brian Carpenter and Stephen Farrell wrote RFC8989, which provides the core of
this document.

Luc André Burdet, Brian Carpenter, and Donald Eastlake provided useful
editorial suggestions.

{:numbered="false"}
