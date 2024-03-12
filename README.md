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
3. Deploy the file in `build/libs/app.jar` to the target machine
4. Now you can run this jar file to any machine which has the same version of JRE: java -jar <your_path_to_jar_file>