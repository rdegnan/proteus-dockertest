# proteus-dockertest

## Publishing Containers to DockerHub
Follow the steps below to publish new dockertest containers to DockerHub:

1. Add a `gradle-local.properties` file to the root project.

    The gradle-local.properties file is a user-specific Gradle configuration file
    that will contain your DockerHub credentials.
    
2. Add your DockerHub credentials to the `gradle-local.properties` file as follows:

        dockerUsername={username}
        dockerPassword={password}
        
3. Run the following Gradle command:

        $ ./gradlew clean build pushImage

## License
Copyright 2018 Greg Whitaker

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.