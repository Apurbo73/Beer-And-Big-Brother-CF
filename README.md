###﻿# Beer And Big Brother CF:



---

### 🔢 Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, i;
    cin >> a >> b;
```

* Reads two integers, `a` and `b`.
* These represent two values (often in problems like population, weight, or size comparisons).

---

```cpp
    for (i = 1;; i++) {
        a *= 3;
        b *= 2;
        if (a > b)
            break;
    }
```

* A `for` loop with no condition (`;;`) creates an **infinite loop**, but it's safely broken using `break` once `a > b`.
* On every iteration:

  * `a` is tripled (`a *= 3`)
  * `b` is doubled (`b *= 2`)
* After each multiplication, it checks if `a` has become greater than `b`.
* When it does, `break;` stops the loop.
* `i` tracks how many steps (iterations) it took.

---

```cpp
    cout << i << endl;
    return 0;
}
```

* Prints how many times the loop ran — essentially the **first year (or step)** where `a` becomes greater than `b`.

---

### 🧠 Real-world Analogy:

Think of:

* `a` as a small animal growing 3x per year.
* `b` as a larger animal growing 2x per year.
* The program finds how many years it takes for the small one to outgrow the larger one.

