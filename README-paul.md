# Instructions for working on dart-autodata

## Checking out dart-autodata branch

    git clone git@github.com:pauldemarco/openapi-generator
    cd openapi-generator
    git checkout dart-autodata

## Pertinent file locations

    * DartAutodataClientCodegen - ./modules/openapi-generator/src/main/java/org/openapitools/codegen/languages/
    * *.mustache - ./modules/openapi-generator/src/main/resources/dart-autodata

## Build CLI

    mvn clean package -DskipTests

## Run generator

    java -jar ~/openapi-generator/modules/openapi-generator-cli/target/openapi-generator-cli.jar generate -g dart-autodata -i spec2.yaml -o out