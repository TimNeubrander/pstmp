# pstmp
Pseudonymous Stored Message Protocol

Distributed messaging protocol inspired by git and Steve Gibson's [SQRL](https://www.grc.com/sqrl/sqrl.htm)

# Brain Dump

PStMP attempts create a stored message format and associated protocol to facilitate verifiable distributed discussions among pseudonymouns entities.  Distrubited Discussions may be moderated, curated, branched, merged independantly.

On-ramp 1. create transformer to take existing discussion format into PStMP and back into original format (Lossy and lossess versions)

discussion formats
- webpage
- blogs, RSS
- AI mediated (ChatGPT)
- email
- Podcast Audio
- social media public (reddit, twitter)
- social media DM
- multi contrubitor (wikipedia, git)
- Forum (stack overflow)


Challenges
- Are URIs requirements
- protocol for "Privacy-ish" preservation (may not be compatable with both verifiable and reconstructable)
- federated gatekeeping for private group discussions
- onboarding content (claim, reputation, or proof)


Discussions among entities can be transformed into a collection of messages.  Stored messages combined necessary metadata may be used to fully or partially reconstruct discussions from the perspective of 

Discussion may be as simple as 

Pseudonym must be deterministically generated from parent entity

Structured collection of messages is a discussion
Discussions may be publish in part or whole by 

Transformation functions
generation


Entity roles
message author
message forwarded
message publisher
discussion initiator
discussion moderation
discussion publisher

message anatomony
Body (required)
Body hash (required)
reply to context
body signature
reply to sub-discussion (message) signature
reply to discussion signature
message and message context
