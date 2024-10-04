# Java JSON
| Metrics | Workflows |
| -------- | ------- |
| ![Metrics](https://raw.githubusercontent.com/iahmadgad/iahmadgad-metrics/refs/heads/main/json-java-metrics.svg) | [![Gradle Java CI](https://github.com/iahmadgad/json-java/actions/workflows/gradle.yml/badge.svg)](https://github.com/iahmadgad/json-java/actions/workflows/gradle.yml) |

Java implementation of JSON.

A beginner project that I am proud of, because I worked hard on it.

I aim to enhance it further & further إن شاء الله, but when I finish this year, my last year in school :')
# Features
- Read JSON strings & files.
- Generate JSON strings.
- Convert JSON objects to Java objects & vice versa.
- Acsess JSON fields using JSON pointers.
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
The file should like like this:
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
