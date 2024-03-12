# Java Project Demo with Gradle
## Development
1. Create project: gradle init --type java-application
2. Build: ./gradlew build
3. Run: ./gradlew run

## Deployment
1. Add to the file `build.gradle`
jar {
    manifest {
        attributes 'Main-Class': 'org.example.App'
    }
}
2. Create jar file: ./gradlew jar
3. Deploy the file in `build/libs/app.jar`
4. Make sure the jave version in `build.gradle` and the JRE version in the deployed machine are matched.