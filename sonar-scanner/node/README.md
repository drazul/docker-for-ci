# Usage

```
cat << EOF > sonar-project.properties
sonar.host.url=${SONAR_HOST}
sonar.login=${SONAR_TOKEN}
sonar.projectKey=${PROJECT_KEY}
sonar.projectName=${PROJECT_KEY}
sonar.projectVersion=${changeset}
sonar.sourceEncoding=UTF-8
sonar.sources=src
sonar.exclusions=**/node_modules/**,**/*.spec.ts
sonar.tests=src
sonar.test.inclusions=**/*.spec.ts
sonar.typescript.lcov.reportPaths=coverage/lcov.info
EOF

sonar-scanner
```

