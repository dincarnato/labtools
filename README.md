# IncaRNAto lab's tools

### Note:
All tools rely upon RNA Framework. Make sure that the `lib/` folder of RNA Framework is added to the `$PERL5LIB` environment variable:

```bash
$ export PERL5LIB=$PERL5LIB:/path/to/RNA/Framework
```

or edit the relevant path in the individual scripts:

```perl
use lib "/path/to/RNAFramework/lib";
```
<br/>

### Tools:

__cm-builder:__ automaGically builds structural alignments of RNAs and Infernal's CMs starting from a single sequence+structure and iteratively refining the model by searching against a database of related sequences

__consensusFold:__ predicts a consensus secondary structure by aggregating multiple reactivity profiles using [ViennaRNA](https://www.tbi.univie.ac.at/RNA/)'s RNAalifold. This tool will become part of RNAFramework's `rf-fold` in future releases.

__filterMM:__ post-processing of MM files prior to analysis with DRACO (filtering, extraction of target regions, etc.). This tool will become part of RNAFramework in future releases.

__stockholmPolish:__ cleanup of Stockholm alignments generated by `cm-builder`

__stockholm2html:__ structure-aware coloring of Stockholm alignments

__transcriptome2genome:__ transcriptome-level to genome-level conversion of BED annotations