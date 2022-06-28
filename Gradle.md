## Gradle core concepts
- **Project** : Dai dien cho nhung viec can hoan thanh, vi du nhu trien khai du an
- **Gradle project** yeu cau 1 tap hop nhung task can de thuc thi.
- **task** : de cap den nhung viec duoc thuc hien boi 1 build. No co the la compiling source, create JAR file, tao Javadoc
- **Build Scripts** : no chinh la build.gradle va nam o thu muc goc cua file project
- 


- `settings.gradle` : setting of high level configurations of project
- `rootProject.name = 'tenProject'` : khai bao ten project
- `build.gradle` : build script configuration file, descriping application for gradle => so that gradle can buid it.
- gradlew va gradlew.bat: gradle wrapper script
- gradlew : is used for mac and linux
- gradlew.bat : is used for windows

#### Projects, build script, tasks, plugin:
- project : is highest level so that gradle know about our application, 
- Build script : each project can have `build script `, in this file we tell gradle about configuration of configuration
- Build sript containt 1 or more task 
- Groovy : use JVM to run

## Gradle Command

- `gradle tasks` : Hien list task trong project
- `gradle clean` : ...
- `gradle clean build` : ...
- `gradle clean build --info` : ...

## Gradle project in Eclipse

- 


