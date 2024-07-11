<p align="center">
<img width="256" height="256" src="images/oewn.png">
</p>

# Open English Wordnet in WNDB format

This project  produces a version of Open English Wordnet data in the form of

-  __wndb__ files conforming to the [WNDB standard](https://wordnet.princeton.edu/documentation/wndb5wn) 

## lossless or seamless ?

### new lossless extended format

This provides **lossless** database files of the Open English Wordnet in [WNDB](https://wordnet.princeton.edu/documentation/wndb5wn) format. 

Downloadable as 
[tar.gz](https://x-englishwordnet.github.io/wndb/oewn_2024.dict.tar.gz) or 
[zip](https://x-englishwordnet.github.io/wndb/oewn_2024.zip).

With OEWN, new **types of relations** have been introduced and their ad-hoc encoding may not be recognized by some libraries (JWI) while others don't bother (NLTK).

Cases in point are
- the new '*is caused by*' relation, encoded with a '&gt;&circ;' pointer.
- the new '*is entailed by*' relation, encoded with a '*&circ;' pointer.

While this encoding scheme is not defined in the PWN 3.1 format, it is thought to be compatible with it.

### compatible or seamless format

This is compatible with PWN3.1 format and may be required to work with some libraries (e.g. JWI). It is thought to be a **seamless** replacement of the PWN 3.1 release provided it is not assumed lexIDs are limited to the [0..15] range. However new relations that are not defined in PWN 3.1 have been dropped.

Downloadable as 
[tar.gz](https://x-englishwordnet.github.io/wndb/oewn_2024_compat.dict.tar.gz) or 
[zip](https://x-englishwordnet.github.io/wndb/oewn_2024_compat.zip).

## how ?

The data is produced by the newer OEWNTK tool suite.

See [OEWNTK](https://github.com/oewntk)
