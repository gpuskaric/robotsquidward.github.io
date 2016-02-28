---
layout: post
title:  "Swift Optionals...?"
date:   2016-02-25
categories: ios swift development
---
This is a simple post about my appreciation for the little things in code.

I’m learning Swift for the first time, and I just learned about Optionals in Swift.  I just want to point out how great the syntax for an Optional is.

If you don’t know, here’s the syntax for a function returning an Optional:

        func foo(isBar: Bool) -> String? {
          if(isBar) {
            return "Bar"
          }
          return nil
        }

I just love the question mark!  Which is Swift’s way of denoting an optional return value.  It’s simple, effective, and memorable.  It gives the function personality, like it’s not quite sure if it has the String to give you or not.  Would you like a String?  Well then cough up the right Bool!

Maybe it’s not quite so profound, but I like to see it as a good example of the greater simplicity and personality you get from Swift.  I can’t wait to learn more.
