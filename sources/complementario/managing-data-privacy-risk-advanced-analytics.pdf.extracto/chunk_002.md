# página 3 — de managing-data-privacy-risk-advanced-analytics.pdf

48 
MIT Sloan Management Review 
summer 2024
Data Protection
A I  P R A C T I C E
Direct identifiers that enable almost immediate iden­
tification include name and Social Security number. 
Quasi-identifiers do not generally enable the identifi­
cation of a single individual on their own, but their 
uniqueness or their combination with other attrib­
utes may do so. For example, the combination of 
a person’s age and their address may enable their 
re-identification. Or consider a data set held by a 
bank’s fraud alert team on customers’ card transac­
tions. That data set contains both direct identifiers 
(such as the customer’s name) and quasi-identifiers 
(such as credit card transaction information).
In the context of analytics and AI, quasi-
identifiers are often highly valuable because they 
can help organizations uncover shared character­
istics and patterns that may help them better find 
or serve customers. But even seemingly innocuous 
quasi-identifiers, such as marital status, can be com­
bined with other pieces of publicly available informa­
tion to re-identify a specific person. Consequently, 
companies are already being challenged to go beyond 
protecting just personally identifiable information 
and consider how to protect quasi-identifiers as well.
Finding the optimal solutions to the privacy-
utility conundrum will also require a broader under­
standing of data privacy throughout the organization, 
beyond IT and cybersecurity functions. Managers 
seeking to better understand the scope of options 
available in balancing data privacy with utility should 
be broadly familiar with the array of approaches 
available. Each has its own advantages and disad­
vantages, with varying implications for data privacy 
and data utility. (See “Five Approaches to Preserving 
Data Privacy.”)
Privacy Versus Utility Trade-off
To understand how organizations are confronting the 
complex matter of protecting personal data in their 
care while also leveraging it for analytics and AI, we’ll 
look at initiatives recently undertaken at National 
Bank of Canada. (Note that Julien oversees artificial 
intelligence at the bank; Gregory and Patrick have 
studied the organization’s practices.) Founded in 1859, 
National Bank is one of the largest financial institu­
tions in Canada. Like its competitors, it must com­
ply with stringent federal and provincial regulatory 
requirements. Customers trust that National Bank 
manages their money and the wealth of personal 
data they share with the bank (when they execute 
transactions or apply for loans, for instance) with the 
utmost care.
As a financial institution, National Bank 
considers customer trust to be its greatest asset, and 
so it has built a culture in which protecting the pri­
vacy of its customers’ data is a core value. In addi­
tion to driving significant efforts and investment in 
cybersecurity and organizationwide training, it has 
also increasingly prioritized analytics and AI. Here, 
new techniques and approaches increase the poten­
tial to leverage personal data to improve services for 
customers. This increasing use of AI techniques also 
requires heightened protection efforts, given that 
new approaches can also be used to compromise the 
privacy of personal data.¹
Data protection had traditionally been treated 
as a security matter that was the responsibility of 
cybersecurity experts at National Bank. Under this 
logic, personal data protection would be guaran­
teed using tried and proven techniques. However, 
some of those techniques may not readily achieve 
the required balance between data privacy and data 
utility. For example, cybersecurity teams can encrypt 
entire files, but doing so prevents data scientists 
from being able to use the data contained within 
those files. Using a more granular approach, direct 
identifiers could be protected using tokenization 
(to achieve de-identification), leaving the data sci­
ence team able to leverage quasi-identifiers, but this 
does not address the risk of re-identification asso­
ciated with those quasi-identifiers. To simultane­
ously satisfy requirements for both data privacy and 
data utility, teams must find a common ground that 
allows them to move beyond techniques that favor an 
either/or approach. In the case of National Bank, we 
have identified three important steps that contribute 
to its ability to achieve this objective.
STEP 1: Bridge the gap between IT and data 
science. In most organizations, cybersecurity and 
AI/data science teams don’t work together. Each has 
its specialty, and trying to put data to work requires 
collaboration between experts who tend to work in 
silos. National Bank realized that this division led 
to inefficiencies, frustration, and an overall lack of 
mutual understanding of teams’ respective priori­
ties and concerns, and it set out to mitigate the issue. 
Managers fostered close collaboration between 
cybersecurity experts and AI delivery team mem­
bers — including those in roles such as AI architect, 
data scientist, machine learning engineer, and data 
engineer — to evolve their competencies and skill 
sets in each other’s domain of expertise.
One illustration of the importance of building 
this mutual understanding is the example of using 
synthetic data, where there may be a probability of 

