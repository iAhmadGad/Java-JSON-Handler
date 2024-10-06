# Java JSON
[![Gradle](https://github.com/iahmadgad/json-java/actions/workflows/gradle.yml/badge.svg)](https://github.com/iahmadgad/json-java/actions/workflows/gradle.yml)
<details>
     <summary><img src="https://img.shields.io/badge/json--java-metrics-blue" alt="Metrics"></summary>
     <img src="https://raw.githubusercontent.com/iahmadgad/iahmadgad/refs/heads/metrics/json-java.metrics.svg" alt="Metrics">     
</details>

Java implementation of JSON.

A beginner project that I am proud of, because I worked hard on it.

I aim to enhance it further & further إن شاء الله, but when I finish this year, my last year in school :')
# Features
- Read JSON strings & files.
- Generate JSON strings & write them into files.
- Convert JSON objects to Java objects & vice versa.
- Access JSON fields using JSON pointers.
- supports nested JSON objects & arrays.
# Examples
## Initialise a new JSON object
```java
JSONObject obj = new JSONObject();
obj.put("$id", "User-info");
obj.put("name", "Gelobt");
obj.put("age", 16);
obj.put("isAlive", true);
```
## Initialise a new JSON array
```java
JSONArray arr = new JSONArray();
arr.add("Java");
arr.add("C++");
arr.add("Cats");
```
## Put JSON array into JSON object
```java
obj.put("THINGS I LOVE", arr);
```
## Write JSON object into file
```java
obj.write(new File("User-info.json"));
```
The file should look like this:
```json
{
     "isAlive":true
     ,"name":"Gelobt"
     ,"THINGS I LOVE":     [
          "Java"
          ,"C++"
          ,"Cats"
     ]

     ,"age":16
     ,"$id":"User-info"
}
```
