# LoremSwiftum

[![](https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat-square)](https://developer.apple.com/swift/)  [![](https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square "License")](LICENSE.md)

**LoremSwiftum** is a lightweight lorem ipsum generator for Server Side Swift. It supports generating texts in different formats (words, sentences, paragraphs) and miscellaneous data (names, URLs etc.). This framework is a reimplementation of the library [LoremIpsum](https://github.com/lukaskubanek/LoremIpsum) written in Objective-C.

Note the original Swift 2.3 iOS/OS X port is located here: [lukaskubanek/LoremSwiftum](https://github.com/lukaskubanek/LoremSwiftum)

## Requirements

- Swift 3.0+

## Installation via Swift Package Manager

Add the following to your Package.swift file:

``` swift
.Package(
    url: "https://github.com/iamjono/LoremSwiftum.git", 
    majorVersion: 1, minor: 0
    ),
```

Then, regenerate your Xcode project:

```
swift package generate-xcodeproj
```

## Usage

To use in a project file, import the package:

``` swift
import LoremSwiftum 
```

### Methods

Generate a single sentence of Lorem Ipsum of between 4 and 16 words:

``` swift
var str = Lorem.sentence
```

Generate "n" sentences of Lorem Ipsum of between 4 and 16 words:

``` swift
var str = Lorem.sentences(count: Int)
```

Generate a single paragraph of Lorem Ipsum of between 3 and 9 sentences:

``` swift
var str = Lorem.paragraph
```


Generate "n" paragraphs of Lorem Ipsum of between 3 and 9 sentences:

``` swift
var str = Lorem.paragraphs(count: Int)
```

Generate a title of between 2 and 7 words:

``` swift
var str = Lorem.title
```

Generate a random single word from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.word
```

Generate "n" words from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.words(count: Int)
```

Generate a random single email from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.email
```

Generate a random single first name from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.firstname
```

Generate a random single last name from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.lastname
```

Generate a random single name (first and last) from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.name
```

Generate a random single tweet from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.tweet
```

Generate a random single url from the Lorem Ipsum "dictionary":

``` swift
var str = Lorem.URL
```


## Author

Lukas Kubanek // [lukaskubanek.com](http://lukaskubanek.com) // [@kubanekl](https://twitter.com/kubanekl)

Jonathan Guthrie // [https://github.com/iamjono](https://github.com/iamjono) [@iamjono](https://twitter.com/iamjono) - Swift 3 port & SPM integration.

## License

`LoremSwiftum` is released under the [MIT License](LICENSE.md).
