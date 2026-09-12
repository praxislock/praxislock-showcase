# Validation

PraxisLock is currently validated as an engineering prototype.

## Current CI status

The private development repository has a green GitHub Actions pipeline validating:

| Check | Status |
|---|---|
| Security regression suite | 64 tests |
| Python 3.11 | Passing |
| Python 3.12 | Passing |
| LangGraph demo smoke test | Passing |
| Package build | Passing |

## What these results mean

The tests validate important security invariants and regression behavior, including:

- agent identity tampering
- payload integrity
- replay rejection
- session isolation
- destination-policy edge cases
- DLP handling
- MCP tool-definition changes
- approval behavior
- LangChain/LangGraph enforcement behavior
- end-to-end taint → sensitive action scenarios

## What these results do **not** mean

These results do **not** prove:

- perfect prompt-injection detection
- zero false positives
- protection against every AI-agent attack
- enterprise production readiness
- independent OWASP certification
- formal security verification

PraxisLock is still undergoing adversarial validation.

## Next validation work

- larger malicious/benign indirect-injection corpora
- multi-step attack chains
- cross-agent attacks
- Unicode / encoding / obfuscation attacks
- DLP evasion
- destination bypass fuzzing
- concurrent replay testing
- failure / chaos testing
- performance testing
- restart recovery
- real agent-framework integrations
