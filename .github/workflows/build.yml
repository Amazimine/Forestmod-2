name: Build Mod

on:
  push:
    branches: [ "main", "master" ]
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Set up Java 21
        uses: actions/setup-java@v4
        with:
          java-version: '21'
          distribution: 'temurin'

      - name: Setup Gradle
        uses: gradle/actions/setup-gradle@v3

      - name: Grant execute permission to gradlew
        run: chmod +x gradlew

      - name: Build mod
        run: ./gradlew build

      - name: Upload JAR
        uses: actions/upload-artifact@v4
        with:
          name: forestmod-jar
          path: build/libs/forestmod-*.jar
          if-no-files-found: error
