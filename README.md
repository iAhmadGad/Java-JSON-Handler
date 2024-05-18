<h1 align="center">Java JSON package</h1>

## Install:
- Download the latest [**release**](https://github.com/iAhmadGad/Java-JSON-Handler/releases).
- Add package to your build using command-line, or your IDE like Eclipse or Netbeans.
## How to use:
Here is an example on how to make a new JSON object:
```
JSONObject obj = new JSONObject();
obj.put("$id", "User-info");
obj.put("name", "Gelobt");
obj.put("age", 16);
obj.put("isAlive", true);
```
& here is an example on how to make a new JSON array:
```
JSONArray arr = new JSONArray();
arr.add("Java");
arr.add("C++");
arr.add("Cats");
```
then you can put this array in the JSON object you`ve just created:
```
obj.put("THINGS I LOVE", arr);
```
last but not least, write this JSON object in a JSON file:
```
obj.write(new File("User-info.json"));
```
& here is your JSON file:
```
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
## Repo Index:
- [**Source code**](https://github.com/iAhmadGad/Java-JSON-Handler/tree/main/src/dev/iahmadgad/json)
- [**Documentation**](https://github.com/iAhmadGad/Java-JSON-Handler/tree/main/docs)
## License:
- [**GPL-3.0**](https://github.com/iAhmadGad/Java-JSON-Handler/blob/main/LICENSE)
