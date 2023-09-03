# Master String coding problems

## Tips

### 1. Use integer array to map characters

```java
mark[s.charAt(i)] //valid in java

mark[s.charAt(i)-'a'] // marking lower case letters
```

### 2. Use Hashmap<Character, Integer> to store unique letters or mark repeating letters

```java
            if(!map.containsKey(ch)){
                map.put(ch,1);
            }
            else{
                int val = map.get(ch);
                map.put(ch,++val);
            }
```

## Most frquently asked string based questions

1. Non Repeating Character

- Given a string S consisting of lowercase Latin Letters. Return the first non-repeating character in S. If there is no non-repeating character, return '$'.

2. Anagram

- Given two strings a and b consisting of lowercase characters. The task is to check whether two given strings are an anagram of each other or not. An anagram of a string is another string that contains the same characters, only the order of characters can be different. For example, act and tac are an anagram of each other.
