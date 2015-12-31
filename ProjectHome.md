In the Java space (and now .Net and Ruby), I'm a huge fan of the simplicity and power of the Apache ibatis project (http://ibatis.apache.org/).  The mysql package has no prepared statements, mysqli is simply too buggy and noone seems to be actively maintaining it, leaving PDO.  It's not a bad alternative.  It's just not ibatis. :)  I also prefer to externalize SQL.

Key features of ibatis:

  * Dynamic SQL;
  * Caching;
  * External SQL;
  * Lazy-loading;
  * Discriminated types; and
  * Type mapping.

I intend to release a version, that I'm at this stage calling (unimaginatively) pbatis, under the same Apache License 2.0 as ibatis.

The sqlmap.xml files will be identical to the ibatis version.  Initially this will be built on top of a PDO wrapper but at some point I intend to bypass that or provide other implementations.

The first version is aimed at providing support for the basic SQL statement types over PDO.