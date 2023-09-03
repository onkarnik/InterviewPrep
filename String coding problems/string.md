# Master String coding problems

- [markup guide](https://www.markdownguide.org/cheat-sheet/)

---

<br/>

## Tips

<br/>

### 1. Use integer array to map characters

```java
mark[s.charAt(i)] //valid in java

mark[s.charAt(i)-'a'] // marking lower case letters
```

<br/>

### 2. Use **Hashmap<Character, Integer>** to store unique letters or mark repeating letters

```java
            if(!map.containsKey(ch)){
                map.put(ch,1);
            }
            else{
                int val = map.get(ch);
                map.put(ch,++val);
            }
```

<br/>

### 3. Learn how to use **_StringBuilder_**

```java
   //methods of StringBuilder class
   StringBuilder sb = new StringBuilder();

   sb.append();
   sb.reverse();
   sb.toString();
```

**Advantages of using sb class**

- String is **_immutable_**. we cannot modify string. when we modify or use concat method we simply get new string literal in memory.
- Using StringBuilder over normal string if you want to modify string is always better and gives good time complexity.
- some problems require use of **_StringBuiler_** class. normal string class in that problem would increase running time by a lot.

<br/>

---

## Most frquently asked string based questions

1. [**Non Repeating Character**(gfg)](https://practice.geeksforgeeks.org/batch/dsa-4/track/DSASP-Strings/problem/non-repeating-character-1587115620)

- Given a string S consisting of lowercase Latin Letters. Return the first non-repeating character in S. If there is no non-repeating character, return '$'.

2. [**Anagram**(gfg)](https://practice.geeksforgeeks.org/batch/dsa-4/track/DSASP-Strings/problem/anagram-1587115620)

- Given two strings a and b consisting of lowercase characters. The task is to check whether two given strings are an anagram of each other or not. An anagram of a string is another string that contains the same characters, only the order of characters can be different. For example, act and tac are an anagram of each other.
