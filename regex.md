<!-- This file will contain some helpful regular expressions -->

<!-- 1 MATCHING PHONE NUMBERS -->

Capture	415-555-1234	
Capture	650-555-2345	
Capture	(416)555-3456	
Capture	202 555 4567	
Capture	4035555678	
Capture	1 416 555 9292

\(?1?\d*\)?(\s|-|\d)?\d*(\s|-|w+)?\d*(\s)?\d*

<!-- Capture SPECIFIC PARTS of Phone Numbers -->
