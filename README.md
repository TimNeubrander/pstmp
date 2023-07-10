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


On-ramp 2. allow for hybrid participation on existing platforms

Publication
- Creditright over copyright (copyright to protect creditright by default.  May be solved by Creative Commons?)
- include default licensing scheme on genesis

Challenges
- forked/multiverse discussion splitting
- 

On-ramp 3. Create Pseudonymous account/identity
- Pseudonymous accounts create the basis for reputational systems.  ActivityPub uses "Actor" ID
- Balance privacy and transparency. Allow complete privacy or transparency to start and allow transition to openess (not required) or allow alternate pseudonyms for public figure to allow private engagement.

Entity (Actor?) -> Delegates (trusted device/app/self-host) -> Identities -> Pseudonym(s) on platform
Core User Trust -> iPhone -> User Work (user-work@example.com) -> Display: @user@mastodon.social, ID: (Pseudonym hash)

Challenges
- How can community protect participants (different responsibility models for different communities?)

Discussions among entities can be transformed into a collection of messages.  Stored messages combined necessary metadata may be used to fully or partially reconstruct discussions from the perspective of participants.

Discussion may be as simple as a thought 100 years ahead of it's time waiting for a future generation to appreciate it.

Pseudonym must be deterministically generated from parent entity

Structured collection of messages is a discussion
Discussions may be publish in part or whole by 

Transformation functions
generation (deletion/retraction)
witness/validation (denial/invalidation)
Optical Character Recognition (screenshot)
Transcription (Text-to-Speech)
Alt Tag (AI Image Generation)
Tokenize (Compile)
fork graph (merge graph)
attribution


Entity roles
message author
message forwarded
message publisher
discussion initiator
discussion moderation
discussion publisher

Identity functions
Trust Delegate
Retire Delegate (remove trust)

message anatomony
Body (required)
Body hash (required)
reply to context
body signature
reply to sub-discussion (message) signature
reply to discussion signature
message and message context
