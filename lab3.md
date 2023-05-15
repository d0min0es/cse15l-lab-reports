# Lab 3 - **Researching Commands**
## Command Options - Grep Command

### **Grep -l Command**

Example 1
```
Steves-MacBook-Pro:911report dom$ grep -l "sophisticated" *
```
```
chapter-3.txt
chapter-5.txt
chapter-8.txt
chapter-9.txt
preface.txt
```

Example 2
```
Steves-MacBook-Pro:911report dom$ grep -l "9/11" *
```
```
chapter-1.txt
chapter-10.txt
chapter-11.txt
chapter-12.txt
chapter-13.1.txt
chapter-13.2.txt
chapter-13.3.txt
chapter-13.4.txt
chapter-13.5.txt
chapter-2.txt
chapter-3.txt
chapter-5.txt
chapter-6.txt
chapter-7.txt
chapter-8.txt
chapter-9.txt
preface.txt
```
The grep -l command is an example of a useful command line option that prints out the names of the text files within the current directory that contain the string argument. This command is useful if trying to categorize files based on if they contain a particular string or not. 

---

### **Grep -c Command**

Example 1
```
Steves-MacBook-Pro:911report dom$ grep -c President chapter-10.txt
```
```
69
```

Example 2
```
Steves-MacBook-Pro:911report dom$ grep -c Marty chapter-13.3.txt
```
```
3
```
The grep -c command takes in a string argument and provides an integer output of the number of lines in a text file containing the string. This is also a useful command option because it's another way to categorize the prevalence of a string argument.

---

### **Grep -n Command**

Example 1
```
Steves-MacBook-Pro:911report dom$ grep -n "minutes" chapter-1.txt
```
```
18:    Atta and Omari arrived in Boston at 6:45. Seven minutes later, Atta apparently took a call from Marwan al Shehhi, a longtime colleague who was at another terminal at Logan Airport. They spoke for three minutes.
38:    Washington Dulles: American 77. Hundreds of miles southwest of Boston, at Dulles International Airport in the Virginia suburbs of Washington, D.C., five more men were preparing to take their early morning flight. At 7:15, a pair of them, Khalid al Mihdhar and Majed Moqed, checked in at the American Airlines ticket counter for Flight 77, bound for Los Angeles. Within the next 20 minutes, they would be followed by Hani Hanjour and two brothers, Nawaf al Hazmi and Salem al Hazmi.
48:    About 20 minutes later, at 7:35, another passenger for Flight 77, Hani Hanjour, placed two carry-on bags on the X-ray belt in the Main Terminal's west checkpoint, and proceeded, without alarm, through the metal detector. A short time later, Nawaf and Salem al Hazmi entered the same checkpoint. Salem al Hazmi cleared the metal detector and was permitted through; Nawaf al Hazmi set off the alarms for both the first and second metal detectors and was then hand-wanded before being passed. In addition, his over-the-shoulder carry-on bag was swiped by an explosive trace detector and then passed. The video footage indicates that he was carrying an unidentified item in his back pocket, clipped to its rim.
74:    About five minutes after the hijacking began, Betty Ong contacted the American Airlines Southeastern Reservations Office in Cary, North Carolina, via an AT&T airphone to report an emergency aboard the flight. This was the first of several occasions on 9/11 when flight attendants took action outside the scope of their training, which emphasized that in a hijacking, they were to communicate with the cockpit crew. The emergency call lasted approximately 25 minutes, as Ong calmly and professionally relayed information about events taking place aboard the airplane to authorities on the ground.
78:    At 8:21, one of the American employees receiving Ong's call in North Carolina, Nydia Gonzalez, alerted the American Airlines operations center in Fort Worth, Texas, reaching Craig Marquis, the manager on duty. Marquis soon realized this was an emergency and instructed the airline's dispatcher responsible for the flight to contact the cockpit. At 8:23, the dispatcher tried unsuccessfully to contact the aircraft. Six minutes later, the air traffic control specialist in American's operations center contacted the FAA's Boston Air Traffic Control Center about the flight. The center was already aware of the problem.
80:    Boston Center knew of a problem on the flight in part because just before 8:25 the hijackers had attempted to communicate with the passengers. The microphone was keyed, and immediately one of the hijackers said, "Nobody move. Everything will be okay. If you try to make any moves, you'll endanger yourself and the airplane. Just stay quiet." Air traffic controllers heard the transmission; Ong did not. The hijackers probably did not know how to operate the cockpit radio communication system correctly, and thus inadvertently broadcast their message over the air traffic control channel instead of the cabin public-address channel. Also at 8:25, and again at 8:29, Amy Sweeney got through to the American Flight Services Office in Boston but was cut off after she reported someone was hurt aboard the flight. Three minutes later, Sweeney was reconnected to the office and began relaying updates to the manager, Michael Woodward.
110:    Also at 8:52, a male flight attendant called a United office in San Francisco, reaching Marc Policastro. The flight attendant reported that the flight had been hijacked, both pilots had been killed, a flight attendant had been stabbed, and the hijackers were probably flying the plane. The call lasted about two minutes, after which Policastro and a colleague tried unsuccessfully to contact the flight.
128:    At 8:54, the aircraft deviated from its assigned course, turning south. Two minutes later the transponder was turned off and even primary radar contact with the aircraft was lost. The Indianapolis Air Traffic Control Center repeatedly tried and failed to contact the aircraft. American Airlines dispatchers also tried, without success.
150:    The hijackers had planned to take flights scheduled to depart at 7:45 (American 11), 8:00 (United 175 and United 93), and 8:10 (American 77). Three of the flights had actually taken off within 10 to 15 minutes of their planned departure times. United 93 would ordinarily have taken off about 15 minutes after pulling away from the gate. When it left the ground at 8:42, the flight was running more than 25 minutes late.
166:    By all accounts, the first 46 minutes of Flight 93's cross-country trip proceeded routinely. Radio communications from the plane were normal. Heading, speed, and altitude ran according to plan. At 9:24, Ballinger's warning to United 93 was received in the cockpit. Within two minutes, at 9:26, the pilot, Jason Dahl, responded with a note of puzzlement: "Ed, confirm latest mssg plz-Jason."
172:    The terrorists who hijacked three other commercial flights on 9/11 operated in five-man teams. They initiated their cockpit takeover within 30 minutes of takeoff. On Flight 93, however, the takeover took place 46 minutes after takeoff and there were only four hijackers. The operative likely intended to round out the team for this flight, Mohamed al Kahtani, had been refused entry by a suspicious immigration inspector at Florida's Orlando International Airport in August.
192:    One of the callers from United 93 also reported that he thought the hijackers might possess a gun. But none of the other callers reported the presence of a firearm. One recipient of a call from the aircraft recounted specifically asking her caller whether the hijackers had guns. The passenger replied that he did not see one. No evidence of firearms or of their identifiable remains was found at the aircraft's crash site, and the cockpit voice recorder gives no indication of a gun being fired or mentioned at any time. We believe that if the hijackers had possessed a gun, they would have used it in the flight's last minutes as the passengers fought back.
206:    The passengers continued their assault and at 10:02:23, a hijacker said, "Pull it down! Pull it down!"The hijackers remained at the controls but must have judged that the passengers were only seconds from overcoming them. The airplane headed down; the control wheel was turned hard to the right. The airplane rolled onto its back, and one of the hijackers began shouting "Allah is the greatest. Allah is the greatest." With the sounds of the passenger counterattack continuing, the aircraft plowed into an empty field in Shanksville, Pennsylvania, at 580 miles per hour, about 20 minutes' flying time from Washington, D.C.
226:    Before 9/11, it was not unheard of for a commercial aircraft to deviate slightly from its course, or for an FAA controller to lose radio contact with a pilot for a short period of time. A controller could also briefly lose a commercial aircraft's transponder signal, although this happened much less frequently. However, the simultaneous loss of radio and transponder signal would be a rare and alarming occurrence, and would normally indicate a catastrophic system failure or an aircraft crash. In all of these instances, the job of the controller was to reach out to the aircraft, the parent company of the aircraft, and other planes in the vicinity in an attempt to reestablish communications and set the aircraft back on course. Alarm bells would not start ringing until these efforts-which could take five minutes or more-were tried and had failed.
288:    In the succeeding minutes, controllers were attempting to ascertain the altitude of the southbound flight.
302:    F-15 fighters were scrambled at 8:46 from Otis Air Force Base. But NEADS did not know where to send the alert fighter aircraft, and the officer directing the fighters pressed for more information:"I don't know where I'm scrambling these guys to. I need a direction, a destination." Because the hijackers had turned off the plane's transponder, NEADS personnel spent the next minutes searching their radar scopes for the primary radar return. American 11 struck the NorthTower at 8:46. Shortly after 8:50, while NEADS personnel were still trying to locate the flight, word reached them that a plane had hit the World Trade Center. 
306:    In summary, NEADS received notice of the hijacking nine minutes before it struck the North Tower. That nine minutes' notice before impact was the most the military would receive of any of the four hijackings. 
320:    Minutes later, United 175 turned southwest without clearance from air traffic control. At 8:47, seconds after the impact of American 11, United 175's transponder code changed, and then changed again. These changes were not noticed for several minutes, however, because the same New York Center controller was assigned to both American 11 and United 175. The controller knew American 11 was hijacked; he was focused on searching for it after the aircraft disappeared at 8:46.
330:    Another commercial aircraft in the vicinity then radioed in with "reports over the radio of a commuter plane hitting the World Trade Center." The controller spent the next several minutes handing off the other flights on his scope to other controllers and moving aircraft out of the way of the unidentified aircraft (believed to be United 175) as it moved southwest and then turned northeast toward New York City.
376:    Within minutes of the second impact, Boston Center instructed its controllers to inform all aircraft in its airspace of the events in New York and to advise aircraft to heighten cockpit security. Boston Center asked the Herndon Command Center to issue a similar cockpit security alert nationwide. We have found no evidence to suggest that the Command Center acted on this request or issued any type of cockpit security alert.
388:    American Airlines Flight 77 FAA Awareness. American 77 began deviating from its flight plan at 8:54, with a slight turn toward the south. Two minutes later, it disappeared completely from radar at Indianapolis Center, which was controlling the flight.
396:    The failure to find a primary radar return for American 77 led us to investigate this issue further. Radar reconstructions performed after 9/11 reveal that FAA radar equipment tracked the flight from the moment its transponder was turned off at 8:56. But for 8 minutes and 13 seconds, between 8:56 and 9:05, this primary radar information on American 77 was not displayed to controllers at Indianapolis Center.
400:    According to the radar reconstruction, American 77 reemerged as a primary target on Indianapolis Center radar scopes at 9:05, east of its last known position. The target remained in Indianapolis Center's airspace for another six minutes, then crossed into the western portion of Washington Center's airspace at 9:10. As Indianapolis Center continued searching for the aircraft, two managers and the controller responsible for American 77 looked to the west and southwest along the flight's projected path, not east-where the aircraft was now heading. Managers did not instruct other controllers at Indianapolis Center to turn on their primary radar coverage to join in the search for American 77.
402:    In sum, Indianapolis Center never saw Flight 77 turn around. By the time it reappeared in primary radar coverage, controllers had either stopped looking for the aircraft because they thought it had crashed or were looking toward the west. Although the Command Center learned Flight 77 was missing, neither it nor FAA headquarters issued an all points bulletin to surrounding centers to search for primary radar targets. American 77 traveled undetected for 36 minutes on a course heading due east for Washington, D.C.
454:    United Airlines Flight 93 FAA Awareness. At 9:27, after having been in the air for 45 minutes, United 93 acknowledged a transmission from the Cleveland Center controller. This was the last normal contact the FAA had with the flight.
476:    At 9:46 the Command Center updated FAA headquarters that United 93 was now "twenty-nine minutes out of Washington, D.C." At 9:49, 13 minutes after Cleveland Center had asked about getting military help, the Command Center suggested that someone at headquarters should decide whether to request military assistance: FAA Headquarters: They're pulling Jeff away to go talk about United 93.
482:    Command Center: Uh, that's a decision somebody's gonna have to make probably in the next ten minutes.
490:    Five minutes later, the Command Center forwarded this update to headquarters: Command Center: O.K. Uh, there is now on that United 93.
502:    The aircraft that spotted the "black smoke" was the same unarmed Air National Guard cargo plane that had seen American 77 crash into the Pentagon 27 minutes earlier. It had resumed its flight to Minnesota and saw the smoke from the crash of United 93, less than two minutes after the plane went down. At 10:17, the Command Center advised headquarters of its conclusion that United 93 had indeed crashed.
534:    The defense of U.S. airspace on 9/11 was not conducted in accord with preexisting training and protocols. It was improvised by civilians who had never handled a hijacked aircraft that attempted to disappear, and by a military unprepared for the transformation of commercial aircraft into weapons of mass destruction. As it turned out, the NEADS air defenders had nine minutes' notice on the first hijacked plane, no advance notice on the second, no advance notice on the third, and no advance notice on the fourth.
546:    In fact, not only was the scramble prompted by the mistaken information about American 11, but NEADS never received notice that American 77 was hijacked. It was notified at 9:34 that American 77 was lost. Then, minutes later, NEADS was told that an unknown plane was 6 miles southwest of the White House. Only then did the already scrambled airplanes start moving directly toward Washington, D.C.
548:    Thus the military did not have 14 minutes to respond to American 77, as testimony to the Commission in May 2003 suggested. It had at most one or two minutes to react to the unidentified plane approaching Washington, and the fighters were in the wrong place to be able to help. They had been responding to a report about an aircraft that did not exist.
550:    Nor did the military have 47 minutes to respond to United 93, as would be implied by the account that it received notice of the flight's hijacking at 9:16. By the time the military learned about the flight, it had crashed. We now turn to the role of national leadership in the events that morning.
598:    We found no evidence that, at this critical time, NORAD's top commanders, in Florida or Cheyenne Mountain, coordinated with their counterparts at FAA headquarters to improve awareness and organize a common response. Lower-level officials improvised-for example, the FAA's Boston Center bypassed the chain of command and directly contacted NEADS after the first hijacking. But the highest-level Defense Department officials relied on the NMCC's air threat conference, in which the FAA did not participate for the first 48 minutes.
602:    At 9:44, NORAD briefed the conference on the possible hijacking of Delta 1989. Two minutes later, staff reported that they were still trying to locate Secretary Rumsfeld and Vice Chairman Myers. The Vice Chairman joined the conference shortly before 10:00; the Secretary, shortly before 10:30. The Chairman was out of the country.
612:    The President remained in the classroom for another five to seven minutes,
636:    The Vice President's military aide told us he believed the Vice President spoke to the President just after entering the conference room, but he did not hear what they said. Rice, who entered the room shortly after the Vice President and sat next to him, remembered hearing him inform the President, "Sir, the CAPs are up. Sir, they're going to want to know what to do." Then she recalled hearing him say, "Yes sir." She believed this conversation occurred a few minutes, perhaps five, after they entered the conference room.
646:    His reaction was described by Scooter Libby as quick and decisive, "in about the time it takes a batter to decide to swing." The Vice President authorized fighter aircraft to engage the inbound plane. He told us he based this authorization on his earlier conversation with the President. The military aide returned a few minutes later, probably between 10:12 and 10:18, and said the aircraft was 60 miles out. He again asked for authorization to engage. The Vice President again said yes.
710:    NORAD officials have maintained consistently that had the passengers not caused United 93 to crash, the military would have prevented it from reaching Washington, D.C. That conclusion is based on a version of events that we now know is incorrect. The Langley fighters were not scrambled in response to United 93; NORAD did not have 47 minutes to intercept the flight; NORAD did not even know the plane was hijacked until after it had crashed. It is appropriate, therefore, to reconsider whether United 93 would have been intercepted.
712:    Had it not crashed in Pennsylvania at 10:03, we estimate that United 93 could not have reached Washington any earlier than 10:13, and probably would have arrived before 10:23. There was only one set of fighters circling Washington during that time frame-the Langley F-16s. They were armed and under NORAD's control. After NEADS learned of the hijacking at 10:07, NORAD would have had from 6 to 16 minutes to locate the flight, receive authorization to shoot it down, and communicate the order to the pilots, who (in the same span) would have had to authenticate the order, intercept the flight, and execute the order.
```

Example 2
```
Steves-MacBook-Pro:911report dom$ grep -n "WARTIME" chapter-10.txt
```
```
4:            WARTIME
```
The grep -n command takes in a string and text file and prints the lines in the text file, as well as the number of the line, that contains the string argument. To get a detailed look of the text file and the amount of times a string appears, then the grep -n command can provide some use.

---

### **Grep -i Command**

Example 1
```
Steves-MacBook-Pro:911report dom$ grep -i government chapter-3.txt
```
```
                evolution of government efforts to counter terrorism by Islamic extremists against
            We mention many personalities in this report. As in any study of the U.S. government,
                response. Government agencies swung into action to find the culprits. The
                an official in the government of Qatar probably warned him about it. Khalid Sheikh
                government's attorneys stressed the seriousness of the crimes, and put forward
                Initial evidence pointed to the government of Syria and, later, Iran. The
                government. Eventually Libya acknowledged its responsibility.
                suspects (including 9/11 mastermind Khalid Sheikh Mohammed), even though government
                employed to stop prohibited items. Numerous government reports indicated that
                waxed and waned over the years, and to others in government, especially the
                breaks codes. The NSA also creates codes and ciphers to protect government
                and maintains in orbit information-gathering satellites that serve other government
                communications often set off alarms elsewhere in the government. Often, too, its
                electronic systems, like email, to other agencies of the U.S. government.
                either were sponsored by governments or, like the Palestine Liberation Organization,
                were militants trying to create governments.
                found host governments not only making connections with the U.S. government through
                governments presumed to be behind the terrorists. Moreover, since terrorist
                implementation among government agencies. The prolonged crisis of 1979-1981, when 53
                foreign policy aims of the U.S. government.
                of the U.S. government, some coordinating mechanism is necessary. When terrorism was
                efforts to achieve cooperation of other governments" and the CIA to "intensify use
                and the bombers proved to be American antigovernment extremists named Timothy Mc
                foreign policy and national security community both in and out of government. While
                the most representative branch of the federal government, Congress closely tracks
                is not a natural locus for program management. Hence, government efforts to cope
                against Bin Ladin Until 1996, hardly anyone in the U.S. government understood that
                learned that Sudanese officials were discussing with the Saudi government the
                South Asia was seen in the department and the government generally as a low
                government in May 1998 were made, as Berger has put RESPONSES TO AL QAEDA'S INITIAL
                learned in the spring of 1998 that the Saudi government had quietly disrupted Bin
                table, despite a consensus that the [government] ought to pursue every avenue it can
                and synthesized for the rest of the government. Indeed, analysts in the unit felt
            Therefore, the government experts who believed that Bin Ladin and his network posed
                1998, the U.S. government also was worrying about the deployment of military power
                government. Riyadh then suspended its diplomatic relations with the Taliban regime.
                recognized the Taliban as the legitimate government of Afghanistan.) Crown Prince
                Washington in late September. His account confirmed reports that the U.S. government
            Other efforts with the Saudi government centered on improving intelligence sharing
                detained by the Saudi government in 1997.67Though U.S. officials repeatedly raised
                with Crown Prince Abdullah, Vice President Gore, while thanking the Saudi government
            The Saudi government, which had a long and close relationship with Pakistan and
                war and install a national unity government. The second, favored by Sheehan, Clarke,
                of whether to recognize the Taliban as Afghanistan's government). Sheehan and Clarke
                government might use Bin Ladin to buy concessions from Washington, but neither side
                with the government of Iraq that al Qaeda would not work against that government and
                would work cooperatively with the Government of Iraq."
                Brief describing intelligence, received from a friendly government, about a
                officials throughout the government describing reports that Bin Ladin planned to
                if they killed him. Officials throughout the government approved this draft. But on
                because these countries had dictatorial governments.
                Bin Ladin's network and to hit Taliban government sites as well. General Shelton
                June, the U.S. government received a flurry of ominous reports, including more
                diplomatic options practically exhausted by the summer of 1999, the U.S. government
            In July 1999, President Clinton authorized the CIA to work with several governments
```

Example 2
```
Steves-MacBook-Pro:911report dom$ grep -i north chapter-13.2.txt
```
```
                Accounting Office; INS-Immigration and Naturalization Service; NEADS-Northeast Air
                derived by the Commission from files provided by the FAA and the Northeast Air
                missions" of NORAD were "aerospace warning" and "aerospace control" for North
                space and the detection, validation, and warning of attack against North America
                northeast bound and descending out of twelve thousand nine hundred feet in a rapid
```    
The grep -i command takes a string and text file argument and its output are all the lines that contain the string, not case-sensitive. This is important because if a string of interest is likely to be written in both lower and upper case, then using grep -i is helpful.

---

**Note**: For each of the 4 grep command line options, I used the site [https://www.geeksforgeeks.org/grep-command-in-unixlinux/](https://www.geeksforgeeks.org/grep-command-in-unixlinux/) as my source for understanding the idea behind each grep option.
