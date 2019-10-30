# Sonar Scanner

This repository contains the definition of the docker images to use sonar scanner in our CI system.
Each Docker contains the latest sonar scanner cli version with its dependencies (java) and the language runtime
we want to scan.

Sonar scanner works in a different way for some languages but here you can find some examples:


[How to use sonar scanner with a dotnet project](dotnet/README.md)

[How to use sonar scanner with a node project](node/README.md)
