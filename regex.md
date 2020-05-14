<!-- This file will contain some helpful regular expressions -->

<!-- 1 MATCHING PHONE NUMBERS -->

Capture	415-555-1234	
Capture	650-555-2345	
Capture	(416)555-3456	
Capture	202 555 4567	
Capture	4035555678	
Capture	1 416 555 9292
<!-- REGEX -->
\(?1?\d*\)?(\s|-|\d)?\d*(\s|-|w+)?\d*(\s)?\d*

<!-- Capture SPECIFIC PARTS of Phone Numbers -->


Task	Text	Capture Groups	 
Capture	415-555-1234	415	Success
Capture	650-555-2345	650	Success
Capture	(416)555-3456	416	Success
Capture	202 555 4567	202	Success
Capture	4035555678	403	Success
Capture	1 416 555 9292	416	Success

<!-- REGEX -->
(\(|1)?(\d{3})

<!-- THREE: MATCH EMAILS -->

Task	Text	Capture Groups	 
Capture	tom@hogwarts.com	tom	Success
Capture	tom.riddle@hogwarts.com	tom.riddle	Success
Capture	tom.riddle+regexone@hogwarts.com	tom.riddle	Success
Capture	tom@hogwarts.eu.com	tom	Success
Capture	potter@hogwarts.com	potter	Success
Capture	harry@hogwarts.com	harry	Success
Capture	hermione+regexone@hogwarts.com	hermione	Success

<!-- REGEX -->
^([\w\.]*)

<!-- Capture HTML Tags -->
<(\w+)
<!-- From a list of files, caputre only image files ending with .jpg, .png, or .gif -->
(\w+)\.(jpg|png|gif)$
