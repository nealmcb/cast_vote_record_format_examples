# cast_vote_record_format_examples
Collection of examples of CVR (cast vote record) examples from a variety of election system vendors

TODO:

* ES&S:

```
Cast Vote Record,Precinct,Ballot Style,Proposition BB (STATUTORY),CRIPPLE CREEK MAYOR CRIPPLE CREEK,CRIPPLE CREEK COUNCIL WARD 4 CC 
WARD 4,CRIPPLE CREEK COUNCIL WARD 5 CC WARD 5,VICTOR CITY COUNCIL WARD 1,VICTOR CITY COUNCIL WARD 2,Referred Issue 2A,Referred Issue
 2B,BALLOT ISSUE 4A: UTE PASS
12,1_STATE,1_STATE,NO / AGAINST,,,,,,,,
13,4_VICW1,4_VICW1,YES / FOR,,,,Tarla Perdew,,YES / FOR,YES / FOR,
14,3_CCW5,3_CCW5,NO / AGAINST,Bruce Brown,,Chris Hazlett,,,,,
15,6_UTE,6_UTE,NO / AGAINST,,,,,,,,YES / FOR
16,2_CCW4,2_CCW4,NO / AGAINST,Bruce Brown,Thomas L. Litherland,,,,,,
```

* OpenCount: One column with ballot id (full path name....), then one for each choice in a contrest with "0" or "1" , then one to summarize validity of ballot for that contest: OK / UNDERVOTED / OVERVOTED

```
#path,US House District 1:Martin Walsh,US House District 1:Write-In,US House District 1,State Representative District 36:Richard Bowman,State Representative District 36,County Clerk:Matt Crane,County Clerk,Governor:Mike Kopp,Governor:Scott Gessler,Governor:Tom Tancredo,Governor:Bob Beauprez,Governor,US House District 4:Scott Renfroe
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000001_side0.jpg,1,0,OK,1,OK,0,1,OK,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000002_side0.jpg,UNDERVOTED,1,OK,1,0,OK,,,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000003_side0.jpg,1,0,OK,1,OK,1,0,OK,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000004_side0.jpg,OK,1,OK,1,OK,,,,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000005_side0.jpg,OK,1,OK,1,OK,,,,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000006_side0.jpg,OK,1,OK,0,UNDERVOTED,,,,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000007_side0.jpg,0,1,OK,1,OK,1,OK,,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000008_side0.jpg,0,1,OK,1,OK,1,0,OK,,,,,
/home/opencount/Desktop/ALL_Ballots_wider/Scanner1~000009_side0.jpg,1,OK,1,OK,,,,,,,,,

```


See also [NIST SP 1500\-102 Cast Vote Records Common Data Format Specification Draft Version 1\.0](https://pages.nist.gov/CastVoteRecords/) samples in XML and JSON format at 
[CDFPrototype: Prototypes based on NIST 1500 series CDFs](https://github.com/HiltonRoscoe/CDFPrototype)
