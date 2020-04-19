# Markdown

Press `Ctrl+Shift+V` on _Visual Studio_Code_ to open preview when you are on a `.md` file.


## Headings

```
# Heading h1
## Heading h2
### Heading h3
#### Heading h4
##### Heading h5
###### Heading h6
```

# Heading h1
## Heading h2
### Heading h3
#### Heading h4
##### Heading h5
###### Heading h6

## Text

```
I like _italic_ / I like *italic*

I like __bold__ / I like **bold**

~~I can erase it~~` => ~~I can erase it~~
```

I like _italic_ / I like *italic*

I like __bold__ / I like **bold**

~~I can erase it~~ => ~~I can erase it~~

## Line breaks

```
Using `<br>` tag:

Going to Thaïland.<br>
Going to Vietnam.<br>
```

Using `<br>` tag:

Going to Thaïland.<br>
Going to Vietnam.<br>

## Block Quotes

```
> Stuck at home !
```

> Stuck at home !

## Code Blocks

**Using indentation only:**

    const var = 'var';
    const number = 1;

**Using backticks:**

```
const hello = 'hello';
```

**Using backticks specifying language:**

```javascript
const var = 'var';
const number = 1;
```

```php
$var = 'var';
$number = 1;
echo $number
```
**Using backticks specifying diff:**

```diff
const value = 'value';
- const number = 1;
+ const number = 2;
```

## Lists

**Bullet:**

```
+ Zidane
```

+ Zidane

**Ordered:**

```
1. Ronaldo
1. Totti
1. Seedorf

```
1. Ronaldo
1. Totti
1. Seedorf

**Ordered with sub-items:** 

```
1. Ronaldo
    * Cristiano
        * Cristiano Ronaldo

        From: 

        ![Alternative Text][Img]

        Using `![Alternative Text][Img]`
1. Bergkamp
```
1. Ronaldo
    * Cristiano
        * Cristiano Ronaldo

        From: 

        ![Alternative Text][Img]

        Using `![Alternative Text][Img]`
1. Bergkamp

**Ordered with nested sub-items:** 

```
1. Ronaldo
    * Figo
        * Eusebio
        
1. Bergkamp
```
1. Ronaldo
    * Figo
        * Eusebio
        
1. Bergkamp


## Separators

 Using `---`:

---

## Tables

```
|Name | Club |
| :-- | :--- |
|Ronaldo|Juventus Turin|
|Pogba|Manchester United|
```

|Name | Club |
| :-- | :--- |
|Ronaldo|Juventus Turin|
|Pogba|Manchester United|

### Images

**With tooltip:**

```
![Alternative Text](https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg "With tooltip")
```

![Alternative Text](https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg "With tooltip")

**Using reference:**

```
![Alternative Text][Img]
```

![Alternative Text][Img]

**Using `<img>` tag in `[]` brackets:**

```
[<img src="https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg">](Img "With tooltip")
```

[<img src="https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg">](Img "With tooltip")

**Using `<img>` tag with `<style>` tag:**

```html
<img src="https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg" class="image" width="500" height="auto">

<style>
    .image {
        border-radius: 10%;
    }
</style>
```

<img src="https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg" class="image" width="500" height="auto">

<style>
    .image {
        border-radius: 10%;
    }
</style>

## Links

https://github.com/ => `https://github.com/`

<https://github.com/> => `<https://github.com/>` 

[Github](https://github.com/) => `[Github](https://github.com/)` 

[Github](https://github.com/ "Open Github") => `[Github](https://github.com/ "Open Github")` 

Go to [Github](https://github.com/) website => `Go to [Github](https://github.com/) website` 

Go to [Github][GithubSite] website => `Go to [Github][GithubSite] website` 

## References

Create: `[RefName]: RefValue`

`RefName` can be either a string or a number.

[GithubSite]: https://github.com/
[Img]: https://cdn.pixabay.com/photo/2015/07/10/17/25/portugal-839817_960_720.jpg
