---
title: "Stop hating PHP"
date: 2025-03-07T14:00:00+01:00
tags:
  - php
  - frameworks
comments: true
---

I have been working with PHP in a professional environment for about three years. Despite this, PHP remains one of the most disliked languages among developers, which I find difficult to understand because it has evolved into a fairly robust and capable language.

## Why is it hated so much?

In its early days, PHP was considered quite insecure. Many of the CVEs at the time were related to PHP, reinforcing its reputation as an unsafe language—an assessment that was accurate back then. Additionally, the language had an overwhelming number of configuration options. Different configurations across devices often caused certain features to work on one system but fail on another. These configurations extended beyond basic settings like maximum file upload sizes, execution times, or memory limits to options that control error handling, which can significantly impact an application's behavior and security.

PHP is also regarded as an outdated language by some. Object-oriented programming (OOP) was introduced relatively late with PHP 5. Additionally, the standard library lacks an organized namespace, which is another common criticism. Many other important features, like OOP, were also added much later than in other languages. For instance, enums were only introduced in PHP 8.1, released in 2021. Moreover, PHP did not have a package manager until 2016, when the first stable version of [Composer](https://getcomposer.org/) was released. By comparison, [Maven](https://maven.apache.org/) had its first release in 2004.

Another common criticism of PHP is its syntax. For instance, array iteration functions are much more elegant and efficient in other languages compared to PHP. Here is a brief example:

**JavaScript:**
```js
result = myarray.map((x) =>  x.property)
        .sort((a, b) => (((a == b) ? 0) : (Math.pow(a, 2) > Math.pow(b, 2)) ? -1 : 1))
        .reduce((a, b) => a * b);
```

**PHP:**
```php
$unsorted = array_map(fn($x) => $x['property'], $array); 
uasort($unsorted, function($a, $b) { if($a == $b) { return 0; } return pow($a, 2) > pow($b, 2) ? -1 : 1; }); // now sorted
$result = array_reduce($unsorted, fn($a, $b) => $a * $b);
```
[Credits](https://www.reddit.com/r/PHP/comments/1fy71s/comment/caezeur/)

As you can javascript example looks way cleaner and is easier to read. The PHP code seems way harder to understand.

Another major issue with PHP is the inconsistency between errors and exceptions. Errors stem from the time when PHP only supported procedural programming, while exceptions were introduced with object-oriented programming (OOP). Since PHP is a blend of both paradigms, some functions throw exceptions while others return errors.

For example, the [json_decode](https://www.php.net/manual/en/function.json-decode.php) function accepts a flag that determines whether it should throw an exception or return an error. Some standard library functions, like [file_get_contents](https://www.php.net/manual/en/function.file-get-contents.php), return an error. If the operation fails, it returns `false`; if successful, it returns the file contents as a string. You then can retrieve the error using [error_get_last](https://www.php.net/manual/de/function.error-get-last.php). In contrast, other functions, such as [SplFileObject::__construct](https://www.php.net/manual/en/splfileobject.construct.php), throw exceptions when an error occurs.

Another reason the language is often disliked is the lack of high-quality, open-source projects written in PHP. While WordPress is popular, its codebase is often criticized for being messy, as the project is in a transition phase between procedural and object-oriented programming. Although it is improving, its current state remains problematic. 


## Is it better today?

Projects like TYPO3 have evolved over the years to adopt a more modern approach to PHP. They began using a package manager and object-oriented programming (OOP) to clean up their codebase. As a result, developing extensions for TYPO3 is now much more enjoyable compared to WordPress plugin development.

Over the past few years, many new features have been added to the language. PHP 8.1 introduced enums, and since PHP 7, we also have scalar type declarations. The language is now much more secure than in its early days. However, the bloat of configuration options still exists, as does the inconsistency between errors and exceptions. That said, the inconsistency is gradually being reduced. While the syntax remains largely the same, I personally don't find it as problematic as others claim. In fact, it can be quite readable and clean. But of course, this is a matter of personal opinion. Many people might feel the same way about the syntax of languages like Rust, Go, or Java.

The package manager Composer now offers a wide range of useful packages. Additionally, there are numerous tools available to enhance your coding experience. These tools provide supportive features and almost every capability commonly found in other languages. Want unit testing? Use [PHPUnit](https://phpunit.de/index.html). Need code formatting? Try [CS-Fixer](https://github.com/PHP-CS-Fixer/PHP-CS-Fixer). Looking for extra type safety and static analysis? Check out [PHPStan](https://phpstan.org/).


## Ecosystem

In addition to all the great tools, it’s the ecosystem that makes me really enjoy PHP. Frameworks like [Symfony](https://symfony.com/) and [Laravel](https://laravel.com/) are well-integrated and a pleasure to use. You can accomplish almost anything you want with them, as long as it involves web development. These frameworks even support building internal CLI applications within web applications. Furthermore, they allow integration with frontend frameworks like React or Vue. [Symfony UX](https://ux.symfony.com/) is another approach that makes web development with PHP more modern and enjoyable. There are so many different ways you can utilize these frameworks.

I have been working professionally in the Symfony environment for about three years, and from my perspective, I can definitely say that I've never encountered a scenario where the framework itself or a third-party library couldn't get the job done. These frameworks help you complete tasks efficiently and effectively. Of course, other frameworks in different languages offer similar functionality, but in my opinion, Symfony stands out for doing many things in exactly the right way.

## Conclusion

Overall, you could say that PHP was a pretty bad language in its early days, and even into the 2010s. However, today PHP is a solid choice for web projects. The language has gained many modern features and continues to evolve, becoming even better. With Composer as your package manager and a well-integrated ecosystem of tools and frameworks, PHP is definitely a great choice for modern web development. It's no longer relevant to hate PHP.

I would recommend you to just give it a shot and try it out yourself. You will love it. 
