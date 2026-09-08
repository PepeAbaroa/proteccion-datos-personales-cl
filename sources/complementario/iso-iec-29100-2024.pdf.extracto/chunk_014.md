# página 15 — de iso-iec-29100-2024.pdf

ISO/IEC 29100:2024(en)
The substitution is considered pseudonymization, provided that:
a)	 the remaining attributes linked to the alias do not suffice to identify the PII principal to whom they 
relate; and
b)	 the alias assignment is such that it cannot be reversed by reasonable efforts of the privacy stakeholders 
other than those that performed them.
Pseudonymization retains linkability. Different data associated with the same pseudonym can be linked. 
The larger the set of data associated with a given pseudonym, the larger is the risk that property a) is 
violated. Moreover, the smaller the group of natural persons to which a set of pseudonymous data relates, the 
greater the likelihood of a PII principal being identifiable. Attributes contained directly in the information 
in question and attributes that can be easily linked to this information (e.g. by using a search engine or 
cross-referencing with other databases) should be taken into account when determining whether or not the 
information relates to an identifiable natural person.
Pseudonymization contrasts with anonymization. Anonymization processes also fulfil properties a) and b) 
above, but destroy linkability. During anonymization, identity information is either erased or substituted 
by aliases for which the assignment function or table is destroyed. Thus, anonymized data are no longer PII.
5.4.6	
Metadata
PII can be stored in an ICT system in such a way that it is not readily visible to the system user (i.e. to the PII 
principal). Examples include the PII principal’s name stored as metadata in the properties of a document, 
and comments or tracked changes stored as metadata in a word processing document. If the PII principal 
became aware of the existence of the PII or the processing of the PII for such a purpose, it is possible that he 
or she prefers that the PII is not processed in such a way or is shared publicly.
5.4.7	
Unsolicited PII
PII that was unsolicited by a PII controller or PII processor (i.e. unintentionally obtained) can also be 
stored in an ICT system. For example, a PII principal can potentially provide PII to a PII controller that was 
not requested or sought by the PII controller (e.g. additional PII provided in the context of an anonymous 
feedback form on a website). The risk of collecting unsolicited PII can be reduced by considering privacy 
safeguarding measures at the time of the design of the system (also referred to as the concept of “privacy by 
design”).
5.4.8	
Sensitive PII
Sensitivity extends to all PII from which sensitive PII can be derived. For instance, medical prescriptions can 
reveal detailed information about the PII principal’s health. Even if PII does not contain direct information 
about the PII principal’s sexual orientation or health, if it can be used to infer such information, the PII can 
be sensitive. For purposes of this document, PII shall be treated as sensitive PII where such inference and 
knowledge of the identity of the PII principal is reasonably possible.
NOTE 1	
In some jurisdictions, what constitutes sensitive PII is also defined explicitly in legislation. Examples include 
information revealing race, ethnic origin, religious or philosophical beliefs, political opinions, trade union membership, 
sexual lifestyle or orientation, and the physical or mental health of the PII principal. In other jurisdictions, sensitive 
PII can include information that can facilitate identity theft or otherwise result in significant financial harm to the 
natural person (e.g. credit card numbers, bank account information, or government-issued identifiers such as passport 
numbers, social security numbers or drivers’ license numbers), and information that can be used to determine the PII 
principal’s real time location.
The processing of sensitive PII requires special precautions. 
NOTE 2	
In some jurisdictions, the processing of sensitive PII can be prohibited by applicable law even with the PII 
principal’s opt-in consent. Some jurisdictions can require implementation of specific controls where certain types of 
sensitive PII are processed (e.g. a requirement to encrypt medical PII when transmitting it over a public network).
9
﻿
© ISO/IEC 2024 – All rights reserved

