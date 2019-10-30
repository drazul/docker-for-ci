# Usage

```
dotnet sonarscanner begin \
 /d:sonar.host.url=${SONAR_HOST} \
 /d:sonar.login=${SONAR_TOKEN} \
 /k:${PROJECT_KEY} \
 /n:${PROJECT_KEY} \
 /v:${changeset} \
 /d:sonar.exclusions=${exclusion_paths}

dotnet build --configuration Release
dotnet sonarscanner end /d:sonar.login=${SONAR_TOKEN}
```

