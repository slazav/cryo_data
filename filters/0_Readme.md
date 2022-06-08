Input and output filters for graphene databases
(see https://github.com/slazav/graphene).

These TCL scripts are called when one put or get a value to a database.
They work with global variables `time`, `data`, and `storage` (the last
one is set only for input filters, `*:0`).

