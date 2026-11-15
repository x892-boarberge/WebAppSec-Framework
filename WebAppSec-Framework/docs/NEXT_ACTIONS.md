# NEXT ACTIONS

## Blocking (nothing downstream is valid without these)
- [ ] OWASP Top 10 edition verified on owasp.org — edition: _______ — access date: _______
- [ ] OWASP ASVS version verified on asvs.owasp.org — version: _______ — access date: _______
- [ ] OWASP WSTG version verified on owasp.org/wstg — version: _______ — access date: _______
- [ ] All 12 CWE IDs spot-checked on cwe.mitre.org
- [ ] Replace every `ASVS-REQ-PENDING` in vulnerabilities.json with the exact ASVS 5.0 requirement ID
- [ ] Replace every `ACADEMIC-PENDING` with a peer-reviewed source that supports the entry

## This week
- [ ] Resolve V03 academic source (command injection)
- [ ] Resolve V04 academic source (access control)
- [ ] Resolve V05 academic source (function-level authorisation)
- [ ] Resolve V06 academic source (authentication, rate limiting)
- [ ] Resolve V07 academic source (session management)
- [ ] Resolve V08 academic source (cryptography)
- [ ] Resolve V09 academic source (misconfiguration)
- [ ] Resolve V10 academic source (dependencies, SBOM)
- [ ] Resolve V11 academic source (logging, detection)
- [ ] Resolve V12 academic source (SSRF)

## Build
- [ ] Start HTTP server and verify the prototype renders correctly
- [ ] Run T01–T08 and complete each test_results/*.md
- [ ] Confirm at least one test fails and is then fixed (documented defect + resolution)

## Do not
- [ ] Do not add a second dataset anywhere — the JSON is the only source of truth
- [ ] Do not add features not listed in the scope freeze (HANDOFF §3)
- [ ] Do not build a backend, authentication, database, or ML component

## Weekly discipline
- [ ] Update source log with every new source
- [ ] Record one notebook entry (Concept / Explanation / Example / Application / Questions)
- [ ] Confirm no scope-freeze item has been breached
