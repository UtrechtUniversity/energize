# energize
Reliable data transfer to and from iRODS

# Use cases

Energize is an abstraction layer that implements reliable data transfer
to and from iRODS. The main use cases are:
- Working around software bugs, for example by partitioning
  transfers of large number of files in multiple parts to limit the
  impact of memory leaks.
- Restarting transfers after network issues and keeping track of what
  data has been transferred previously.
- Facilitating transfer of data in batches, for example if a researcher
  intends to upload data from a laptop at night, and temporarily halt
  the transfer during the daytime.
- Generating reports of data transfers for provenance tracking
