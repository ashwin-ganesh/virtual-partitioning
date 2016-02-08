Applications can be logically separated to parts that face
different types of threats, or suffer dissimilar exposure
to a particular threat because of external events or innate
properties of the software. Based on this observation,
we propose the virtual partitioning of applications that
will allow the selective and targeted application of those
protectionmechanisms that are most needed on each partition,
or manage an application’s attack surface by protecting
the most exposed partition. We demonstrate the
value of our scheme by introducing a methodology to
automatically partition software, based on an intrinsic
property such as user authentication. Our approach is
able to automatically determine the point where the user
authenticates, without access to source code. At runtime,
we partition binaries using a binary monitor that
utilizes the identified authentication points to split execution
to pre- and post-authentications parts, and adapts
defenses by switching between protection mechanisms
of varied intensity, such as dynamic taint analysis and
instruction-set randomization. We evaluate our approach
using seven well-known Internet applications, including
the MySQL database server. Our results indicate that our
methodology can accurately discover the authentication
points of applications. Furthermore, we show that using
virtual partitioning to apply a costly protection mechanism on the most exposed part of these services, the pre-authenticated part, can reduce performance overhead by up to 5x, depending on the nature of the application.