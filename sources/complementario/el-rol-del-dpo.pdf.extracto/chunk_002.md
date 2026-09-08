# página 3 — de el-rol-del-dpo.pdf

ACCEPTED FOR IEEE SECURITY AND PRIVACY MAGAZINE
3
The Data Protection Ofﬁcer,
an ubiquitous role nobody really knows
Francesco Ciclosi, Fabio Massacci, Member, IEEE,
Abstract—Among all cybersecurity and privacy workers, the Data Protection Ofﬁcer (DPO) stands between those auditing a
company’s compliance and those acting as management advisors. A person that must be somehow versed in legal, management, and
cybersecurity technical skills. We describe how this role tackles socio-technical risks in everyday scenarios.
Index Terms—GDPR, data protection ofﬁcer (DPO), socio-technical system, qualitative studies, case studies
!
1
INTRODUCTION
T
HE recent application of Regulation (EU) 2016/679, best
known to the world as the General Data Protection
Regulation or GDPR, introduced the role of the data pro-
tection ofﬁcer (DPO). While DPOs have been a key enabler
of the GDPR [1], the role of this privacy worker is not a new
concept: in several EU Member States, its appointment was
already good practice for some years. Yet, the GDPR does
not formally describe the DPO job proﬁle, and most papers
discuss how to support a DPO with algorithms without
providing practical examples of what the DPO does.
For example, Diamantopoulou et al. [2] identify which
ISO 27001/2 controls need to be extended to meet GDPR
requirements and which of them the DPO is involved - but
why in some and not in others? Ryan et al. [3] explain how
their framework RegTech can be helpful to a DPO for check-
ing GDPR compliance - but when and for what concretely?
Chatzipolidis et al. [4] describe a readiness assessment tool
for GDPR’s compliance - but for solving social or technical
issues? Other articles discuss GDPR’s compliance topics as
if DPOs did not exist, from software engineering [5] to
socio-technical management processes [6], from the GDPR’s
cost among cybersecurity investments [7], to algorithms for
checking GDPR compliance itself [8].
Our purpose is to introduce this legally required orga-
nizational role — this ubiquitous privacy worker — to the
engineering community represented by Security & Privacy
readers through concrete examples of what problems DPOs
face, what they do, and what they may or must know.
While the literature is surprisingly silent about this, we
think that the knowledge of the everyday challenges that
DPOs have is the starting point for all subsequent research
activities. For example, if a researcher has no reference to
the daily activities of the key privacy worker in charge of
GDPR compliance, how can one design logic or a tool for
checking this privacy compliance or any privacy-by-design
technology with a practical impact? In summary, our key
•
F. Ciclosi (corresponding author) is with the University of Trento, Italy,
and on leave from the Italian Ministry of Economic Development.
E-mail: francesco.ciclosi@unitn.it
•
F. Massacci is with the University of Trento, Italy and Vrije Universiteit
Amsterdam, The Netherlands.
Manuscript accepted 02/11/2022
research question is:
•
Can we enucleate in a few representative scenarios the
concrete activities of a DPO?
The article focuses on the role of the DPO introduced by
the GDPR, but the insights are valuable for readers outside
the EU countries. The GDPR can apply to organizations
that carry out their activities in the EU and organizations
outside the EU that process the personal data of EU data
subjects. Further, in many countries worldwide, there is data
protection legislation in which a DPO role exists at some
level. The International Association of Privacy Professionals
(IAPP) lists the different roles in many countries worldwide
that share some characteristics with the DPO legally deﬁned
in the EU [9].
2
OUR METHODOLOGY
The insights described in this article are grounded in case
studies along Yin’s case study methodology [10, Ch.4] and
the suggestions [11] by Glaser, the founder of grounded
theory, to build core categories across ﬁeld observations
derived from the live experience.
First, we analyzed data protection laws and recommen-
dations of relevant authorities. Secondly, we analyzed the
seven functions of the DPO that the European Data Protec-
tion Supervisor (EDPS) identiﬁed in its paper on the role
of DPO in compliance with Regulation (EC) 45/2001. Then,
we looked at the summary of opinions of some supervisory
authorities (i.e., Bulgaria, Croatia, Italy, Poland, and Spain)
on the DPO’s activities involved with these functions (e.g.,
[12]) to have a perspective that was not restricted to a single
country.
To make this paper concrete as a use cases references,
we selected only sources of information for which there was
evidence that the activities carried out by DPO involve at
least one of these seven functions. The starting point for
the case study selection was the personal experience of
the ﬁrst author, who has been a DPO in the Italian public
administration for the past ﬁve years and is a member of
the Italian Association of DPOs.
To make the results of our study accessible, we looked
for some publicly available information (for example, court

