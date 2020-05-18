https://regexr.com/


(?<=) : This is called a positive look behind. This will match a group before the main expression without including it in the result. 

\(?(\d{3})\)?[ -]?(\d{3})[ -]?(\d{4})

This expression will match: 
1234567890
123-456-7890
(123) 456-7890

