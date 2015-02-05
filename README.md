iStatServer
===========

A dumb python server to do smart statistics things.

Install
-------

    sudo pip install -r deps.txt

Use
---

In a terminal, fire up the server:

    ./serve

Then, in a different terminal, try sending it a file:

    curl -F file=@demo.csv localhost:5000/file
    > Great Success!

If everything is properly configured, there should now be a demo.csv file in the uploads/ directory.

API
---

POST your data as a CSV file to any of the following endpoints:

=== /k-means ===

Returns a JSON string containing...

=== /ward ===

Returns a JSON string containing...

=== /hca ===

Returns a JSON string containing...

=== /nmf ===

Returns a JSON string containing the output component matrices (indexed as "H" and "W"), along with the mean error term for the factorization.
