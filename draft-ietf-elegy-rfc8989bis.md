---
title: Nominating Committee Eligilibity
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
    organization: Google
    email: martin.h.duke@gmail.com

normative:

informative:


--- abstract

The IETF Nominating Committee (NomCom) appoints candidates to most IETF
leadership committee. RFC8713 provides criteria for membership on NomCom that
attempt to ensure that NomCom volunteers are members of the loosely defined
IETF community, by requiring in-person attendance in three of the past five in-
person meetings. In 2020 and 2021, the IETF had six consecutive fully online
plenary meetings that drove rapid advancement in remote meeting technologies and
procedures, including an experiment that included remote attendance for NomCom
eligibility. This document updates RFC8713 by building a new set of eligibility
criteria from first principles, with consideration for the increased salience of
remote attendance.

--- middle

# Introduction

{{!RFC8713}} defines the process for selection of the Internet Architecture
Board (IAB), Internet Engineering Steering Group (IESG), IETF Trust, and the
IETF LLC Director. These four committees form the senior leadership of the IETF.
A key actor in the process is the Nominating Committee (NomCom), which nominates
a single candidate for each open position from the pool of volunteers, subject
to confirmation by other bodies.

NomCom voting members are themselves volunteers that have met certain
eligibility requirements. The actual NomCom is selected at random from the pool
of eligible volunteers, with restrictions to ensure that no more than two
volunteers with the same primary affiliation are chosen.

{{Section 4.14 of RFC8713}} requires that volunteers must have attended three of
the previous five in-person meetings. In practice, this has meant that the
volunteer picked up their registration badge. Current members of the Internet
Society Board of Trustees, IETF Trust, LLC Board, IAB, and IESG are ineligible.

{{?RFC8989}} specified an experiment in the wake of six consecutive fully online
meetings from 2020 to 2021, where the traditional interpretation of the
requirement would have resulted in no eligible volunteers. It extended the
attendance requirement to define meeting attendance as including logging in to
at least one session of a fully-online IETF meeting.

RFC8989 also created two other tracks to obtain eligibility: (1) serving as a
working group chair or secretary in the past 3 years, and (2) author or editor
of an IETF Stream RFC in the past five years, including internet-drafts in the
RFC Editor queue.

This document discusses some of the first principles that inform the design of
NomCom eligibility. It makes recommendations on how the future process should
work. Its objective is to eventually replace Section 4.14 of RFC8713 with
criteria loosely based on those in RFC8989.

# Conventions and Definitions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL
NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED",
"MAY", and "OPTIONAL" in this document are to be interpreted as
described in BCP 14 {{!RFC2119}} {{!RFC8174}} when, and only when, they
appear in all capitals, as shown here.

# NomCom Principles

The NomCom is intended to be composed of randomly selected members of "the
community." For many years, in-person attendance was a reasonable proxy for the
commitment associated with being a member. Two days of travel and an attendance
fee is a relatively large expenditure of time and money. Additionally, in-person
attendance is thought to increase personal familiarity with candidates for
leadership positions, although there is no mechanism to ensure any interactions.
Finally, the NomCom interview process was largely conducted in-person at IETF
meetings, so the ability to attend was a prerequisite to participate.

Beyond the principle that the community should govern itself, selecting
volunteers with a demonstrated commitment to the organization, while limiting
the number from any organization, avoids the potential for mischief via
nominations that disrupt IETF operations or work against the interests of the
community as a whole.

However, attitudes to business travel evolve, and remote meeting technology
continues to improve, to the extent that many longstanding community members
choose to participate remotely. The system has always excluded community members
due to cost or personal reasons. Further, the NomCom can now fully complete its
business using online tools.

Counting remote attendance lowers the barriers to entry. As IETF is committed to
having a no-fee remote option ({{?I-D.ietf-shmoo-remote-fee}}) the only
required investment is to log on once per meeting at a specific time (sometimes
a locally inconvenient hour). While this document does not formally impose a
requirement for the NomCom to function entirely remotely, including remote-only
attendees in the pool is likely to effectively require a remote component to
NomCom operations.

Finally, it is historically difficult to recruit volunteers for NomCom, so
overly restrictive criteria work against getting a deep talent pool.

# Criteria

The following paths to qualification replace {{Section 4.14 of RFC8713}}. Any
one of the paths is sufficient, unless the person is otherwise disqualified
under {{Section 4.15 of RFC8713}}.

Path 1:
The person has registered for and attended 3 out of the last 5 IETF meetings,
either in-person or online. In-person attendance is as determined by the record
keeping of the Secretariat. Online attendance is based on being a registered
person who logged in for at least one session of an IETF meeting.

Path 2:
The person has been a Working Group Chair or Secretary within the 3 years prior
to the day the call for NomCom volunteers is sent to the community.

Path 3:
The person has been a listed author or editor (on the front page) of at least
two IETF Stream RFCs within the last 5 years prior to the day the call for
NomCom volunteers is sent to the community. An Internet-Draft that has been
approved by the IESG and is in the RFC Editor queue counts the same as a
published RFC, with the relevant date being the date the draft was added to the
RFC Editor queue. For avoidance of doubt, the 5-year timer extends back to the
date 5 years before the date when the call for NomCom volunteers is sent to the
community.

# Available Data

TODO: This document should contain data about how the proposed criteria would
have affected eligibility for NomComs in the recent past.

# Security Considerations {#security-considerations}

The threat model associated with NomCom eligibility is that an organization or
group of organizations would attempt to obtain a majority of NomCom positions,
in order to select an IETF leadership in support of an agenda that might be
self-serving and against the interests of the community as a whole.

Note that {{!RFC8713}} lets the Chair decide the NomCom voting requirement, so a
simple majority may be inadequate. However, 7 of 10 forms a quorum, so at worst
seven NomCom members working together can almost certainly impose their will.

Whatever the merits of admitting remote attendees, it reduces the minimum cost
of creating a NomCom-eligible volunteer from three flights and ~5 days of travel
over the course of a year, to zero financial cost and the time required to log
in three times over the course of a year. Some organizations might not be
deterred in either case, while others might now find such an attack to be
feasible.

## A Surge of Volunteers

A large number of "legitimate" volunteers makes it quite difficult to control 6
of 10 NomCom slots. Setting aside limitations on the number of selections from
any organization, basic probability shows that to have even a 50% chance of
controlling 6 or more NomCom positions, an attacker needs somewhat roughly 60%
of the volunteer pool. For example, if there are 300 "legitimate" volunteers,
an attacker must produce 365 volunteers to exceed a 50% chance of NomCom
capture (see {{capture-math}}).

A sudden surge in the number of volunteers, particularly of people that no one
recognizes as a part of the community is an early-warning system for leadership
to further investigate.

While loosening eligibility criteria lowers the cost to an attacker of producing
eligible volunteers, it also increases the number of "legitimate" volunteers
that increases the difficulty and detectability of an attack.

## The Two-Per-Organization Limit

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

## One Year of Participation

Attendance at 3 meetings requires at least 1 year. Given the volume of
volunteers necessary to capture the process, an attack requires a surge in
attendees over the course of a year. IETF leadership SHOULD analyze unexplained
surges in attendance to look for signs of manipulating the eligibility
requirements (e.g. logging in to a single session and then immediately logging
out). In the event of malfeasance, the leadership would then have months to
adjust policy in response before the NomCom cycle begins.

# IANA Considerations

This document has no IANA actions.

--- back

# NomCom Capture Calculations {#capture-math}

{{security-considerations}} offers some mathematical results for the probability
of NomCom capture. This appendix shows the work.

Let (a ch b) mean the number of combinations of b items chosen from a population
of a items, or

(a ch b) = fact(a) / (fact(a-b) * fact(b))

## No per-organization limit

The first computation assumes there is no limit of two per organization,
or equivalently, no organization produces more than two volunteers.

Let L be the number of "legitimate" volunteers (i.e. those not allied with an
attacker" and A be the number of attacking volunteers. Then there are
((L+A) ch 10) ways to select a NomCom. The number of outcomes where attackers
capture the NomCom is

Sum(i=6..10)[(A ch i) * (L ch (10-i)]

and the probability of capture is therefore

Sum(i=6..10)[(A ch i) * (L ch (10-i)] / ((L+A) ch 10).

For L = 300, this probability crosses 50% at A = 365.

## Two per Organization

Assume that the population of L is drawn from L different organizations (this
assumption is unfavorable to the attacker). Assume also that there are three
conspiring organizations. Then no more than 6 members can be drawn from A.

Let B be the number of nominees per attacking organization, so that A = 3B.

The number of combinations to pick exactly N attackers, N <= 6, is

C(N) = (L ch (10-N)) *
    Sum(i=0:min(N,2))[(B ch i)<em>Sum(j=0..min(2, N-i))[(B ch j)</em>(B ch min(2, N-i-j))]]

And the probability of capture is

C(6) / Sum(i=0..6)[C(i)]

For L = 300, the A required to exceed a 50% probability of capture is 771.

# Change Log

> **RFC Editor's Note:** Please remove this section prior to
> publication of a final version of this document.

## Since draft-duke-elegy-rfc8989bis-00

* Editorial suggestions from Luc André Burdet

## Since draft-duke-gendispatch-rfc8989bis-00

* Matched normative section to RFC8989
* Added security considerations and appendix

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
