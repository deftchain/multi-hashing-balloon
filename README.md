##balloon-multi-hashing
__multi-hashing 0.0.9 with support for balloon hashing algorithm (balloon_128)__

### further reading / credits
balloon hashing is a memory-hard pow algorithm rivaling argon2 (secure hash at 1/8th memory cost).
the original password hashing algorithm was developed by Dan Boneh, Henry Corrigan-Gibbs and Stuart Schechter.
ported for PoW use by barrystyle (deft developer); this being the first coin ever to put it to use.

### installation:
not particularly fond of nodejs (or its convoluted packaging mechanisms). after installing nomp/unomp and running
'npm update' from root of pool; change to ./node_modules/stratum-pool/multi-hashing, delete the contents and
replace them with this repo (making sure to delete the .git files etc).

drop back in directory structure (so you're at ./node_modules/stratum-pool) and run 'npm install multi-hashing/'
(making sure the trailing forward slash is there) and it will compile the module. then copy the 'algoProperties.js'
over the existing one under './node_modules/stratum-pool/lib'.

then, create a coin definition under ./coins with 'balloon' as the algorithm.
