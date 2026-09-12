# Threat Model

PraxisLock focuses on **runtime threats to tool-using AI agents**.

## Primary threat classes

### Indirect prompt injection
Untrusted content attempts to modify agent behavior.

### Intent divergence
An agent begins taking actions that are not justified by the original user goal.

### Sensitive-data exfiltration
An agent attempts to send secrets, credentials, personal information, or protected data to an unauthorized destination.

### Excessive tool authority
An agent has access to capabilities that are unnecessary for its current task.

### Tool / MCP supply-chain changes
A previously trusted tool changes its description, schema, behavior, or authority.

### Agent identity abuse
An attacker attempts to impersonate another agent or act using a different security identity.

### Signed-message replay
A previously valid agent message is replayed to repeat an action.

### Approval replay / substitution
An approval intended for one exact action is reused for a different action.

### Memory poisoning
Untrusted content is stored and later influences behavior outside the original interaction.

### Multi-agent contamination
Compromised information propagates from one agent to another.

## Out of scope / not claimed

The current prototype does not claim to solve every aspect of:

- underlying model compromise
- malicious model weights
- host / kernel compromise
- cloud-provider compromise
- physical device compromise
- all social-engineering attacks
- all novel prompt-injection techniques

PraxisLock is designed as one security boundary in a broader defense-in-depth architecture.
