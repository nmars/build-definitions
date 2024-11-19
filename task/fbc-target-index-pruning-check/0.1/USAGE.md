# fbc-pruning-check task

### Purpose:
- This task ensures file-based catalog (FBC) components do not remove previously released versions of operators from a target catalog, specified
in the `TARGET_INDEX` parameter, which by default points to the production Red Hat catalog `registry.redhat.io/redhat/redhat-operator-index`.

### What this check does:
- Derives the OCP version from the FBC image's `org.opencontainers.image.base.name` annotation or label.
- Runs `opm render` on both the FBC image and the TARGET_INDEX.
- Checks if the FBC fragment would remove a channel or any entry from an existing channel in the TARGET_INDEX.
