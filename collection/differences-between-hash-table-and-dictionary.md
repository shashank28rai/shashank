# Differences between Hash table and Dictionary

| **Dictionary** | **Hash table** |
| :--- | :--- |
| It returns error if we try to find a key which does not exist | It returns null if we try to find a key which does not exist. |
| It is faster than a Hashtable because there is no boxing and unboxing | It is slower than dictionary because it requires boxing and   unboxing. |
| Only public static members are thread safe | All the members in a Hashtable are thread safe, |
| Dictionary is a generic type which means we can use it with any data type. | Hashtable is not a generic type, |

## Dictionary Ex:-

Dictionary&lt;string, int&gt; dictionary = new Dictionary&lt;string, int&gt;\(\);

dictionary.Add\("cat", 2\);

dictionary.Add\("dog", 1\);

dictionary.Add\("llama", 0\);

dictionary.Add\("iguana", -1\);

## **Hash table** Ex:-

Hashtable hashtable = new Hashtable\(\);

hashtable.Add\("Area", 1000\);

hashtable.Add\("Perimeter", 55\);

hashtable.Add\("Mortgage", 540\);

