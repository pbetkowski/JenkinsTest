1. Zainstalować jenkinsa na localhost:port
2. Zainstalować Maven, dodać do zmiennych środowiskowych według dokumentacji
3. Zainstalować do Jenkinsa moduły Mavenowe
4. Do folderu z projektem powinny być dodane uprawnienia
5. Pom.xml musi zawierać plugin do generowania buildu i packaging
6. W jenkinsie jako opcję build wybrać Maven, dodać packaging i ścieżkę do pom.xml - $workspace\pom.xml


plugin:

<plugin><artifactId>maven-compiler-plugin</artifactId><version>3.1</version><configuration><fork>true</fork><executable>C:\Program Files\Java\jdk-11\bin\javac.exe</executable></configuration></plugin>