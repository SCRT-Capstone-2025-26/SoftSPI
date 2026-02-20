SoftSPI
=======

A fork of SoftSPI with locking. There appear to be some bugs (?) and strange implementations that this fork doesn't (yet in may in the future).

This may end up being optimized for performance in the future, but currently is not. Currently the code locks and unlocks a mutex every transaction. If you want to maintain control over the SPI through many transactions then you can lock it before (I don't know if pico mutexes are fair so this may be questionable).

This fork is only designed for the RP2040.
