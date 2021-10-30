# Topic

## Pain vs. Suffering :
Learning  is great, but it does come at a price which is **`Pain`**(the pain of growth).

But this **`Pain`** is for higher purpose and ambition, so *`Pain`* also the ways in which you grow.

In other hand there is **`Suffering`** it has the same meaning as **`Pain`** but what is the difference ?

**`Suffering`** is *`pain`* without purpose. *`Pain`* with no higher goal. *`Pain`* with no dreams, no ambition, no aspiration.

![Pain vs. Suffering](https://excellentjourney.files.wordpress.com/2015/07/screen-shot-2015-07-29-at-4-23-55-pm.png)

As you work through feeling the pain of growth consider heavily the story that you attach to it:

    1. What’s your perspective?
    2. Why are you doing this?
    3. Do you want what comes at the end of this journey?
    4. Are you doing this for you?

## Beginners Guide to Big O :

![Big O](https://www.educative.io/v2api/editorpage/5870871921033216/image/6036875259150336)

**`Big O`** notation is used in Computer Science to describe the performance or complexity of an algorithm.

The best way to understand **`Big O`** is to produce some examples in code, so let's start with our first example:

1. **`O(1)`** :
    * *`O(1)`* describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

    ```
    bool IsFirstElementNull(IList<String> elements)
    {
    return elements[0] == null;
    }
    ```

2. **`O(N)`** :
    * *`O(N)`* describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.

    ```
    bool ContainsValue(IEnumerable<string> elements, string value)
    {
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
    }
    ```
3. **`O(N²)`** :
    * *`O(N²)`* represents an algorithm whose performance is directly proportional to the square of the size of the input data set.

    ```
    bool ContainsDuplicates(IList<string> elements)
    {
    for (var outer = 0; outer < elements.Count; outer++) 
    {
        for (var inner = 0; inner < elements.Count; inner++) 
        { 
            // Don't compare with self 
            if (outer == inner) continue;             
            
            if (elements[outer] == elements[inner]) return true; 
        }
    }    
    return false;
    }
    ```
4. **`O(2^N)`** :
    * *`O(2^N)`* denotes an algorithm whose growth doubles with each addition to the input data set.

    ```
    int Fibonacci(int number)
    {
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
    }
    ```
5. **`Logarithms`** :
    * *`Logarithmic`* running time ( O(log n) ) essentially means that the running time grows in proportion to the *`logarithm`* of the input size.

    `As an example`, if 10 items takes at most some amount of time `x`, and 100 items takes at most, say, `2x`, and 10,000 items takes at most `4x`, then it's looking like an `O(log N)` time complexity.