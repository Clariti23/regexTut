Resource: https://regexr.com/

Fun Facts
(?<=) : This is called a positive look behind. This will match a group before the main expression without including it in the result. 

# Example 1
\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})

This expression will match: 
1234567890
123-456-7890
(123) 456-7890
 
 # Example 2
(\+1[ -])?\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})

This expression will match:
+1 123 456 7890
+1-123 456 7890

as well as all of the previous phone number iterations.
