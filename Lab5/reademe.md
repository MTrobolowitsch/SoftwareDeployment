# Team Mitglieder
- Manuel Trobolowitsch

## Release Approvement

Es wurde eine simple Node.JS Express Web App erstellt und mit einem Test (mochaJS) ausgestattet,welcher den REST Call testet.

Die Pipelines auf DevOps wurden so eingerichtet, dass nach jedem Commit automatisch versucht wird zu builden und anschließend zu deployen. 
Sollte dies erfolgreich sein wird automatisch dieRelease Pipeline getriggered.


## Commit Approval
Ein Commit braucht ein Approval von mir um danach gebuildet und deployed zu werden.
Siehe Screenshot ("AutomatedTriggerAndApproval")
Bei einem Commit wird der Container Container gebuildet und in den Registry gepusht.
Danach wird der Container gepullt und das Image mittels AKS gestartet.

### Dockerfile
Dockerfile ist anbei zu finden, welches das für das kleine nodejs programm aus Lab2 gemacht wurde.
Link zum deployten Container: http://20.73.37.199/
