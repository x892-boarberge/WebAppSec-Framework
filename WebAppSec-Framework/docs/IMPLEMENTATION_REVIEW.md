# Implementation review — issues to resolve before submission

This review accompanies the supplied files. It does not silently alter their research content.

1. **OWASP edition:** the JSON metadata uses OWASP Top 10:2021. The project's current standards baseline must be reconciled with the verified OWASP Top 10:2025 edition before finalising mappings. Review every category assignment rather than changing the metadata string alone.
2. **ASVS placeholders:** `ASVS-REQ-PENDING` remains in the register. Do not describe the Verify layer as fully mapped until exact ASVS 5.0 requirement IDs have been checked against the official standard.
3. **Academic evidence:** `ACADEMIC-PENDING` remains in every entry. The evidence requirement is not met until suitable peer-reviewed sources are selected and cited.
4. **Vulnerability scope overlap:** V06 combines weak authentication with excessive authentication attempts; V07 combines session fixation with missing session expiry; V08 combines password hashing with transport/storage cryptography. These are distinct weakness mechanisms and their CWE mappings and assessments need narrowing or explicit separation.
5. **V09 classification:** CWE-16 is broad. The entry should either define a precise representative misconfiguration and map it to a more specific CWE, or justify retaining a broad category-level entry.
6. **V10:** CWE-1395 is used for dependency on a vulnerable third-party component. Keep it distinct from unmaintained components (CWE-1104); confirm the vulnerability definition and OWASP mapping are aligned.
7. **WSTG references:** entries explicitly marked VERIFY must be checked against the chosen WSTG edition. Do not treat a label as verified merely because it appears in the JSON.
8. **Risk method:** arithmetic currently checks out for all 12 entries. The ordinal likelihood and impact judgements still require consistent scoring anchors and defensible entry-specific justifications.
9. **Test status:** T01 is a blank execution record and T02–T08 are templates. No test has been run by creating these files. Record actual environment, observations, pass/fail outcome and defects after execution.
10. **Prototype security/quality:** the prototype inserts register values into `innerHTML`. Since the register is local and curated this is a controlled academic demonstration, but the implementation should still escape untrusted text or use safe DOM text APIs as a quality improvement. Do not present it as a production security tool.
11. **Scope consistency:** the prototype is static and JSON-driven. Do not add a database, authentication, backend, scanner or ML component unless the project scope is formally changed and justified.
