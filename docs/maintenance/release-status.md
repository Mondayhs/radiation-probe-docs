# Release & Verification Status

!!! warning "No approved flight baseline declared by this public website"
    The current released FSW, hardware/ICD pairing and validation status must be confirmed from the private project records. Do not infer flight readiness from a successful build or a working GUI.

| System | Revision / commit | Evidence | Status |
|---|---|---|---|
| CRP PCB | TBD | Board drawings and inspection | Unverified here |
| CRP FSW | TBD | Tagged release and regression test | Unverified here |
| CRP ICD | TBD | Approved revision | Unverified here |
| Test GUI / parser | TBD | Reference packets and comparison | Unverified here |
| Long-run operation | TBD | Raw logs and signed test report | Evidence pending |
| Proton SEE tests | TBD | Test plan, logs and report | Evidence pending |

## Release process recommendation

1. Freeze firmware commit and build artifacts.
2. Identify matching PCB and ICD revisions.
3. Capture test results under controlled conditions.
4. Document known issues, deviations and recovery steps.
5. Obtain engineering review before promotion to a flight baseline.

Private internal release history should map each public design-evolution item to a commit and corresponding test evidence.
