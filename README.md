# crmaaa

CRM Art and Architectural
Argumentation Conceptual Model
Specification
Document Type : Specification
Author : George Bruseker (Takin.solutions)
Version : 0.9
Filename : CRM_AAA_Spec_v.0.9.pdf
Report Date : 2/2/21
Project Reference : Sustainable Art and Architectural Data Reuse in Teaching and Research
Table of Contents
Table of Contents 1
Introduction 2
Hierarchical Presentation 4
Class Hierarchy 4
Property Hierarchy 6
Classes 8
Properties 25
1
Introduction
This document represents the formal specification for an unofficial formal extension of the
CIDOC CRM designed for application in the area of art and architectural historical research. The
scope of this extension is to support art and architectural research in the sense of the study of
primary and secondary documents for the derivation, manually and programmatically, of
historically contextual facts that can be used to support reflection and structured argumentation.
The core expressivity that this extension adds is the ability to accurately express historically
bound, contextual social facts relative to the agents holding those beliefs and the temporal
period for which those beliefs were valid. The extension enables this expressivity by introducing
the notions of institutional fact and speech act as core modelling concepts. Institutional facts are
collective beliefs held by groups for period of time about the world. Such collective beliefs while
subjectively grounded are epistemically objective for the community over which they hold sway.
Introducing the notion of institutional fact allows for a specialization of the core CRM to be able
to express these social realities (expressed in simple, aoristic binary properties in the core
CRM) in their full social complexity as temporally and socially bound beliefs. The concomitant
core notion introduced in this extension is the idea of Speech Act in the Austinian and Serlean
sense. A speech act is a kind of intentional event (E7 Activity of CRM base) in which agents
purposefully apply a rule and perform a set ritual in order to bring about a new social state or
institutional fact. Introducing the notion of speech act provides both a high level ontological
category and set of relations for describing the kinds of events which are the cause of
institutional facts as well as providing a starting point for the analysis of the non truth
propositional use of information objects. In speech acts, information objects (e.g. phrases and
formulae) are deployed not to convey states of the world but to generate states of the world.
The subject of historical investigation is not simply the bare facts available to an empirical
analysis of the physical world but involves an investigation of the social activities which
generated contexts of understanding and belief that may differ significantly over times and
peoples. Materializing the social relations represented in CRM base as institutional facts gives
them a better ontological position and offer a better epistemological approach to their study by
recognizing social, negotiated facts as objective realities in themselves and treating them as first
class entities of study. This involves a departure from the aims of CRM base which is guided by
an information integration functionality which favours the representation of the latest state of
knowledge in a presentist perspective. In the study of the history of art and architecture it is in
no small part the different non-coinciding facts held or supported by different entities over
different times which are of interest. The materialization of institutional facts supports the
information management functionality which guides this informal extension of the CIDOC CRM
which aims to support historians in representing the positive knowledge they can gather from
primary and secondary evidence of both past simple and institutional facts for the purposes of
proposing hypotheses and analyses of texts, authors, periods, works and so on. In this regard,
CRMAnA also provides an initial limited set of classes for describing traditional and digital
methods of deriving facts from texts, in order to support the linking of contemporary research
processes as provenance nodes for the different data points of simple and institutional facts
which they generate in the course of their research.
2
This unofficial extension of the CIDOC CRM is formulated in relation to:
CIDOC CRM v.7.01
CIDOC CRM Inf v.0.10.1
CIDOC CRM Sci v. 1.2.8
The specification consists of the a set of declarations for formalized classes and properties that
extend the CIDOC CRM and the above official extensions.
Adopting the conventions of the CIDOC CRM each class and property have been given an
identifier in addition to their names. The naming convention adopted for this extension is:
ZE = class
ZP = property
The choice of these names was arbitrary, making a conceptual connection with the official CRM
representation while clearly distinguishing the new classes and properties from those of either
CMR base or other extensions.
3
Hierarchical Presentation
Class Hierarchy
E1 CRM Entity
E2 Temporal Entity
ZE1 Institutional Fact
ZE2 Appellative Status
ZE3 Contact Status
ZE4 Classificatory Status
ZE5 Function Status
ZE6 Social Status
ZE7 Custodial Status
ZE8 Ownership Status
ZE9 Residential Status
ZE10 Family Status
ZE11 Membership Status
ZE12 Referential Status
ZE14 Similarity Status
ZE15 Set Status
E4 Period
E5 Event
E63 Beginning of Existence
E65 Creation
E7 Activity
I1 Argumentation
ZE18 Critical Reading
E65 Creation
D7 Digital Machine Event
ZE17 Digital Reading
E11 Modification
D7 Digital Machine Event
ZE17 Digital Reading
ZE16 Utterance Event
ZE13 Speech Act
ZE17 Digital Reading
ZE18 Critical Reading
E13 Attribute Assignment
ZE19 Naming
E15 Identifier Assignment
E17 Type Assignment
E8 Acquisition
4
ZE20 Declarative Acquisition
E10 Transfer of Custody
ZE21 Declarative Transfer of Custody
E85 Joining
ZE22 Declarative Joining
E86 Leaving
ZE23 Declarative Leaving
E77 Persistent Item
E70 Thing
E71 Human-Made Thing
E28 Conceptual Object
ZE24 Notional Set
5
Property Hierarchy
ZP1 has intentional subject [D: ZE1, R: E1]
ZP5 has appellative subject [D:ZE2, R:E1]
ZP8 has contact subject [D:ZE3, R:E39]
ZP11 has classificatory subject [D:ZE4, R:E1]
ZP14 has functional subject [D:ZE5, R:E72]
ZP17 has social subject [D:ZE6, R:E39]
ZP20 has custodial subject [D:ZE7, R:E19]
ZP23 has ownership subject [D:ZE8, R:E72]
ZP26 has residence subject [D:ZE9, R:E39]
ZP29 has family subject [D:ZE10, R:E21]
ZP32 has membership subject [D:ZE11, R:E39]
ZP35 has referential subject [D:ZE11, R:E89]
ZP2 ascribes intentional target [D: ZE1, R:E1]
ZP6 ascribes appellation [D: ZE2, R:E41]
ZP9 ascribes contact point [D:ZE3,R: E41]
ZP12 ascribes classification [D:ZE4, R:E55]
ZP15 ascribes function [D:ZE5, R:E55]
ZP18 ascribes social status [D:ZE6, R:E55]
ZP21 ascribes custodian [D:ZE7, R:E39]
ZP24 ascribes owner [D:ZE8, R:E39]
ZP27 ascribes residence place [D:ZE9, R:E53]
ZP30 ascribes relative [D:ZE10, R:E21]
ZP33 ascribes group [D:ZE11, R:E74]
ZP36 ascribes referent [D:ZE12, R:E1]
ZP3 ascribes intentional relation [D: ZE1, R:E55]
ZP7 ascribes appellative relation [D: ZE1, R:E55]
ZP10 ascribes contact point relation [D: ZE3, R:E55]
ZP13 ascribes classification relation [D: ZE4, R:E55]
ZP16 ascribes functional relation [D: ZE5, R:E55]
ZP19 ascribes social status relation [D: ZE6, R:E55]
ZP22 ascribes custodial relation [D: ZE7, R:E55]
ZP25 ascribes ownership relation [D: ZE8, R:E55]
ZP28 ascribes residence relation [D: ZE9, R:E55]
ZP31 ascribes family relation [D: ZE10, R:E55]
ZP34 ascribes group relation [D: ZE11, R:E55]
ZP37 ascribes referential relation [D: ZE12, R:E55]
ZP38 ascribes referential mode [D: ZE12, R:E55]
ZP4 holds for [D: ZE1, R:E74]
P16 used specific object
ZP41 utters [D: ZE13, R:E33]
P33 used specific technique
ZP39 invokes [D: ZE13, R:E29]
6
ZP40 performs [D: ZE13, R:E29]
O13 triggers
ZP42 intentionally initiates [D: ZE13, R:ZE1]
7
Classes
8
# ZE1
Label Institutional Fact
Superclass of
Subclass of E2 Temporal Entity
Scope Note An instance of institutional fact is an ascription of a status function to an
object by a community. The institutional fact is a concretization of a
collective intentionality of the community in question towards a certain
object over a certain period. An instance of institutional fact is
recognizable to a competent speaker/member of a symbolic community
(native or learner with sufficient progress, e.g. anthropologist). An
instance of institutional fact may not be perceived through a single sense
impression but through multiple experiences and implicit reasonings
(e.g.: the behaviour of a child to an elder, and linguistic evidence and
interview), yet typically such intermediate observations and inferences
are not necessarily recorded or accessible. The historical statement is
typically the assertion of the institutional fact, that such and such a fact
was the case, and in force, at some time. The epistemic veridicality of the
stated /reference instance of institutional fact is always open to
contestation. The means of contestation involve analyzing the sources
which support it. Instances of institutional fact come into existence based
on conventions establishing the conditions under which they come into
effect. Typically, an instance of institutional fact will come into existence
either because of the performance of its stipulated, initiating speech act
(e.g.: state of being married via marriage) or as a result of events fulfilling
existing norm prescriptions in the community (e.g.: state of being father
as result of birth of child of sister). An institutional fact comes to be
through the agreed fiat of a community. It typically ceases to exist either
because of a stipulated, nullifying speech act (e.g. divorce proceeding),
because a community ceases to support the effective rule supporting its
declaration (e.g.: ownership of people) or force majeure (e.g.: object
ascribed function/status or community perceiving status is eliminated).
Example
Properties ZP1 has intentional subject
ZP2 ascribes intentional target
ZP3 ascribes intentional relation
ZP4 holds for
9
# ZE2
Label Appellative Status
Superclass of ZE3 Contact Status
Subclass of ZE1 Institutional Fact
Scope Note An instance of appellative status is the collective ascription of an
appellation to an object by a community. The substance of the
appellative status is the communal commitment to the naming of the
object in question with a designated appellation, under a designated
modality. Instances of appellative status are recognizable through
evidence of community members adopting the intentional stance of
so-naming towards the object in question, as observable from direct
witnesses, through the reports of competent observers or through
evidence of a declarative act (Naming) initiating this status. Examples of
such evidence include, several individuals so naming a thing, a witness
declaring that a thing is ‘so named, by us’ or through documents
reporting this fact. Instances of appellative status may come to be
through a formal process such as a declarative act of naming, or may
have arisen through habit, fiat or be of unknown origin. Instances of
appellative status may end either though a formal process, such as a
new declarative act of naming, the formal stripping of a name, or may
simply fade out of use, be eliminated by fiat or be of unknown reason.
Example The appellative status of the Polity of Macedonia (E74) as ”is identified
by” the Former Yugoslavian Republic of Macedonia (E41) 1991-2019 by
the Greek Polity (E74)
https://en.wikipedia.org/wiki/North_Macedonia#Names_and_etymology
Properties ZP5 has appellative subject
ZP6 ascribes appellation
ZP7 ascribes appellative relation
# ZE3
Label Contact Status
Superclass of
Subclass of ZE2 Appellative Status
Scope Note An instance of contact status is the collective ascription of a contact point
to an actor by a community. The substance of the contact status is the
10
communal commitment to the addressing of messages to the actor in
question according to a designated contact point appellation, using the
implied message exchanging method. Instances of contact status are
recognizable through evidence of community members adopting the
intentional stance of so-addressing messages to the actor in question, as
observable from direct witnesses, through the reports of competent
observers or through evidence of a declarative act (Identifier Assignment)
initiating this status. Examples of such evidence include, several
individuals so addressing messages to an actor via this contact point
appellation, a witness declaring that an actor can so be reached by us or
through documents reporting this fact. Instances of contact status may
come to be through a formal process such as a declarative act of
identifier assignment, or may have arisen through habit, fiat or be of
unknown origin. Instances of contact status may end either though a
formal process, such as a new declarative act of identifier assignment,
through formal assignment, or may simply fade out of use, be eliminated
by fiat or for unknown reasons.
Example The contact point status of George Bruseker as “has contact point”
Leoforos Minoos 4, Heraklion 2016-2019 held by National Bank of
Greece (E74)
Properties ZP8 has contact subject
ZP9 ascribes contact point
ZP10 ascribes contact point relation
# ZE4
Label Classificatory Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of classificatory status is the collective ascription of a type to
an object by a community. The substance of the classificatory status is
the communal commitment to the classification of the object in question
according to the designated type. Instances of classificatory status are
recognizable through evidence of community members adopting the
intentional stance of so-classifying the object in question, as observable
from direct witnesses, through the reports of competent observers or
through evidence of a declarative act (Type Assignment) initiating this
status. Instances of classificatory status may come to be through a
11
formal process such as a declarative act of classification (type
assignment), or may have arisen through habit, fiat or be of unknown
origin. Instances of classificatory status may end either though a formal
process, such as a new declarative act of classification, be officially
declassified, or may simply fade out of use, be eliminated by fiat or be of
unknown reason.
Example The classificatory status of the assemblage of apatosaurus and
camarasaurus remains (E19) as ‘has type’ Brontosaurus excelsus (E55)
1905 -? held by American Museum of Natural History (E74)
Properties ZP11 has classificatory subject
ZP12 ascribes classification
ZP13 ascribes classificatory relation
# ZE5
Label Function Status
Superclass of
Subclass of ZE4 Classificatory Status
Scope Note An instance of functional status is the collective ascription of an operative
functionality to an object by a community. The substance of the function
status is the communal commitment to relating to and using the object in
question according to a designated function. Instances of function status
are recognizable through evidence of community members adopting the
intentional stance of so-using or relating to the object in question, as
observable from direct witnesses, through the reports of competent
observers or through evidence of a declarative act (Type Assignment)
initiating this status. Instances of function status may come to be through
a formal process such as a declarative act of classification (type
assignment), or may have arisen through habit, fiat or be of unknown
origin. Instances of function status may end either though a formal
process, such as a new declarative act of classification.
Example The function status of St Joe’s Cathedral (E22) as ‘has type’ minor
basilica (E55) 1984 - Present held by the Catholic Church (E74)
12
Properties ZP14 has functional subject
ZP15 ascribes function
ZP16 ascribes functional relation
# ZE6
Label Social Status
Superclass of
Subclass of ZE4 Classificatory Status
Scope Note An instance of social status is the collective ascription of a social function
to an actor by a community. The substance of the social status is the
communal commitment to relating to and action toward the actor in
question according to the designated status. Instances of social status
are recognizable through evidence of community members adopting the
intentional stance of so relating or acting toward the actor in question, as
observable from direct witnesses, through the reports of competent
observers or through evidence of a declarative act (Type Assignment)
initiating this status. Instances of social status may come to be through a
formal process such as a declarative act of assignment (type
assignment), or may have arisen through habit, fiat or be of unknown
origin. Instances of social status may end either though a formal process,
such as a new declarative act of classification.
Example The social status of Friedrich Hegel (E21) as ‘has type’ Privatdozent
(E55) 1801-1805 held by Jena University (E74)
https://en.wikipedia.org/wiki/Georg_Wilhelm_Friedrich_Hegel#Career_ye
ars
Properties ZP17 has social subject
ZP18 ascribes social status
ZP19 ascribes social status relation
# ZE7
Label Custodial Status
Superclass of
13
Subclass of ZE1 Institutional Fact
Scope Note An instance of custodial status is the collective ascription of a relationship
of custodianship over an object by some actor by a community. The
substance of the custodial status is the communal commitment to the
recognition of the relationship of custodianship over the designated
object by the actor in question. Instances of custodial status are
recognizable through evidence of community members adopting the
intentional stance of so-recognizing this status, as observable from direct
witnesses, through the reports of competent observers or through
evidence of a declarative act (Declarative Transfer of Custody) initiating
this status. Instances of classificatory status may come to be through a
formal process such as a declarative act of classification (Declarative
transfer of custody), or may have arisen through habit, fiat or be of
unknown origin. Instances of custodial status may end either though a
formal process, such as a new declarative act of legal transfer of
custody, or may simply fade out of use, be eliminated by fiat or be of
unknown reason.
Example The custodial status of the G'psgolox totem pole (E22) as ‘ has present
holder’ the Swedish National Museum of Ethnography (E74) 1929-2006
by the Swedish Polity (E74)
https://en.wikipedia.org/wiki/G%27psgolox_totem_pole#:~:text=G'psgolo
x%20totem%20pole%20is,gift%20to%20the%20Haisla%20people.
Properties ZP20 has custodial subject
ZP21 ascribes custodian
ZP22 ascribes custodial relation
# ZE8
Label Ownership Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of ownership status is the collective ascription of a
relationship of legal possession over an object by some actor by a
community. The substance of the ownership status is the communal
14
commitment to the recognition of the relationship of possession over the
designated object by the actor in question. Instances of ownership status
are recognizable through evidence of community members adopting the
intentional stance of so-recognizing this status, as observable from direct
witnesses, through the reports of competent observers or through
evidence of a declarative act (Declarative Acquisition) initiating this
status. Instances of ownership status may come to be through a formal
process such as a declarative act of taking ownership (declarative
acquisition), or may have arisen through habit, fiat or be of unknown
origin. Instances of ownership status may end either though a formal
process, such as a new declarative act of declarative acquisition, or may
simply fade out of use, be eliminated by fiat or be of unknown reason.
Example The ownership status of the Euphronios Krater (E22) as ‘has present
owner’ the Metropolitan Museum of Art (E74) from 1972-2006 held by the
American Polity (E74)
https://en.wikipedia.org/wiki/Euphronios_Krater
Properties ZP23 has ownership subject
ZP24 ascribes owner
ZP25 ascribes ownership relation
# ZE9
Label Residential Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of residential status is the collective ascription to an actor of
a place of residence by a community. The substance of the residential
status is the communal commitment to the recognition and use of the
designated place with regards to the residence of the designated actor.
Instances of residential status are recognizable through evidence of
community members adopting the intentional stance of so-recognizing
this status, as observable from direct witnesses, through the reports of
15
competent observers or through evidence of a declarative act (Residence
Declaration) initiating this status. Instances of residence status may
come to be through a formal process such as a declarative act of taking
ownership (declarative acquisition), or may have arisen through habit, fiat
or be of unknown origin. Instances of residence status may end either
though a formal process, such as a new declarative act of declarative
acquisition, or may simply fade out of use, be eliminated by fiat or be of
unknown reason.
Example The residential status of the Prime Minister Role of Canada as ‘has
former or current residence’ 24 Sussex Drive (E53) 1951 - Present held
by the Canadian Polity (E74)
The residential status of Justin Trudeau as ‘has former or current
residence’ Rideau Hall (E74) 2015 - Present held by the Canadian Polity
(E74)
Properties ZP26 has residence subject
ZP27 ascribes residence place
ZP28 ascribes residence relation
# ZE10
Label Family Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of family status is the collective ascription of a familial
relationship between one actor and another by a community. The
substance of the family status is the communal recognition of the familial
connection between the two actors in question. Instances of family status
are recognizable through evidence of community members adopting the
intentional stance and behaviour indicated as proper to this relation, as
observable from direct witnesses, through the reports of competent
observers or through evidence of a declarative act (??? adoption)
initiating this status. Instances of family status may come to be simply
16
through birth in a certain community or may require that a formal process
such as a right of passage has been undertaken. Instances of family
status may end either though a formal process such as a renunciation or
through death.
Example
Properties ZP29 has family subject
ZP30 ascribes relative
ZP31 ascribes family relation
# ZE11
Label Membership Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of membership status is the collective ascription of a
membership relationship between an actor and some group by a
community. The substance of the membership status is the communal
recognition of the ascribed membership relation between the actor and
the group in question. Instances of membership status are recognizable
through evidence of community members adopting the intentional stance
and behaviour indicated as proper to this relation, as observable from
direct witnesses, through the reports of competent observers or through
evidence of a declarative act (Joining) initiating this status. Instances of
membership status may come to be through a formal process such as a
declarative act of declarative joining or may have arisen through habit,
fiat or be of unknown origin. Instances of membership status may end
either though a formal process (declarative leaving), or may simply fade
out, be eliminated by fiat or for unknown reasons.
Example
Properties ZP32 has membership subject
17
ZP33 ascribes group
ZP34 ascribes group relation
# ZE12
Label Referential Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of referential status is the collective ascription of a referential
relationship between a propositional object and some entity by a
community. The substance of the referential status is the communal
recognition of the ascribed referential relation between the propositional
object and the entity in question. Instances of referential status are
recognizable through evidence of community members adopting the
intentional stance and behaviour indicated as properly holding between
the propositional object and the object it is taken to refer to in the manner
it is meant to refer, as observable from direct witnesses, through the
reports of competent observers or through evidence of a declarative act
(???artistic genius, the beginning of civilization???) initiating this status.
Instances of referential status may come to be through a formal process
such as a declarative act or may have arisen through habit, fiat or be of
unknown origin. Instances of referential status may end either though a
formal process, or may simply fade out, be eliminated by fiat or for
unknown reasons.
Example
Properties ZP35 has referential subject
ZP36 ascribes referent
ZP37 ascribes referential relation
ZP38 ascribes referential mode
# ZE13
18
Label Speech Act
Superclass of
Subclass of E7 Activity
Scope Note An instance of speech act comprises an intentional activity engaged in
by a set of actors to create a new institutional fact within a community.
Speech acts are carried out through invoking a social rule and performing
a prescribed set of actions often including the locution of set formulae.
Correct execution of the speech act as specified by the rule results in the
existence of new institutional facts. The substance of speech act is ritual
action by a group. An instance of speech act begins when the intended
ritual proceeding as specified by the rule invoked is initiated. The
instance of speech act ends when the required set of actions specified
for the action in question are executed or it is abandoned.
Example
Properties ZP39 invokes [D: ZE13, R:E29]
ZP40 performs [D: ZE13, R:E29]
ZP41 utters [D: ZE13, R:E33]
ZP42 intentionally initiates [D: ZE13, R:ZE1]
ZP52 intentionally terminates [D: ZE13, R:ZE1]
ZP53 initiates for [D:ZE13, R:E74]
# ZE14
Label Similarity Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of similarity status is the collective ascription of a similarity
relationship between any two objects by a community. The substance of
the similarity status is the communal recognition of the ascribed similarity
relation between the two entities in question. Instances of similarity status
are recognizable through evidence of community members adopting the
intentional stance and behaviour indicated by the kind of similarity
believed to hold between the two referenced entities, as observable from
19
direct witnesses, through the reports of competent observers or through
evidence of a declarative act initiating this status. Instances of similarity
status may come to be through a formal process such as a scholarly
declarative act or may have arisen through habit, fiat or be of unknown
origin. Instances of similarity status may end either though a formal
process (official disproof), or may simply fade out, be eliminated by fiat or
for unknown reasons.
Example
Properties ZP43 has similarity subject
ZP44 has similarity target
ZP45 ascribes similarity relation
ZP46 ascribes similarity relation mode
# ZE15
Label Set Status
Superclass of
Subclass of ZE1 Institutional Fact
Scope Note An instance of set status is the collective ascription of some relationship
of belonging between some entity and a notional set by a community.
The substance of the set status is the communal recognition of the
ascribed belonging between the subject entity and the set in question.
Instances of set status are recognizable through evidence of community
members adopting the intentional stance and behaviour indicated as
proper to this set belonging relation, as observable from direct witnesses,
through the reports of competent observers or through evidence of a
declarative act initiating this status. Instances of set status may come to
be through a formal process or may have arisen through habit, fiat or be
of unknown origin. Instances of membership status may end either
though a formal process, or may simply fade out, be eliminated by fiat or
for unknown reasons.
Example
20
Properties ZP47 has set belonging subject
ZP48 ascribes set
ZP49 ascribes set belonging relation
ZP50 ascribes set belonging mode
# ZE16
Label Utterance Event
Superclass of
Subclass of E7 Activity
Scope Note An instance of this class is an act by an agent purposefully using a
determined lectical information phrase within the purposes of oratorical
and argumentative context towards a certain effect. Instances of
utterance event document known historical cases of the deployment of a
text by an actor in a context towards some goal. Instances of utterance
event can also be detected /interpreted within a text when the research
goal and purpose is to determine intention and function of textual
passages in their historical context.
Example
Properties ZP50 uttered
# ZE17
Label Digital Reading
Superclass of
Subclass of D7 Digital Machine Event, ZE13 Speech Act
Scope Note An instance of digital reading is a digital processing event guided by set
instructions or parameters for returning an output result set of
identifications that makes propositions about the content of an input
dataset. Digital reading is a computational process guided by a
parametrized hypothesis resulting in a new propositional dataset for
scientific consideration. The propositional information generated by the
21
digital reading process should be considered as provisional knowledge
posited under a hypothesis. Typically propositions generated by the
digital reading will become the subject of further scholarly research.
Example
Properties
# ZE18
Label Critical Reading
Superclass of
Subclass of I1 Argumentation, ZE13 Speech Act
Scope Note An instance of critical reading is a process of analysis undertaken by a
scholar to derive analytical facts from a specific information resource.
Critical reading engages the background knowledge of the scholar and
their interpretive horizon in order to support them in actively read the
research object to derive factual, historically contextualized information
regarding the object. This process can take as input previous scholarly
documentation or outputs of digital reading events.
Example
Properties
# ZE19
Label Naming
Superclass of
Subclass of E13 Attribute Assignment
22
Scope Note Instances of naming are comprised of an act which officially confers a
name to some object under a specific procedure. The result of the
instance of naming is the coming to be of a collective acceptance of a
name for some object in some mode for some time. The details of this
institutional fact are documented in the resultant instance of Appellative
Status.
Example
Properties
# ZE20
Label Declarative Acquisition
Superclass of
Subclass of ZE13 Speech Act, E8 Acquisition
Scope Note Instances of this class comprise official acquisition events undertaken
following formal procedures within a social grouping leading to formal
ownership status over an object relative to the participating parties. A
successful act of declarative acquisition leads to the generation of an
instance of ownership status, the institutional fact that thereafter
mediates the social relation to this object until it has been abrogated.
Example
Properties
# ZE21
Label Declarative Transfer of Custody
Superclass of
Subclass of ZE13 Speech Act, E10 Transfer of Custody
23
Scope Note Instances of this class comprise official transfer of custody events
undertaken following formal procedures within a social grouping leading
to formal change in the custody status over an object relative to the
participating parties. A successful act of declarative transfer of custody
leads to the generation of an instance of custody status, the institutional
fact that thereafter mediates the social relation to this object until it has
been abrogated.
Example
Properties
# ZE22
Label Declarative Joining
Superclass of
Subclass of ZE13 Speech Act, E85 Joining
Scope Note Instances of this class comprise official joining events undertaken
following formal procedures within a social grouping leading to formal
change in the membership status of an actor relative to a group for the
participating parties. A successful act of declarative joining leads to the
generation of an instance of membership status, the institutional fact that
thereafter mediates the social relation to this object until it has been
abrogated.
Example
Properties
# ZE23
Label Declarative Leaving
Superclass of
24
Subclass of ZE13 Speech Act, E86 Leaving
Scope Note Instances of this class comprise official leaving events undertaken
following formal procedures within a social grouping leading to formal
change in the membership status of an actor relative to a group for the
participating parties. A successful act of leaving leads to the generation
of an instance of membership status, the institutional fact that thereafter
mediates the social relation to this object until it has been abrogated.
Example
Properties
# ZE24
Label Notional Set
Superclass of
Subclass of E28 Conceptual Object
Scope Note Instances of this class comprise notional sets of objects which have been
classified together for one reason or another. A notional set comes to be
when it is asserted or otherwise declared. It gains or loses members
according to the particular rules guiding its maintenance. Typically sets
serve a functional purpose such as the grouping of some objects
according to an ad hoc, context particular, or a context categorical
criterion.
See also Linked.Art:Set
Example
Properties ZP51 has former or current set member
Properties
25
# ZP1
Label has intentional subject
Super property of ZP5 has appellative subject [D:ZE2, R:E1]
ZP11 has classificatory subject [D:ZE4, R:E1]
ZP20 has custodial subject [D:ZE7, R:E19]
ZP23 has ownership subject [D:ZE8, R:E72]
ZP26 has residence subject [D:ZE9, R:E39]
ZP29 has family subject [D:ZE10, R:E21]
ZP32 has membership subject [D:ZE11, R:E39]
ZP35 has referential subject [D:ZE11, R:E89]
Sub property of
Domain ZE1 Institutional Fact
Range E1 CRM Entity
Scope Note This property is used to connect an instance of institutional fact to an
entity with which it is concerned. The intentional subject indicated by
this property is the object about which the institutional fact holds for
the group committed to this institutional reality.
Example
# ZP2
Label ascribes intentional target
Super property of ZP6 ascribes appellation [D: ZE2, R:E41]
ZP12 ascribes classification [D:ZE4, R:E55]
ZP21 ascribes custodian [D:ZE7, R:E39]
ZP24 ascribes owner [D:ZE8, R:E39]
ZP27 ascribes residence place [D:ZE9, R:E53]
ZP30 ascribes relative [D:ZE10, R:E21]
ZP33 ascribes group [D:ZE11, R:E74]
ZP36 ascribes referent [D:ZE12, R:E1]
Sub property of
Domain ZE1 Institutional Fact
Range E1 CRM Entity
26
Scope Note This property is used to indicate the entity which an instance of
institutional fact ascribes to its subject. The intentional target
indicated by this property is the object which the institutional fact
establishes as holding of its subject for the group committed to this
institutional reality. The manner of its holding is indicated by the
intentional relation.
Example
# ZP3
Label Ascribes intentional relation
Super property of ZP7 ascribes appellative relation [D: ZE1, R:E55]
ZP13 ascribes classification relation [D: ZE4, R:E55]
ZP22 ascribes custodial relation [D: ZE7, R:E55]
ZP25 ascribes ownership relation [D: ZE8, R:E55]
ZP28 ascribes residence relation [D: ZE9, R:E55]
ZP31 ascribes family relation [D: ZE10, R:E55]
ZP34 ascribes group relation [D: ZE11, R:E55]
ZP37 ascribes referential relation [D: ZE12, R:E55]
ZP38 ascribes referential mode [D: ZE12, R:E55]
Sub property of
Domain ZE1 Institutional Fact
Range E55 Type
Scope Note This property is used to indicate the relationship which an instance of
institutional fact takes to hold between its subject and its object. The
intentional relation indicated by this property is the kind of relationship
which the institutional fact establishes as holding between them for
the group committed to this institutional reality.
Example
# ZP4
Label holds for
Super property of
27
Sub property of
Domain ZE1 Institutional Fact
Range E39 Actor
Scope Note This property is used to indicate the community or group for whom an
instance of institutional fact holds. Institutional facts have identity only
relative to some group for whom they have a significance as
formulated through a chosen symbolic system.
Example
# ZP5
Label Has appellative subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE2 Appellative Status
Range E1 CRM Entity
Scope Note This property is used to indicate the entity for which an appellation
holds as institutional fact.
Example
# ZP6
Label ascribes appellation
Super property of ZP9 ascribes contact point [D:ZE3,R: E41]
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE2 Appellative Status
Range E1 CRM Entity
Scope Note This property is used to indicate the appellation which is indicated as
holding for the named subject of the appellative status.
Example
28
# ZP7
Label ascribes appellative relation
Super property of ZP10 ascribes contact point relation [D: ZE3, R:E55]
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE2 Appellative Status
Range E55 Type
Range Target Bundle P1 is identified by, P48 has preferred identifier, P102 has title
Scope Note This property is used to indicate the specific manner in which the
appellation which is indicated as holding for the named subject of the
appellative status pertains to this subject.
Example
# ZP8
Label has contact subject
Super property of
Sub property of ZP5 has appellative subject [D:ZE2, R:E1]
Domain ZE3 Contact Status
Range E39 Actor
Scope Note This property is used to indicate the entity for which a contact point
has been specified as means of contact.
Example
# ZP9
Label ascribes contact point
Super property of
29
Sub property of
Domain ZE3 Contact Status
Range E41 Appellation
Scope Note This property is used to indicate the contact point which is indicated
as holding for the named subject of the contact status.
Example
# ZP10
Label ascribes contact point relation
Super property of
Sub property of ZP7 ascribes appellative relation [D: ZE1, R:E55]
Domain ZE3 Contact Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
contact point which is indicated as holding for the named subject of
the contact status pertains to this subject.
Example
# ZP11
Label has classificatory subject
Super property of ZP14 has functional subject [D:ZE5, R:E72]
ZP17 has social subject [D:ZE6, R:E39]
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE4 Classificatory Status
Range E72 Legal Object
Scope Note This property is used to indicate the entity for which a certain
classification is taken to hold by the instance of classificatory status.
Example
30
# ZP12
Label ascribes classification
Super property of ZP15 ascribes function [D:ZE5, R:E55]
ZP18 ascribes social status [D:ZE6, R:E55]
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE4 Classificatory Status
Range E55 Type
Scope Note This property is used to indicate the type which is indicated as
holding for the subject of the classification status.
Example
# ZP13
Label ascribes classificatory relation
Super property of ZP16 ascribes functional relation [D: ZE5, R:E55]
ZP19 ascribes social status relation [D: ZE6, R:E55]
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE4 Classificatory Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the type
which is indicated as holding for the subject of the classification
status pertains to this subject.
Example
# ZP14
Label has functional subject
Super property of
Sub property of ZP11 has classificatory subject [D:ZE4, R:E1]
31
Domain ZE5 Functional Status
Range E72 Legal Object
Scope Note This property is used to indicate the entity for which a certain
functional classification is taken to hold by the instance of functional
status.
Example
# ZP15
Label ascribes function
Super property of ZP15 ascribes function [D:ZE5, R:E55]
ZP18 ascribes social status [D:ZE6, R:E55]
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE5 Functional Status
Range E55 Type
Scope Note This property is used to indicate the type of function which is
indicated as holding for the subject of the function status.
Example
# ZP16
Label ascribes functional relation
Super property of
Sub property of ZP13 ascribes classification relation [D: ZE4, R:E55]
Domain ZE5 Functional Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
function which is indicated as holding for the subject of the function
status pertains to this subject.
Example
32
# ZP17
Label has social subject
Super property of
Sub property of ZP11 has classificatory subject [D:ZE4, R:E1]
Domain ZE6 Social Status
Range E39 Actor
Scope Note This property is used to indicate the actor for which a certain social
status is taken to hold by the instance of social status.
Example
# ZP18
Label ascribes social status
Super property of
Sub property of ZP12 ascribes classification [D:ZE4, R:E55]
Domain ZE6 Social Status
Range E55 Type
Scope Note This property is used to indicate the type of social status which is
indicated as holding for the subject of the classification status.
Example
# ZP19
Label ascribes social status relation
Super property of
Sub property of ZP13 ascribes classification relation [D: ZE4, R:E55]
Domain ZE6 Functional Status
Range E55 Type
33
Scope Note This property is used to indicate the specific manner in which the type
of social status which is indicated as holding for the subject pertains
to this subject.
Example
# ZP20
Label has custodial subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE7 Custodial Status
Range E72 Legal Object
Scope Note This property is used to indicate the legal object over which a certain
custodial status is taken to hold..
Example
# ZP21
Label ascribes custodian
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE7 Custodial Status
Range E39 Actor
Scope Note This property is used to indicate the custodian to whom the custody
of the legal object which is the subject of the custodial status
redounds.
Example
# ZP22
Label ascribes custodial relation
34
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE7 Custodial Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
custodial status which is indicated as holding over the legal object by
the custodian pertains to this subject.
Example
# ZP23
Label has ownership subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE8 Ownership Status
Range E72 Legal Object
Scope Note This property is used to indicate the legal object over which a certain
ownership status is taken to hold..
Example
# ZP24
Label ascribes owner
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE8 Ownership Status
Range E39 Actor
Scope Note This property is used to indicate the owner to whom the title of the
legal object which is the subject of the ownership status redounds.
35
Example
# ZP25
Label ascribes ownership relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE8 Ownership Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
ownership status which is indicated as holding over the legal object
by the owner pertains to this subject.
Example
# ZP26
Label has residence subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE9 Residence Status
Range E39 Actor
Scope Note This property is used to indicate the actor for whom the residence
status is taken to hold.
Example
# ZP27
Label ascribes residence place
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
36
Domain ZE9 Residence Status
Range E53 Place
Scope Note This property is used to indicate the place at which the subject of the
residence status is taken to reside/dwell/abide.
Example
# ZP28
Label ascribes residence relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE9 Residence Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
residence status which is indicated as holding over the actor pertains
to this subject.
Example
# ZP29
Label has family subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE10 Family Status
Range E21 Person
Scope Note This property is used to indicate the person for whom the family
status is taken to hold.
Example
37
# ZP30
Label ascribes relative
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE10 Family Status
Range E21 Person
Scope Note This property is used to indicate the person ascribed as having a
family relation to the subject person of the family status.
Example
# ZP31
Label ascribes family relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE10 Family Status
Range E55 Type
Scope Note This property is used to indicate the specific type of family status
which is indicated as holding between the subject individual and
his/her ascribed relative.
Example
# ZP32
Label has membership subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE11 Membership Status
38
Range E39 Actor
Scope Note This property is used to indicate the person for whom the
membership status is taken to hold.
Example
# ZP33
Label ascribes group
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE11 Membership Status
Range E74 Group
Scope Note This property is used to indicate the group ascribed to the subject
person of the membership status as having a membership relation
thereto.
Example
# ZP34
Label ascribes membership relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE11 Membership Status
Range E55 Type
Scope Note This property is used to indicate the specific type of membership
status which is indicated as holding between the subject individual
and the group to which she/he is ascribed.
Example
39
# ZP35
Label has referential subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE12 Referential Status
Range E89 Propositional Object
Scope Note This property is used to indicate the propositional object for which the
referential status is taken to hold.
Example
# ZP36
Label ascribes referent
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE12 Referential Status
Range E1 CRM Entity
Scope Note This property is used to indicate the referent to which the subject
propositional object is taken to refer.
Example
# ZP37
Label ascribes referential relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE12 Referential Status
Range E55 Type
Scope Note This property is used to indicate the specific type of referential status
40
which is indicated as holding between the subject propositional object
and its indicated intended referent.
Example
# ZP38
Label ascribes referential mode
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE12 Referential Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
referential status which is indicated as holding between the subject
propositional object and its indicated intended referent holds.
Example
# ZP39
Label invokes
Super property of
Sub property of P33 used specific technique
Domain ZE13 Speech Act
Range E29 Design or Procedure
Scope Note This property is used to indicate the normative rule which a speech
act relies on as typological and as sanctioning code in order to bring
out a token/instance of the institutional fact it prescribes.
Example
# ZP40
41
Label performs
Super property of
Sub property of P33 used specific technique
Domain ZE13 Speech Act
Range E29 Design or Procedure
Scope Note This property is used to indicate the performance plan sanctioned by
normative rule appealed to by the speech act to bring about a new
institutional fact. This performance plan indicates the series of
necessary procedures that must be followed in order for the speech
act to have been successfully carried out and to have created a
genuine instance of the institutional fact that it was designed to make
possible.
Example
# ZP41
Label utters
Super property of
Sub property of P16 used specific object
Domain ZE13 Speech Act
Range E33 Linguistic Object
Scope Note It is typical of performance plans for normative procedures to include
a necessary invoking clause of set of clauses which must be uttered
in the course of the performance of the speech act in order to for it to
be successfully invoked. This property enables the documentation of
the use of such a linguistic object.
Example
# ZP42
Label Intentionally initiates
Super property of
42
Sub property of O13 triggers
Domain ZE13 Speech Act
Range ZE1 Institutional Fact
Scope Note This property is used to connect the instance of speech act to the
instance of institutional fact which it brought into existence through
the correct performance of the specified performance to bring about
the norm type it aimed to bring about.
Example
# ZP43
Label has similarity subject
Super property of
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE14 Similarity Status
Range E1 CRM Entity
Scope Note This property is used to indicate one of two entities for which the
similarity status is taken to hold.
Example
# ZP44
Label ascribes similarity target
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE14 Similarity Status
Range E1 CRM Entity
Scope Note This property is used to indicate the other entity for which the
similarity status is taken to hold.
43
Example
# ZP45
Label ascribes similarity relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE12 Referential Status
Range E55 Type
Scope Note This property is used to indicate the specific type of similarity which is
indicated as holding between the two entities indicated in the
similarity status.
Example
# ZP46
Label ascribes similarity mode
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE14 Similarity Status
Range E55 Type
Scope Note This property is used to indicate the specific manner in which the
similarity status, which is indicated as holding between two entities
indicated in the similarity status, is the case.
Example
# ZP47
Label has set belonging subject
Super property of
44
Sub property of ZP1 has intentional subject [D: ZE1, R: E1]
Domain ZE15 Set Status
Range E1 CRM Entity
Scope Note This property is used to indicate an entity which is taken as belonging
to a particular set by the instance of set status..
Example
# ZP48
Label ascribes set
Super property of
Sub property of ZP2 ascribes intentional target [D: ZE1, R:E1]
Domain ZE15 Set Status
Range ZE24 Notional Set
Scope Note This property is used to indicate the set to which an entity is indicated
as belonging .
Example
# ZP49
Label ascribes set relation
Super property of
Sub property of ZP3 ascribes intentional relation [D: ZE1, R:E55]
Domain ZE15 Set Status
Range E55 Type
Scope Note This property is used to indicate the specific type of belonging to the
set which is indicated as holding between the subject entity and the
target set.
Example
45
# ZP50
Label uttered
Super property of
Sub property of P16 used specific object [D: ZE1, R:E55]
Domain ZE16 Utterance Event
Range E73 Information Object
Scope Note This property is used to connect an instance of utterance event to the
specific information object that was used in its performance.
Example
# ZP51
Label has former or current set member
Super property of
Sub property of
Domain ZE24 Notional Set
Range E1 CRM Entity
Scope Note This property is used to connect an instance of set to an entity
considered to be one of its members.
Example
# ZP52
Label Intentionally terminates
Super property of
Sub property of O13 triggers
Domain ZE13 Speech Act
46
Range ZE1 Institutional Fact
Scope Note This property is used to connect the instance of speech act to the
instance of institutional fact which it cancels through the correct
performance of the specified performance to bring about the norm
type it aimed to bring about.
Example
# ZP53
Label Initiates for
Super property of
Sub property of
Domain ZE13 Speech Act
Range E74 Group
Scope Note This property is used to connect the instance of speech act to the
instance of group for whom it initiates the existence of a social fact
through its performance.
Example
