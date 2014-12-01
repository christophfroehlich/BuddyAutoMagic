# Requirements for mail
Assignment emails will be sent via the Gmail account who is owner of the BuddyAutoMagic - google-document.
There have to be two drafts in the Gmail-account with the following subjects:
- Local Buddy Assignment
- Exchange Buddy Assignment
(cf. buddyAutoMagic.gs: function sendOutAssignmentEmails(outMail, debug) {} )
``` javascript
var localMessage = getGmailDraftBySubject("Local Buddy Assignment");
var exchangeMessage = getGmailDraftBySubject("Exchange Buddy Assignment");
```

# Variable names
these is a (maybe uncomplete list) of possible variable names:
- ${"Affinity"}
- ${"Local name"}
- ${"Exchange name"}
- ${"Local ID"}
- ${"Exchange ID"}
- ${"Email sent"}
- ${"Force Match"}
- ${"Gender Score"}
- ${"Gender Preference"}
- ${"Exchange Gender"}
- ${"Age Score"}
- ${"Age difference"}
- ${"Local Age"}
- ${"Exchange Age"}
- ${"Country pref Score"}
- ${"Exchange Nationality"}
- ${"Pref 1"}
- ${"Pref 2"}
- ${"Pref 3"}
- ${"Study Level Score"}
- ${"Local level"}
- ${"Exchange level"}
- ${"Faculty Score"}
- ${"Local faculty"}
- ${"Exchange faculty"}
- ${"Languages Score"}
- ${"Languages in common"}
- ${"Interests Score"}
- ${"Interests in common (both love)"}
- ${"Motivation Score"}
- ${"Motivation"}
- ${"Arrival time Score"}
- ${"Arrives on"}
- ${"Willingness Score"}
- ${"Would you be interested in having more than one buddy?"}
- ${"Appendix Score"}
- ${"Local Email"}
- ${"Exchange Email"}
- ${"Local Facebook"}
- ${"Exchange Facebook"}
- ${"Local Phone"}
- ${"Exchange Phone"}
- ${“heshe”} ← wird automatisch mit dem geschlechtsentsprechenden Wort ersetzt falls das geschlecht angegeben wurde.
