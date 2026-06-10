# Lispex

**The language that captures the shape of thought.**

Lispex keeps a small, R7RS-shaped surface where code is data and data prints
plainly — parens are punctuation, recursion is rhyme. Quoted forms and
meta-programming come for free; the engine underneath is
[CSKernel™](https://github.com/studiohaze/cskernel), the deterministic
semantic kernel used by [Lena Code](https://github.com/studiohaze/lenacode).

```scheme
(define (fact n)
  (if (<= n 1) 1
      (* n (fact (- n 1)))))
```

- Website: https://www.lispex.com
- Status: in active development; source lives in a private repository while
  the language stabilizes. This is Lispex's public home.

> Heritage note: this is the S-expression language that briefly carried the
> name "Topaz" in an early experiment. [Topaz](https://github.com/studiohaze/topaz)
> is now its own (non-Lisp) language.

---

© 2026 Lispex. `(expressed-by 'studio-haze)` — [Studio Haze Inc.](https://www.studiohaze.co.kr)
