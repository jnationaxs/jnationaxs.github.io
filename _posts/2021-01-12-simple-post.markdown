---
layout: post
title:  "Simple post"
date:   2021-01-12 10:23:30 -0800
categories: posts
---

This is a post about nothing, so to fill up space I've included some code

{% highlight swift %}
func bubbleSort(_ arr: inout [Int]) -> [Int] {
    guard arr.count > 1 else {
        return arr
    }
    for x in 0..<arr.count - 1 {
        for y in 0..<arr.count - 1 - x {
            if arr[y] > arr[y + 1] {
                let holder = arr[y]
                arr[y] = arr[y + 1]
                arr[y + 1] = holder
            }
        }

    }
    return arr
}
{% endhighlight %}
