# NAME

Template::Plugin::Package - allow calling of class methods on arbitrary classes that do not accept the class name as their first argument.

# SYNOPSIS

    [% USE foo = Package('Foo') %]
    [% foo.bar('arguments', 'to', 'bar') %]

# DESCRIPTION

Template::Plugin::Package allows you to call functions in arbitrary
packages much like Template::Plugin::Class does, but the methods are called
without the package class name as the first parameter.

Use Template::Plugin::Package to call class methods that in normal Perl
code require '::' to call.

Use Template::Plugin::Class to call class methods that require '->' to
call.

# SEE ALSO

[Template::Plugin::Class](https://metacpan.org/pod/Template%3A%3APlugin%3A%3AClass)

# COPYRIGHT & LICENSE

Copyright 2024 Andy Lester.

This library is free software; you can redistribute it and/or modify it
under the terms of the Artistic License version 2.0.

# ACKNOWLEDGEMENTS

Template::Plugin::Package is taken directly from Template::Plugin::Class.

# AUTHOR

Current maintainer: Andy Lester, `<andy at petdance.com>`
