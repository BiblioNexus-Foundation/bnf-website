Title: Foundation Project
license: https://www.apache.org/licenses/LICENSE-2.0

  {# This template is pre-processed using Django syntax #}
  {# If you wish to use the '{#' markdown id introducer, please use:  #} 
  {# '{% templatetag opencomment %}' instead of '{#'  #}
  {# see /lib/path.pm for further details #}

<br>
The mission of the Apache Software Foundation (ASF) is to provide software 
for the public good.  We do this by providing services and support for many 
like-minded software project communities consisting of individuals who choose
to participate in ASF activities.

# What is the ASF? #

Established in 1999, the ASF is a US 501(c)(3) charitable organization, funded by 
individual donations and corporate sponsors.  Our all-volunteer board oversees 
more than 350 leading Open Source projects, including Apache HTTP Server -- 
the world's most popular Web server software. 

The ASF provides an established framework for 
intellectual property and financial contributions that simultaneously limits potential
legal exposure for our project committers. 
Through the ASF's meritocratic process known as "[The Apache Way](/theapacheway/)," more than 730 individual
Members and 7,000 Committers successfully collaborate to develop freely available 
enterprise-grade software, benefiting millions of users worldwide: thousands of software 
solutions are distributed under the Apache License; and the community actively participates
 in ASF mailing lists, mentoring initiatives, and ApacheCon, the Foundation's official user 
conference, trainings, and expo.

# How did the ASF and Apache&reg; projects grow? #

Formerly known as the Apache Group, the ASF was [incorporated](records/certificate.html) in 1999 as
a [membership-based][1], not-for-profit corporation in order to ensure that the
Apache projects continue to exist beyond the participation of individual
volunteers. Individuals who have demonstrated a commitment to collaborative
open-source software development, through sustained participation and
contributions within the Foundation's projects, are eligible for membership
in the ASF. An individual is awarded membership after nomination and
approval by a majority of the existing [ASF members](members.html). Thus,
the ASF is governed by the community it most directly serves -- the people
collaborating within its projects.  

# How are the ASF and Apache projects governed? #

The [ASF members](members.html) periodically elect a [Board of
Directors](board/) to manage the organizational affairs of the Foundation,
as accorded by the [ASF Bylaws](bylaws.html). The Board, in turn, appoints
a number of officers to oversee the day-to-day operations of the
Foundation. A number of [public records](records/) of our operation are
made available to the community. A more detailed explanation of [How the
ASF works](how-it-works.html) in terms of day to day operations is
available, and the [Apache Community Development project](http://community.apache.org/)'s
goal is to help newcomers learn more about the Apache Software Foundation.

Individual Apache projects are in turn 
governed directly by Project Management Committees (PMC) made up of 
individuals who have shown merit and leadership within those projects.
There are detailed descriptions of [ASF and project governance models](governance/).

# What is the role of ASF Members? #

As a Delaware membership corporation, [Apache Members](governance/members.html) are like shareholders in 
the legal corporation.  Members vote on the Board of Directors and may propose 
new Member candidates at [Annual Member's Meetings](governance/meetings).
Members have a [number of rights and responsibilities documented in our Governance guide](governance/members.html).

Note that Apache Members have a role with respect to the ASF as a corporation and 
their [role is defined in the ASF's bylaws][2]. This is separate from membership in 
our many Apache Project Management Committees, who are only responsible for 
development and community management in their individual project.

# Who runs the ASF? #

The membership of the ASF elects the 9 member board to run the foundation
and to set and ensure policy. The directors of the board are:

<!-- 
  N.B. Also: http://apache.org/foundation/board/
-->
#### Board members ####

|  |  |  |
|-----------|-------------|-------------|
|  {{ CI.board.0}} | {{ CI.board.1}} | {{ CI.board.2}} |
|  {{ CI.board.3}} | {{ CI.board.4}} | {{ CI.board.5}} | 
|  {{ CI.board.6}} | {{ CI.board.7}} | {{ CI.board.8}} |

<!--
The tables below are now updated automatically from committee-info.json
See lib/view.pm which sets up the data
-->

#### Officers ####

<br>The Board has appointed the following corporate officers of the ASF:

| Office    | Individual  |
|-----------|-------------|
| Board Chair |  {{ CI.boardchair.person }} |
| Vice Chair |  {{ CI.vicechair.person }} |
| President |  {{ CI.president.person }} |
| Exec. V.P |  {{ CI.execvp.person }} |
| Treasurer |  {{ CI.treasurer.person }} |
| Assistant Treasurer |  {{ CI.assistanttreasurer.person }} |
| Secretary |  {{ CI.secretary.person }} |
| Assistant Secretary |  {{ CI.assistantsecretary.person }} |
| V.P., [Legal Affairs](/legal/) |  {{ CI.legal.chair }} |
| Assistant V.P., [Legal Affairs](/legal/) |  {{ CI.assistantvplegalaffairs }} |
| V.P., [Security](/security/) |  {{ CI.security.chair }} |
| V.P., Data Privacy |  {{ CI.dataprivacy.chair }} |
| V.P., [W3C Relations](https://whimsy.apache.org/board/minutes/W3C_Relations.html) |  {{ CI.w3crelations.person }} |

<br>The President has appointed the following corporate officers of the ASF:

| Office    | Individual  |
|-----------|-------------|
| V.P., [Brand Management](marks/) |  {{ CI.brand.chair }} |
| V.P., [Conferences](https://events.apache.org/) |  {{ CI.concom.chair }} |
| V.P., [Diversity and Inclusion](http://diversity.apache.org/) |  {{ CI.diversity.chair }} |
| V.P., Fundraising |  {{ CI.fundraising.chair }} |
| V.P., [Infrastructure](/dev/) |  {{ CI.infrastructure.person }} |
| V.P., [Marketing and Publicity](/press/) |  {{ CI.marketingandpublicity.chair }} |
| V.P., [Travel Assistance](/travel/) |  {{ CI.tac.chair }} |
| [Infrastructure Administrator](/dev/) |  {{ CI.infrastructureadministrator.person }} |

<!--
Not currently appointed, see Dec 2020 board meeting minutes
| V.P., Finance |  {{ CI.finance.chair }} |
-->

<br>VP, Fundraising has appointed the following corporate officers of the ASF:

| Office    | Individual  |
|-----------|-------------|
| V.P., Sponsor Relations |  {{ CI.sponsorrelations.person }} |

#### PMC chairs ####

<br>The Board has appointed the following Vice Presidents to chair the PMCs 
of each Apache project:

| Office    | Individual  |
|-----------|-------------|  {% for p in pmcs %}
| V.P.,  {% if p.site %}[{% endif %}Apache {{ p.name }}{% if p.site %}]({{p.site}}){% endif %} | {{ p.chair }} | {% endfor %}

<br>The Foundation is a collaborative project of the ASF. Our goal is to build
and sustain the literal foundation upon which our open-source software
projects are based.


  [1]: https://www.apache.org/foundation/governance/
  [2]: https://www.apache.org/foundation/bylaws.html#meetings-of-members