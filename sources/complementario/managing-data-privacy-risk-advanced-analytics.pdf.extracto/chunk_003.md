# página 4 — de managing-data-privacy-risk-advanced-analytics.pdf

summer 2024 
sloanreview.mit.edu 
49
re-identification, depending on the type of algorithm 
used to generate the data, the data used to train the sys­
tem, fine-tuning of the parameters, and the attributes 
to which this approach is applied.² This marks a signif­
icant departure from the use of techniques such as data 
encryption, which provide great security at the expense 
of any data utility. National Bank’s cybersecurity and AI 
delivery teams worked together to develop a common 
understanding of both the issue and the fact that they 
would have to evaluate the potential for personal data 
to be de-anonymized against the degree of utility pro­
vided by synthetic data. This process gave the cyberse­
curity team insight into how re-identification techniques 
are now increasingly rooted in data science, while the AI 
team improved its understanding of the work that cyber­
security teams do to ensure the proper sharing and use 
of personal data.
STEP 2: Formalize and document data-privacy 
decision-making. Decisions regarding data privacy 
need to be clearly motivated and justifiable to regula­
tors in the eventuality of an audit — a scenario in which 
organizations must demonstrate that they have done 
everything they could to protect the privacy of customer 
data. That means they must be able to justify why they 
decided to use a given privacy preservation technique 
over another in a given situation.
Collaboration between cybersecurity and AI deliv­
ery teams at National Bank has led to ongoing efforts to 
quantify the impacts of various approaches on data pri­
vacy and data utility to better inform such decisions. (See 
“Modeling Data Privacy and Data Utility,” p. 50.) Teams 
simulate audits on data sets that have been protected 
using different data privacy approaches and parameters 
to calculate the probability of re-identification within 
those data sets. At the same time, they evaluate the util­
ity of those data sets based on the same approaches and 
parameters. For example, certain data anonymization 
techniques work by making quasi-identifiers more gen­
eral (such as substituting broader income brackets for 
actual income values). While that increases the privacy 
of customer data, it’s important not to compromise all of 
the nuances contained in the original data set that make 
Five Approaches to Preserving Data Privacy
Each approach to preserving the privacy of personal data will have an effect on the degree to which the data set 
remains useful for AI and analytics.  
APPROACH
DESCRIPTION
TYPICAL 
APPLICATION
TYPICAL USE CASE
SEEN BY 
REGULATORS AS
IMPACT ON DATA 
USABILITY
Masking
Hide attribute 
values in whole or in 
part with modified 
characters
Direct identifiers
Credit card numbers, 
email addresses
De-identification
High (loss of original 
information)
Tokenization
Replace sensitive 
attributes with 
nonsensitive 
substitutes (tokens)
Direct identifiers
Social Security 
numbers, bank 
account numbers
De-identification
High (regain 
usability through 
detokenization)
Data 
anonymization
Remove or modify 
(for example, swap 
or generalize) 
personal information 
to prevent 
re-identification
Quasi-identifiers
Health care records, 
location data
Anonymization
Moderate to low 
(original properties of 
the data can be closely 
approximated)
Data synthesis
Create new data that 
mimics the properties 
of the original data 
set without personal 
information
Quasi-identifiers
Data science research, 
data sharing
Anonymization
Low (original 
properties of the data 
can be preserved)
Data encryption
Convert data into 
nonreadable, 
unstructured text 
using an algorithm 
and an encryption key
Entire files
Secure storage and 
transmission
Anonymization
High (only possible 
through decryption)

