# tsexample

Fork of tsexample

Text Search Parser which split by whitespace only:

			space (0x20, ' ')
			form feed (0x0c, '\f')
			line feed (0x0a, '\n')
			carriage return (0x0d, '\r')
			horizontal tab (0x09, '\t')
			vertical tab (0x0b, '\v') 

Example:

	SELECT * FROM ts_parse(  'sample_parser', '3,6V 3.6V MySQL Win-98 xyz #$%^& test@test.com c:\docs /etc/lib 678678678');

	tokid	token
	1	3,6V
	1	3.6V
	1	MySQL
	1	Win-98
	1	xyz
	1	#$%^&
	1	test@test.com
	1	c:\docs
	1	/etc/lib
	2	678678678


