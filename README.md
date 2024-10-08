# Java JSON
[![Gradle](https://img.shields.io/github/actions/workflow/status/iahmadgad/json-java/gradle.yml?label=Gradle&logo=gradle)](https://github.com/iahmadgad/json-java/actions/workflows/gradle.yml)
[![Javadoc][Javadoc Badge]](https://github.com/iahmadgad/json-java/actions/workflows/javadoc.yml)
[![LICENSE](https://img.shields.io/github/license/iahmadgad/json-java.svg)](https://github.com/iahmadgad/json-java/blob/main/LICENSE)
<details>
     <summary><picture><img src="https://img.shields.io/badge/json--java-metrics-blue" alt="Metrics"></picture></summary>
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

<!---Variables go down there 👇-->
[Javadoc Badge]: https://img.shields.io/github/actions/workflow/status/iahmadgad/json-java/javadoc.yml?label=Javadoc&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSI2NCIgaGVpZ2h0PSI2NCIgdmlld0JveD0iMCAwIDMyIDMyIj48cGF0aCBkPSJNMTEuNjIyIDI0Ljc0cy0xLjIzLjc0OC44NTUuOTYyYzIuNTEuMzIgMy44NDcuMjY3IDYuNjI1LS4yNjdhMTAuMDIgMTAuMDIgMCAwIDAgMS43NjMuODU1Yy02LjI1IDIuNjcyLTE0LjE2LS4xNi05LjI0NC0xLjU1em0tLjgtMy40NzNzLTEuMzM2IDEuMDE1Ljc0OCAxLjIzYzIuNzI1LjI2NyA0Ljg2Mi4zMiA4LjU1LS40MjdhMy4yNiAzLjI2IDAgMCAwIDEuMjgyLjgwMWMtNy41MzQgMi4yNDQtMTUuOTc2LjIxNC0xMC41OC0xLjYwM3ptMTQuNzQ3IDYuMDlzLjkwOC43NDgtMS4wMTUgMS4zMzZjLTMuNTggMS4wNy0xNS4wMTQgMS4zOS0xOC4yMiAwLTEuMTIyLS40OCAxLjAxNS0xLjE3NSAxLjctMS4yODIuNjk1LS4xNiAxLjA3LS4xNiAxLjA3LS4xNi0xLjIzLS44NTUtOC4xNzUgMS43NjMtMy41MjYgMi41MSAxMi43NyAyLjA4NCAyMy4yOTYtLjkwOCAxOS45ODMtMi40MDR6TTEyLjIgMTcuNjMzcy01LjgyNCAxLjM5LTIuMDg0IDEuODdjMS42MDMuMjE0IDQuNzU1LjE2IDcuNjk0LS4wNTMgMi40MDQtLjIxNCA0LjgxLS42NCA0LjgxLS42NHMtLjg1NS4zNzQtMS40NDMuNzQ4Yy01LjkzIDEuNTUtMTcuMzEyLjg1NS0xNC4wNTItLjc0OCAyLjc3OC0xLjMzNiA1LjA3Ni0xLjE3NSA1LjA3Ni0xLjE3NXptMTAuNDIgNS44MjRjNS45ODQtMy4xIDMuMjA2LTYuMDkgMS4yODItNS43MTctLjQ4LjEwNy0uNjk1LjIxNC0uNjk1LjIxNHMuMTYtLjMyLjUzNC0uNDI3YzMuNzk0LTEuMzM2IDYuNzg2IDQuMDA3LTEuMjMgNi4wOSAwIDAgLjA1My0uMDUzLjEwNy0uMTZ6bS05LjgzIDguNDQyYzUuNzcuMzc0IDE0LjU4Ny0uMjE0IDE0LjgtMi45NCAwIDAtLjQyNyAxLjA3LTQuNzU1IDEuODctNC45MTYuOTA4LTExLjAwNy44LTE0LjU4Ny4yMTQgMCAwIC43NDguNjQgNC41NDIuODU1eiIgZmlsbD0iIzRlNzg5NiIvPjxwYXRoIGQ9Ik0xOC45OTYuMDAxczMuMzEzIDMuMzY2LTMuMTUyIDguNDQyYy01LjE4MyA0LjExNC0xLjE3NSA2LjQ2NSAwIDkuMTM3LTMuMDQ2LTIuNzI1LTUuMjM2LTUuMTMtMy43NC03LjM3M0MxNC4yOTQgNi44OTMgMjAuMzMyIDUuMyAxOC45OTYuMDAxem0tMS43IDE1LjMzNWMxLjU1IDEuNzYzLS40MjcgMy4zNjYtLjQyNyAzLjM2NnMzLjk1NC0yLjAzIDIuMTM3LTQuNTQyYy0xLjY1Ni0yLjQwNC0yLjk0LTMuNTggNC4wMDctNy41ODcgMCAwLTEwLjk1MyAyLjcyNS01LjcxNyA4Ljc2M3oiIGZpbGw9IiNmNTgyMTkiLz48L3N2Zz4=
