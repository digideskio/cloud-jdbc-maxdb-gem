# JDBC driver for MaxDB as a Ruby gem

This is a Ruby gem that wraps the JDBC driver for the [SAP MaxDB database](
http://maxdb.sap.com/).

This gem is needed by the [ActiveRecord JDBC adapter for MaxDB](
https://github.com/sapnwcloudlabs/activerecord-maxdb-adapter).

**Note**: In order to have this gem build, install and work correctly, you would
need to obtain the JDBC driver of the MaxDB database, and place it under the
/lib folder of the gem. Please name the file sapdbc.jar, or adjust accordingly
the gem metadata descriptors which refer to it, if you need the name to be different
(those are jdbc-maxdb.gemspec, lib/jdbc/maxdb.rb and optionally Manifest.txt).
You can obtain the jar file from [here](http://www.sapdb.org/sap_db_jdbc.htm).


Please build the gem from sources and install it:

    jruby -S gem build jdbc-maxdb.gemspec
	jruby -S gem install jdbc-maxdb