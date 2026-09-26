# Licence: MIT, and why

AGPL-3.0 was chosen for `space-seeker` because that project wraps an AGPL
client. Nothing here wraps anybody's code, so that reasoning does not transfer
and MIT is the honest choice.

The stated goal was: anyone may branch this, do what they like, and the author
does not need to be paid or credited. MIT is the licence that grants exactly
that and nothing more. A public repo with *no* licence is worse than either —
it is "all rights reserved" by default, so nobody could legally use it at all.

### The part that cannot be done

A licence grants permission. **It cannot charge anybody.** "MIT plus Space
Bunny plus a royalty on downstream use" is not a licence: the royalty clause
cannot be enforced by anyone, and putting it in the document makes the whole
thing look unserious to a lawyer.

If payment is ever wanted, that is a contract, not a licence, and it belongs in
a separate document. `NOTICE` is the enforceable half of "give us credit" —
attribution with no conditions attached.

## Changing it

    sed -i 's/MIT/Apache-2.0/' LICENSE     # adds an explicit patent grant
    # then commit, tag, and force-push the tag

Apache-2.0 is the upgrade worth considering: it adds a patent grant and a
formal NOTICE mechanism, which MIT has no equivalent of.
