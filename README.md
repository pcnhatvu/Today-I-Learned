# Today-I-Learned

##### 26/09/2022: Collection.stream().forEach() and Collection.forEach()
```
- The first difference between them is Execution Order. Collection.forEach() processed in order of the items. 
  In constract, the processing order of Collection.stream().forEach() is undefined. 
- The second thing is Modification. Collection.forEach() throws an exception immediately after removing an element. 
  In constrast, Collection.stream().forEach() continues interating over the whole list before see an exception. 
  In case of modifying, there is no problem with doing this using either Collection.stream().forEach() or Collection.forEach(), 
  but we shouldn't do this because the stream should facilitate parallel execution. 
  So, modifying elements of a stream could lead to unexpected behavior.
- Conclution: if we don't require a stream but only want to iterate over a collection, 
  the first choice should be using Collection.forEach() directly on the collection.
```
##### 27/09/2022: What is gRPC?
```

```
##### 29/09/2022: Why do we need api gate-way?
```

```
##### 30/09/2022: What is redis cache, spring cache?
```

```
##### 01/10/2022: group by, having in SQL?
```

```
##### 02/10/2022: How to check null in Java?
```

```
##### 03/10/2022: Serializable in Java?
```

```
##### 04/10/2022: ```&``` and ```&&``` in Java
```

```
##### 09/10/2022: What is rebase in git?
```

```
##### 10/10/2022: Integer.toString() vs String.valueOf() in Java
```

```
##### 17/10/2022: What is BindingResult in Spring?
```

```
