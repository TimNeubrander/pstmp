# pstmp
Pseudonymous Stored Message Protocol

Distributed messaging protocol inspired by git and Steve Gibson's [SQRL](https://www.grc.com/sqrl/sqrl.htm)

# Brain Dump

PStMP attempts create a stored message format and associated protocol to facilitate verifiable distributed discussions among pseudonymous entities.  Distributed Discussions may be moderated, curated, branched, merged independently.

### On-ramp 1. Create transformer to take existing discussion format into PStMP and back into original format (Lossy and lossless versions)

discussion formats
- webpage
- blogs, RSS
- AI mediated (ChatGPT)
- email
- Podcast Audio
- social media public (reddit, twitter)
- social media DM
- multi contributor (Wikipedia, git)
- Forum (stack overflow)

Challenges
- Are URIs requirements
- protocol for "Privacy-ish" preservation (may not be compatible with both verifiable and reconstructable)
- federated gatekeeping for private group discussions
- onboarding content (claim, reputation, or proof)


### On-ramp 2. allow for hybrid participation on existing platforms

Publication
- Creditright over copyright (copyright to protect creditright by default.  May be solved by Creative Commons?)
- include default licensing scheme on genesis

Challenges
- forked/multiverse discussion splitting
- 

### On-ramp 3. Create Pseudonymous account/identity

User Facing identity presentation
- Pseudonymous accounts create the basis for reputational systems.  ActivityPub uses "Actor" ID
- Some users will want to connect a subset of pseudonyms to "real world" identities (verified accounts
- Balance privacy and transparency. Allow complete privacy or transparency to start and allow transition to openness (not required) or allow alternate pseudonyms for public figure to allow private engagement.

Entity (Actor?) -> Delegates (trusted device/app/self-host) -> Identities -> Pseudonym(s) on platform
Core User Trust -> iPhone -> User Work (user-work@example.com) -> Display: @user@mastodon.social, ID: (Pseudonym hash)

Challenges
- How can community protect participants (different responsibility models for different communities?)
- Stolen identity resolution (may require trust/proof)
- If proof who validates? (Some validation systems require uploading of government issues documentation)

### On-ramp 4. Reputation systems

Is it possible to have an open federated moderation system?  Many existing reputation systems rely on opacity ("Security Reasons") for proper functioning as almost all systems are instituted to prevent harm from "bad" actors

What is reputation?
- reputation is metadata (contextualized?) about an instantiation of an entity that is not controlled (must not be controlled??) by that entity
- May be used to limit access to platform

Existing reputation systems
- email spam filtering (Domain, Account, message)
- voting systems like reddit, youtube
- Interaction tracker (engagement, click, stop scroll signals)
- Captcha completion
- Peer reviewed research (reputation by association??)


Challenges
- Well implemented reputation systems foster trust in platforms, and may be the basis for continued platform participation for the platform's users
- "Fairness" platforms that implement "unfair" reuptation systems may lose trust


Discussions among entities can be transformed into a collection of messages.  Stored messages combined necessary metadata may be used to fully or partially reconstruct discussions from the perspective of participants.

Discussion may be as simple as a thought 100 years ahead of it's time waiting for a future generation to appreciate it.

Pseudonym must be deterministically generated from parent entity

Structured collection of messages is a discussion
Discussions may be publish in part or whole by 

Transformation functions
- generation (deletion/retraction)
- witness/validation (denial/invalidation)
- Optical Character Recognition (screenshot)
- Transcription (Text-to-Speech)
- Alt Tag (AI Image Generation)
- Tokenize (Compile)
- fork graph (merge graph)
- attribution


Entity roles
- message author
- message forwarded
- message publisher
- discussion initiator
- discussion moderation
- discussion publisher

Identity functions
- Establish Entity Root Trust
- Replace root trust
- Generate Delegate (requires Root)
- Retire Delegate (remove trust)
- Delegate Authenticates Root Trust (may require OOB Proof Key)

message anatomony
- Body (required)
- Body hash (required)
- reply to context
- body signature
- reply to sub-discussion (message) signature
- reply to discussion signature
- message and message context
 
Trust Chain
Entity (Root Trust) -> Master Proof Key
Root Trust + Delegate Proof Key -> Delegate 
Entity + Master Proof key -> Replacement Entity (Can generate self Destruct claim verifiable by delegates using master Proof key???  Optional pointer to replacement entity)
Entity + Delegate Proof Key -> Replace Delegate (Can generate destroy delegate claim verifiable by public with pseudonym and destroy claim???, optional pointer to replacment delegate)
