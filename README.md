h1. Levenshtein-mySQL

Levenshtein-SQL implements the "Levenshtein distance":http://en.wikipedia.org/wiki/Levenshtein_Distance. It's string metric for measuring the amount of difference between two sequences. This implemetation originally wrote by Jason Rust.

h2. Usage

<pre>
SELECT term FROM words WHERE levenshtein('search_string', term) BETWEEN 0 AND 4
SELECT term levenshtein(term, 'search_string') as dist from words where levenshtein(term, 'search_string') as dist<4 limit 2;
</pre>

h2. Project info

More info can be found at: http://stackoverflow.com/questions/4671378/levenshtein-mysql-php
