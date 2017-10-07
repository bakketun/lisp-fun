---
title: "My First Post"
date: 2017-10-04T12:37:54+02:00
draft: false
---

Hello World!

This is an **example**:

```common-lisp
(defun create-canonical-headers (headers)
  (merge-duplicate-headers
   (sort (loop for (key . value) in headers
               collect (cons (string-downcase key) (trimall value)))
         #'string<
         :key #'car)))
```
