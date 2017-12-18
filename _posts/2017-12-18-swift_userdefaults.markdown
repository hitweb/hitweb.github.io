---
layout: post
title:  "Swift, Maxime Britto, UserDefaults !"
date:   2017-12-18 13:30:00 +0100
categories: swift
---
C'est un réel plaisir de suivre les cours en ligne de `Maxime Britto sur le développement iOS`.

[https://www.purplegiraffe.fr/](https://www.purplegiraffe.fr/)

L'utilisation du Playground, pour faire des codes simple... comme l'utilisation de l'App Playgrounds, sur iPad, permet d'apprendre à coder en s'amusant. 

![My helpful screenshot]({{ "http://blog.hitweb.com/assets/iPad_Playgrounds.jpg" | absolute_url }})

Les vidéos de Maxime permettent de maîtriser très rapidement les différentes interfaces de Xcode.
Voici un exemple d'utilisation de UserDefaults pour stocker des données en Swift :

```swift
//: Playground - noun: a place where people can play

import Foundation

let username = "hitweb"

UserDefaults.standard.set(username, forKey: "nickname")
UserDefaults.standard.set(129, forKey: "score");
UserDefaults.standard.set(["Riri", "Fifi", "Loulou"], forKey: "castors_juniors")

// quitter app
// relance app

let loadedName = UserDefaults.standard.string(forKey: "nickname")
let score = UserDefaults.standard.integer(forKey: "score")
let cousins = UserDefaults.standard.array(forKey: "castors_juniors")
```

[https://github.com/hitweb/code-examples/swift/](https://github.com/hitweb/code-examples/swift/)

