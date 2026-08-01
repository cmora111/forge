# INQ-0002

## Question

Where should meaning reside:
within an identifier,
or within the surrounding hierarchy?

## Observation

While designing the Stage Method,
we repeatedly removed redundant information
from identifiers because that information
was already expressed by the surrounding
structure.

Examples:

backups/stages/
    stage2-servo-verification-20260728-152036

instead of

backups/stages/
    stage2-servo-verification-backup-20260728-152036

The directory hierarchy already communicates
that the artifact is a backup.

Repeating "backup" in the identifier
adds no new information.


## Hypothesis

Context should communicate classification.

Identifiers should communicate identity.

Redundant meaning should be avoided.
