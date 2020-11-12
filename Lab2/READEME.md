# Release Approvement
Es wurde eine simple Node.JS Express Web App erstellt und mit einem Test (mochaJS) ausgestattet,
welcher den REST Call testet.
Es wurden 2 App Services auf Azure erstellt, einmal für Dev und einmal für Production.
Die Pipelines auf DevOps wurden so eingerichtet, dass nach jedem Commit automatisch versucht
wird zu builden und anschließend zu deployen (Dev). Sollte dies erfolgreich sein wird automatisch die
Release Pipeline getriggered.
Release ist abgeschlossen und auf der zugehören URL erreichbar (Prod).