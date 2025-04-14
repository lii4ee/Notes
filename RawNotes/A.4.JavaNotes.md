### Iterating through a map
```
for(Map.Entry<Integer, String> i: map.entrySet())
        {
            System.out.println("Key :" + i.getKey() + ", Value :"+ i.getValue());
        }
```

```
    Iterator <Map.Entry<Integer, String>> iterator = map.entrySet().iterator();
        while(iterator.hasNext()){
            Map.Entry<Integer, String> entry = iterator.next();
            System.out.println(entry.getKey() + " " + entry.getValue());
        }
```

```
map.forEach((k , v) -> System.out.println(k + " :: " +v));
```

```
    map.entrySet()
        .stream()
        .forEach(
            entry -> System.out.println(entry.getKey() + " :::: " + entry.getValue())
        );
```