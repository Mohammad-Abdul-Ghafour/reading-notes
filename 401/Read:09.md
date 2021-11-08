# Game of Greed 4
## Dunder Methods :

Methods that have two prefix and suffix underscores in the method name called **`Dunder Methods`**.

Dunder here means *`Double Under (Underscores)`*

These are commonly used for operator overloading, they are a set of predefined methods you can use to enrich your classes.

for example **`__init__`** or **`__str__`**.

### Why do we need Dunder methods ?
Consider a case where we have the following class:

```python
class point:
    x = 4
    y = 5

p1 = point()
print(p1)
```

> The print statement would print something like *`<__main__.point object at 0x7fb992998d00>`*

But, we might want the print statement to display something.

We can achieve this by overriding the __str__ method of our class and We could also override other methods such as the *`len`*, *`+`*, *`[]`* etc.

```python
class point:
    x = 4
    y = 5
    def __str__():
        return x+y

p1 = point()
print(p1)
```

This will print *`9`*.

And there are a lot of **`Dunder Methods`** to take a look at :

1. **`Initialization Methods`** :

![Initialization Methods](https://miro.medium.com/max/1400/1*sWthu_8-6_R-d_AeLToTrQ.png)

2. **`Representation Methods`** :

![Representation Methods](https://miro.medium.com/max/1400/1*fD16vt088LbTFaO_qo_XVA.png)

3. **`Rich comparison Methods`** :

![Rich comparison Methods](https://miro.medium.com/max/1400/1*7eglYMfJEwMo4qbil2O28g.png)

4. **`Attribute access Methods`** :

![Attribute access Methods](https://miro.medium.com/max/1400/1*7FVfTZh0IPIFZ_a8xuthVQ.png)

5. **`Descriptors Methods`** :

![Descriptors Methods](https://miro.medium.com/max/1400/1*912cNPioQyMLETwHnY3MNQ.png)

6. **`Container Methods`** :

![Container Methods](https://miro.medium.com/max/1400/1*4eRv5XKxVQtvDEXAZAaWLw.png)

7. **`Numeric operations Methods`** :

![Numeric operations Methods](https://miro.medium.com/max/1400/1*hyM-aAqna9iOWTHuWjq4-A.png)

## Statistics - Probability :

**`Probability`** is the chance of an event happening.

To calculate the chance of an event happening, we also need to consider all the other events that can occur.

**`Statistics`** enables us to calculate **`probabilities`** using real-world observations. **`Probability`** provides the theory, while **`statistics`** provides the tools to test that theory using data.

The descriptive statistics, specifically mean and standard deviation, become the proxies for the theoretical.

> Why would I need a proxy if I can just calculate the theoretical probability itself >

What is the probability that a critical car component will fail when you are driving ?

There are no easy ways to calculate probabilities, so we must fall back on using data and statistics to calculate them.

Given more and more data, we can become more confident that what we calculate represents the true probability of these important events happening.

![](https://miro.medium.com/max/1400/1*NmJZoHXjg52jmb9_nQlOXg.jpeg)