# Before Spring Security Dependency

1. Created a Spring app with Spring Initializr.
2. Added the Spring Boot Starter Web. Spring Boot Starter Test comes automatically. See `build.gradle`.
3. Create a `@RestController` - `HomeResource.java`
4. Build and run. `./gradlew build bootrun`
5. Go to `localhost:8080` in a web browser.
6. Notice no authentication is required to view the page.

# After Spring Security Dependency

1. In `gradle.build` add Spring Boot Starter Security.
2. Build and run. `./gradlew build bootrun`
3. Go to `localhost:8080` in a web browser.
4. See the redirect to a form login page.
5. Notice in the Spring log output shows a DefaultSecurityFilterChain was added. A generated 
