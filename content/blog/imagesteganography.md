---
title: "Imagesteganography"
date: 2021-02-03T20:24:44+05:30
slug: "hiding another image inside an image"
description: "hiding another image inside an image"
keywords: ["image processing ",cryptography" , "privacy"]
draft: false
tags: []
math: true
toc: true

---


## What is Steganography?

"Steganography is an art of hiding information inside information i.e. embedding it in some other data. Steganography is the practice of concealing a file, message, image, or video within another file, message, image, or video.
The main objective of Steganography is mainly concerned with the protection of contents of the hidden information.
Images are ideal for information hiding because of the large amount of redundant space is created in the storing of images.
The goal of steganography is to hide messages in such a way that no one apart from the intended recipient even knows that a message has been sent. This can be achieve by concealing the existence of information within seemingly harmless carriers or cover.
"

## History

1. The first recorded uses of steganography can be traced back to 440 BC when Herodotus mentions an example of steganography in the histories of Herodotus.
2. ancient example is that of histories, who shaved the head of his most trusted slave and tattooed a message on it. After his hair had grown the message was hidden. The purpose was to instigate a revolt against the Persians.
3. During the “Cold War” period, US and USSR wanted to hide their sensors in the enemy’s facilities. These devices had to send data to their nations, without being spotted.
In October 2001, the New York Times published an article claiming that al-Qaeda had used steganography to encode messages into images, and then transported these via e-mail and possibly via USENET to prepare and execute the September 11, 2001 terrorist attack.

## What is the advantage of steganography over cryptography?


Cryptography hides the contents of a secret message from a malicious people, whereas steganography even conceal the existence of the message.
In cryptography, the system is broken when the attacker can read the secret message.
Breaking a steganography system need the attacker to detect that steganography has been used.

![cityscapes](/blog/images/city.png)



## as an image 

![eq](/blog/images/eq.png)

## as an equation in latex/katex 


$\frac{9283}{7411}$


$\frac{a}{n}$ = a

\documentclass[12pt,a4paper]{article}
\usepackage[latin2]{inputenc}
\usepackage{graphicx}
\usepackage{ulem}
\usepackage{amsmath}
\begin{document}
\begin{itemize}
\item \textbf{Error Probability of Algorithm }
\end{itemize}


Prime vs Composite



\textbf{Theorem}: Error Probability of Solovay Strassen Algorithm is 
$\le \frac{1}{2}$ .

\textbf{Proof:}

\ \ \ \ We need to show that for any odd composite n, n is Euler 
Pseudo-prime to the base a for at most half of the integers a ? Z$_{n
}$$^{*}$

Let G(n) = \{a: a $?Z_{n}$$^{*}$, $(\frac{a}{n}) \equiv 
a^{(n-1)/2 }$ (mod n)\}

First, we shall show that G(n) is subgroup of $Z_{n}$$^{*}$. 

Then by simply using Lagrange's theorem, if G(n) ? $Z_{n}$$^{*}$, 
we can prove that,\ \ \ \ \ \ \ \ \ \ \ \ 

$|G(n)|\le \frac{|Z_{n}|}{2}\le \frac{n-1}{2}$\\




\ \ \ \ \underline{Claim}: G(n) is a subgroup of $Z_{n}$$^{*}$

\ \ \ \ Proof: 

\ \ \ \ \ \ \ \ Suppose that a, b $?G(n).$

\ \ \ \ \ \ \ \ $ (\frac{a}{n}) \equiv a^{(n-1)/2 } (mod n)} $

\ \ \ \ \ \ \ \ $ (\frac{b}{n}) \equiv b^{(n-1)/2 } (mod n)} $

\ \ \ \ It follows from the multiplicative property of Jacobi symbols,

\ \ \ \ \ \ \ \ $(\frac{ab}{n})\equiv (\frac{a}{n})(\frac{b}{n}) \equiv 
a^{(n-1)/2 }b^{(n-1)/2 }$ (mod n).

\ \ \ \ $ab ?G(n).$

\ \ \ \ Hence, Closure holds for G(n). 

\ \ \ \ We know that since, G(n) is a subset of multiplicative finite 
group and is also closed under the operation of multiplication. 

\ \ \ \ $$ G(n) is subgroup of $Z_{n}$$^{*}$



\ \ \ \ Now, we need to show that there exist at least on element in $
Z_{n}$$^{*}$ which does not belong to G(n).



Suppose, n = p$^{k}$ q, where p and q are odd, p is prime, k ? 2, gcd 
(p, q) =1. 

 \ \ \ \ Let, a= 1 + $p^{k-1}q.$

\ \ \ \ We have, $(\frac{a}{n})= (\frac{a}{q})=1. $

\ \ \ \ Using Binomial theorem,

\ \ \ \ $a^{(n-1)/2}= \sum_{i=0}^{(n-1)/2}{(\frac{n-1}{2})C_{i}} 
(p^{k-1}q)^{i}$

\ \ \ \ \ \ \ \ \ \ \ \ $\equiv 1+\frac{n-1}{2} p^{k-1}q (mod n) $

\ \ \ \ $[$$?$ as for k? 2, the other terms in binomial expansion are 
0 (mod n) $]$

\ \ \ \ 

\ \ \ \ Let us assume, a $?G(n)$

\ \ \ \ $ (\frac{a}{n}) \equiv a^{(n-1)/2 } (mod n)} $

\ \ \ \ $?1=1+\frac{n-1}{2} p^{k-1}q (mod n)$

\ \ \ \ $? \frac{n-1}{2} p^{k-1}q=0 (mod n)$

\ \ \ \ $? p^{k}q \vert (\frac{n-1}{2} )p^{k-1}q ? p \vert 
\frac{n-1}{2} ?n \equiv 1 (mod p).$

\ \ \ \ But this is \textbf{contradiction. }Because we know that $
n\equiv 0 (mod p)$

\ \ \ \ $a ?G(n)$

\ \ \ \ $although a ?Z_{n}^{} , it does not belong to G(n)$

\ \ \ \ Thus, $\vert G(n)\vert \le \frac{n-1}{2}$ 

\ \ \ \ Suppose, n is composite. 

\ \ \ \ If gcd (a, n) ? 1 $? (\frac{a}{n}) \equiv 0$ ,

\ \ \ \ Thus, algorithm gives always correct answer in this case.

\ \ \ \ If, $a ? Z_{n}^{} , $thus gcd (a, n) ? 1, Solovay Strassen 
returns wrong answer if and only if a $?G(n)$.

\ \ \ \ We proved that |G(n)| ? (n-1)/2.

\ \ \ \ Thus, the probability of a wrong answer is:

\ \ \ \ \ \ \ \ \ \ \ \ $\frac{|Z_{n}^{}|}{n-1} 
\frac{|G(n)|}{|Z_{n}^{}|} \le \frac{1}{2}$





\end{document}