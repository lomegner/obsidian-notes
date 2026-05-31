references:
[NaN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN)
[`NaN!===NaN`//true](https://en.wikipedia.org/wiki/Double-precision_floating-point_format)
[How does the internet work?](https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work)
[How the web works](https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works)
[bigint](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt)
[null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/null)
[short-circutting in JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence#short-circuiting)
[operators precedence](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence)
[logical AND](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_AND)
[logical OR](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_OR)
[nullish coalescing operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing)
[optional chaining](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)
[dynamic & static sites ](https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Server-side/First_steps/Introduction#static_sites)

## Notes
### 1.  How does the Internet work?
When two computers need to communicate, you have to link them, either physically (usually with an Ethernet cable) or wirelessly (for example with Wi-Fi or Bluetooth systems). All modern computers can sustain any of those connections.

 **Note:** For the rest of this article, we will only talk about physical cables, but wireless networks work the same. 

Such a network is not limited to two computers. You can connect as many computers as you wish. But it gets complicated quickly. If you're trying to connect, say, ten computers, you need 45 cables, with nine plugs per computer!
To solve this problem, each computer on a network is connected to a special tiny computer called a _router_. This _router_ has only one job: like a signaler at a railway station, it makes sure that a message sent from a given computer arrives at the right destination computer. To send a message to computer B, computer A must send the message to the router, which in turn forwards the message to computer B and makes sure the message is not delivered to computer C.
so router is a device which is a third party between computers for connecting them to each other despite of their numbers since their large quantity cause complication for connection.

### A network of networks
So far so good. But what about connecting hundreds, thousands, billions of computers? Of course a single _router_ can't scale that far, but, if you read carefully, we said that a _router_ is a computer like any other, so what keeps us from connecting two _routers_ together? Nothing, so let's do that.

Such a network comes very close to what we call the Internet, but we're missing something. We built that network for our own purposes. There are other networks out there: your friends, your neighbors, anyone can have their own network of computers. But it's not really possible to set cables up between your house and the rest of the world, so how can you handle this? Well, there are already cables linked to your house, for example, electric power and telephone. The telephone infrastructure already connects your house with anyone in the world so it is the perfect wire we need. To connect our network to the telephone infrastructure, we need a special piece of equipment called a _modem_. This _modem_ turns the information from our network into information manageable by the telephone infrastructure and vice versa.

**modem** is a router which lets us to access the other computers data which are out of our scope or our ISP and we can't control them because we don't own them, like a random person computer on the other side of the world or our friend's computer. this connection is made by the telephone wire for transmitting data since telephone wires are in every house and street and alley.

So we are connected to the telephone infrastructure. The next step is to send the messages from our network to the network we want to reach. To do that, we will connect our network to an Internet Service Provider (ISP). An ISP is a company that manages some special _routers_ that are all linked together and can also access other ISPs' routers. So the message from our network is carried through the network of ISP networks to the destination network. The Internet consists of this whole infrastructure of networks.
so An ISP, or Internet Service Provider, is a company that provides individuals and organizations access to the Internet, basically each company has a server (server is a computer or system that provides data, resources, or services to other computers, known as clients, over a network) which stores data of their websites like Google, Amazon and etc. 

If you want to send a message to a computer, you have to specify which one. Thus any computer linked to a network has a unique address that identifies it, called an "IP address" (where IP stands for _Internet Protocol_). It's an address made of a series of four numbers separated by dots, for example: `192.0.2.172`.
That's perfectly fine for computers, but we human beings have a hard time remembering that sort of address. To make things easier, we can alias an IP address with a human-readable name called a _domain name_. For example (at the time of writing; IP addresses can change) `google.com` is the domain name used on top of the IP address `142.250.190.78`. So using the domain name is the easiest way for us to reach a computer over the Internet.

### Finding computers
so basically what we said earlier was the definition of DNS, but what's DNS? DNS stands for Domain Name System. It is a hierarchical and decentralized naming system used to translate human-readable domain names (like www.example.com) into machine-readable IP addresses (like 192.0.2.1). This translation is essential because while humans find it easier to remember names, computers and network devices communicate using numerical IP addresses.
More commonly, DNS services are implemented as software running on general-purpose servers or virtual machines. This software can be installed on various operating systems, allowing any capable computer to function as a DNS server.
so DNS is an application our servers which converts domain names into IP's.

### Internet and the web
As you might notice, when we browse the Web with a Web browser, we usually use the domain name to reach a website. Does that mean the Internet and the Web are the same thing? It's not that simple. As we saw, the Internet is a technical infrastructure which allows billions of computers to be connected all together. Among those computers, some computers (called _Web servers_) can send messages intelligible to web browsers. The _Internet_ is an infrastructure, whereas the _Web_ is a service built on top of the infrastructure. It is worth noting there are several other services built on top of the Internet, such as email.
The term "web" can refer to several concepts, but it is most commonly associated with the World Wide Web (WWW). Here’s a brief overview:
World Wide Web (WWW): This is a system of interlinked hypertext documents and multimedia content accessed via the internet. Users can view web pages using web browsers, navigate between them through hyperlinks, and interact with various types of content.

### Intranets and Extranets
Intranets are _private_ networks that are restricted to members of a particular organization. They are commonly used to provide a portal for members to securely access shared resources, collaborate and communicate. For example, an organization's intranet might host web pages for sharing department or team information, shared drives for managing key documents and files, portals for performing business administration tasks, and collaboration tools like wikis, discussion boards, and messaging systems.
Extranets are very similar to Intranets, except they open all or part of a private network to allow sharing and collaboration with other organizations. They are typically used to safely and securely share information with clients and stakeholders who work closely with a business. Often their functions are similar to those provided by an intranet: information and file sharing, collaboration tools, discussion boards, etc.
Both intranets and extranets run on the same kind of infrastructure as the Internet, and use the same protocols. They can therefore be accessed by authorized members from different physical locations.

this modem in the house can connect to computer via cable or WIFI, that's where Wi-Fi plays its role. 

## 2.`NaN`
The **`NaN`** global property is a value representing Not-A-Number.

**Note:** you should only type `NaN` and `nan`, `nAn`, `nAN`, `Nan` or anything else doesn't work.

`NaN` is a property of the _global object_. In other words, it is a variable in global scope.

### Situation that result in `NaN`
There are five different types of operations that return `NaN`:

- Failed number conversion (e.g. explicit ones like `parseInt("blabla")`, `Number(undefined)`, or implicit ones like `Math.abs(undefined)`)
- Math operation where the result is not a real number (e.g. `Math.sqrt(-1)`)
- Indeterminate form (e.g. `0 * Infinity`, `1 ** Infinity`, `Infinity / Infinity`, `Infinity - Infinity`)
- A method or expression whose operand is or gets coerced to `NaN` (e.g. `7 ** NaN`, `7 * "blabla"`) — this means `NaN` is contagious
- Other cases where an invalid value is to be represented as a number (e.g. an invalid Date `new Date("blabla").getTime()`, `"".charCodeAt(1)`)

based on passage above, everything resulting in imaginary number ($i$), situation which need limit evaluation like  $\infty \div{\infty}$ ,$1^{\infty}$, $\infty-{\infty}$ and so on, and some special operation like number and string multiplication, is `NaN`. 

`NaN` and its behaviors are not invented by JavaScript. Its semantics in floating point arithmetic (including that `NaN !== NaN`) are specified by [IEEE 754](https://en.wikipedia.org/wiki/Double_precision_floating-point_format). `NaN`'s behaviors include:
- If `NaN` is involved in a mathematical operation (but not bitwise operations), the result is usually also `NaN`.
- When `NaN` is one of the operands of any relational comparison (`>`, `<`, `>=`, `<=`), the result is always `false`.
- `NaN` compares unequal (via `==`, `!=`, `===`, and `!==`) to any other value — including to another `NaN` value.

**example:**
```javascript
console.log(NaN===NaN);//false
console.log(NaN!==NaN);//true
```
the reason that `NaN!==NaN` is `true`, isn't because JavaScript, it has mathematical reason which for more info you can check [this article](https://en.wikipedia.org/wiki/Double-precision_floating-point_format)

`NaN` is also one of the falsy values in JavaScript.

### `NaN` checker
To tell if a value is `NaN`, use `Number.isNaN()` or `isNaN()` to most clearly determine whether a value is `NaN` — or, since `NaN` is the only value that compares unequal to itself, you can perform a self-comparison like `x !== x`.

```javascript
isNaN(NaN); // true
Number.isNaN(NaN); // true

function valueIsNaN(v) {
  return v !== v;
}
valueIsNaN(1); // false
valueIsNaN(NaN); // true
```

However, do note the difference between `isNaN()` and `Number.isNaN()`: the former will return `true` if the value is currently `NaN`, or if it is going to be `NaN` after it is coerced to a number, while the latter will return `true` only if the value is currently `NaN`:

```javascript
isNaN("hello world"); // true
Number.isNaN("hello world"); // false
```

For the same reason, using a BigInt value will throw an error with `isNaN()` and not with `Number.isNaN()`:

```javascript
isNaN(1n); // TypeError: Conversion from 'BigInt' to 'number' is not allowed.
Number.isNaN(1n); // false
```

**Note:** what basically passage above tries to say is, using `isNaN` for checking if a expression result or value is `NaN` or not, will give unexpected results while `Number.isNaN()` will act logical and give expected results, so just ignore `isNaN()` and use `Number.isNaN()` for checking if a value is `NaN` or not.

Additionally, some array methods cannot find `NaN`, while others can. Namely, the index-finding ones (`indexOf()`, `lastIndexOf()` cannot find `NaN`, while the value-finding ones (`includes()` can:

```javascript
const arr = [2, 4, NaN, 12];
arr.indexOf(NaN); // -1
arr.includes(NaN); // true

// Methods accepting a properly defined predicate can always find NaN
arr.findIndex((n) => Number.isNaN(n)); // 2
```

For more information about `NaN` and its comparison, see [Equality comparison and sameness](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness).

For more info about `NaN` read [this article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN).

## 3.Type conversion and type coercion
In JavaScript, type conversion and type coercion refer to the ways in which values are converted from one type to another. While they are related concepts, they have distinct meanings:

### Type Conversion

Type conversion is the explicit process of converting a value from one type to another. This can be done using built-in functions or methods. When you perform type conversion, you are intentionally changing the type of a value.

Examples of Type Conversion:

1. Using String():
```javascript
   let num = 123;
   let str = String(num); // Converts number to string
   console.log(str); // "123"
```

2. Using Number():
```javascript
   let str = "456";
   let num = Number(str); // Converts string to number
   console.log(num); // 456
```

3. Using Boolean():  
```javascript
   let value = 0;
   let boolValue = Boolean(value); // Converts number to boolean
   console.log(boolValue); // false
   ```

4. Using parseInt() and parseFloat():
```javascript
   let strNum = "3.14";
   let intNum = parseInt(strNum); // Converts string to integer (3)
   let floatNum = parseFloat(strNum); // Converts string to float (3.14) 
```

### Type Coercion

Type coercion, on the other hand, is an implicit process where JavaScript automatically converts types when performing operations that involve different types. This can happen during comparisons, arithmetic operations, or when using certain operators.

Examples of Type Coercion:

1. String Concatenation:
```javascript
    let result = "The answer is " + 42; 
    console.log(result); // "The answer is 42"
    ```
    
Here, the number 42 is coerced into a string for concatenation.

2. Arithmetic Operations:
```javascript
    let sum = '5' + 5; 
    console.log(sum); // "55" (string concatenation)
    
    sum = '5' - 5; 
    console.log(sum); // 0 (string coerced into a number)
```

3. Comparisons:
```javascript
    console.log(5 == '5'); // true (coerces string '5' into number)
    
    console.log(5 === '5'); // false (strict equality does not coerce types)
```

4. Logical Operations:
```javascript
    console.log(true + 1); // 2 (true coerced into number 1)
    
    console.log(false + null); // 0 (false coerced into number 0 and null coerced into number 0)
    ```
    

- Type Conversion: Explicitly converting a value from one type to another using functions like String(), Number(), etc.
- Type Coercion: Implicitly converting types during operations where different types are involved, often without the programmer's direct intention.

## 4.How the web works
1. The browser goes to the DNS server, and finds the real address of the server that the website lives on (you find the address of the shop).
2. The browser sends an HTTP request message to the server, asking it to send a copy of the website to the client (you go to the shop and order your goods). This message, and all other data sent between the client and the server, is sent across your internet connection using TCP/IP.
3. If the server approves the client's request, the server sends the client a "200 OK" message, which means "Of course you can look at that website! Here it is", and then starts sending the website's files to the browser as a series of small chunks called data packets (the shop gives you your goods, and you bring them back to your house).
4. The browser assembles the small chunks into a complete web page and displays it to you (the goods arrive at your door — new shiny stuff, awesome!).

### Order in which component files are parsed
When browsers send requests to servers for HTML files, those HTML files often contain `<link>` elements referencing external CSS stylesheets and `<script>` elements referencing external JavaScript scripts. It's important to know the order in which those files are parsed by the browser as the browser loads the page:

- The browser parses the HTML file first, and that leads to the browser recognizing any `<link>`-element references to external CSS stylesheets and any `<script>`-element references to scripts.
- As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from `<link>` elements, and any JavaScript files it has found from `<script>` elements, and from those, then parses the CSS and JavaScript.
- The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
- As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

### Packets
Earlier we used the term "packets" to describe the format in which the data is transferred between the client and server. What do we mean here? Basically, when data is sent across the web, it is sent in thousands of small chunks. There are multiple reasons why data is sent in small packets. They are sometimes dropped or corrupted, and it's easier to replace small chunks when this happens. Additionally, the packets can be routed along different paths, making the exchange faster and allowing many different users to download the same website at the same time. If each website was sent as a single big chunk, only one user could download it at a time, which obviously would make the web very inefficient and not much fun to use.

## 5.Bigint
In JavaScript, bigInt is a data type that provides a way to represent and work with integers larger than the maximum safe integer limit for the standard Number type. The maximum safe integer in JavaScript is $2^{53} - 1$ (or 9007199254740991).

Key Features of Bigint:

1. Arbitrary Precision: Unlike regular numbers, which are represented as double-precision floating-point values, bigint can represent integers of arbitrary size, limited only by the available memory, which means you can type any integer number in bigint as long as your memory supports it.

2. Syntax: You can create a `bigint` by appending an `n` to the end of an integer or by using the `BigInt()` constructor.
   - Example:

```javascript
     const bigIntFromLiteral = 123456789012345678901234567890n; // Using 'n' suffix
     const bigIntFromConstructor = BigInt("123456789012345678901234567890"); // Using constructor
     ```
     
**Note:** appending `n` to the end of the number is more common.

3. Operations: You can perform arithmetic operations on BigInt values, but you must be careful not to mix them with regular numbers. If you try to mix them, you'll get a TypeError.
   - Example:
     ```javascript
     const a = 10n;
     const b = 20n;
     const sum = a + b; // Works fine
     const c = 10; // Regular number
     // const result = a + c; // This will throw TypeError
     ```

4. Comparison: You can compare bigint values with other bigint values or with regular numbers, but keep in mind that they have different types (if you type `typeof` for a number like `56`, you receive `number` as its type but for a bigint like `56n` the type is `bigint`),so strict equality returns false due to their type difference.

   - Example:
```javascript
     console.log(10n === 10); // false (different types)
     console.log(10n == 10);  // true (loose equality)
```

5. Use Cases: bigint is particularly useful in scenarios where you need to handle large integers (integers which are greater than $2^{53}-1$), such as cryptography, high-precision calculations or when working with large datasets.

**Limitations:**
- You cannot use bigInt with methods that expect regular numbers (like Math functions).

**Precision:**
#examplePrecision
```javascript
console.log(10007199254740999+4==10007199254740999n+4n);//false
console.log(4==4n);//true
```
in the first `console.log()`because the number is greater than $2^{53}-1$, when you check the equality of bigint version of $10007199254740999+4$ which is $10007199254740999n+4n$ with the original number ($10007199254740999+4$), because this number ($0007199254740999+4$) is greater than $2^{53}-1$, the result of $10007199254740999+4$ may be slightly different than its real value due to JavaScript limitation in numbers greater than $2^{53}-1$, so you witnessed the precision error we were talking about it earlier, since this addition operation result is greater than $2^{53}-1$, we have to use bigint, the difference is not significant but for precise calculation that small gap of precision cannot be ignored.

real value of `10007199254740999+4`=`10007199254741003`
what JavaScript `10007199254740999+4` result is : `10007199254741004`
what JavaScript `10007199254740999n+4n` result is: `10007199254741003n`

this precision error doesn't limit to operation, even in plain number comparison, this flaw appears.

**example:**
```javascript
console.log(10007199254741003==10007199254741003n);//false
```
these two numbers as operands may seem identical but because they are larger than $2^{53}-1$, The number `10007199254741003` exceeds the safe integer limit for JavaScript's Number type, which is $2^{53} - 1$ (or `9007199254740991`), When you represent numbers larger than this limit as regular numbers, they may lose precision. This means that when you compare them, they may not be equal even if they look like they should be, but bigint number represent the real value of a number which is larger than $2^{53}-1$.
In JavaScript, numbers are represented using the IEEE 754 double-precision floating-point format (IEEE 754 double-precision floating-point format provides a way to represent real numbers in a binary format that can accommodate a wide range of values, including very small and very large numbers), which can accurately represent integers only up to $2^{53} - 1$ (or 9007199254740991). This is because JavaScript uses a 64-bit representation for numbers, where 53 bits are used for the significand (the part of the number that contains its digits).

When you use a number larger than $2^{53} - 1$, such as 10007199254741003, it cannot be represented exactly in this format. Instead, it gets rounded to the nearest representable value and number value changes in memory. This rounding can lead to precision loss.

so basically what you see on the screen is different what is stored in the computer memory representing that number.

Here's how it works in your specific case:

1. Regular Number: When you write 10007199254741003, JavaScript tries to represent this number as a floating-point value. However, since it's larger than $2^{53} - 1$, it cannot be represented exactly and gets rounded to a nearby value.

2. BigInt: The 10007199254741003n is a BigInt literal. BigInts can represent integers of arbitrary size without losing precision because they are not limited by the same constraints as regular numbers.

3. Comparison: When you compare these two values using `==`, JavaScript attempts to convert both operands to the same type before making the comparison:
   - The regular number (10007199254741003) is converted to its closest representable floating-point value (which may not be exactly 10007199254741003).
   - The BigInt (10007199254741003n) retains its exact value which is 10007199254741003 as a regular number.

Since these two values are not equal after conversion (due to the precision loss of the regular number), the comparison returns false.

In summary, even though you're dealing with what seems like a single number, how that number is stored and represented in memory affects its precision and equality comparisons in JavaScript.

the reason why IEEE 754 double-precision floating-point format can only support $2^{53}-1$ is was kind of complicated, you can read about it from chatgpt answers in JavaScript channel or on internet, so just ignore the reason why we can only have 2^53-1 numbers.

in #examplePrecision second `console.log()`, we see that `4==4n` because 4 is less than $2^{53}-1$, so the numbers are precise and `4==4n` output is true. another thing which I realized that you can represent any integer as bigint and they are equal to regular number exactly like `4==4n` example but the real difference happens when you want to work with numbers larger than $2^{53}-1$, which in that case regular integers are not equal to bigints version of the same number due to precision error reasons, so in that case bigint should be utilized otherwise the regular number is ok, so how should we know when to work with a bigint? since the difference between the regular number and a bigint version of that number is not that big in a mathematical operation, if the output or result of a **regular numbers** mathematical calculation was larger than $2^{53}-1$ or equal or near it, we should use bigints and for individual regular numbers which are larger than, near or a bit smaller than $2^{53}-1$, we should also use bigints.

**Note:** Be careful coercing values back and forth, however, as the precision of a BigInt value may be lost when it is coerced to a Number value.

### Comparisons

A BigInt value is not strictly equal to a Number value, but it _is_ loosely so:

```javascript
0n === 0; // false
0n == 0; // true
```

A Number value and a BigInt value may be compared as usual:

```javascript
1n < 2; // true
2n > 1; // true
2 > 2; // false
2n > 2; // false
2n >= 2; // true
```
### Bottom line
you can't use decimal number as bigint because decimal numbers aren't integers.
after all bigint application is rare and we should only use it in occasions we discussed earlier.
Namely, only `0n` is falsy, everything else is truthy.

for more info, please read [this article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt)
### 6.null
Null is one of JavaScript's primitive values and is treated as falsy for boolean operations.

`null` expresses a lack of identification, indicating that a variable points to no object. In APIs, `null` is often retrieved in a place where an object can be expected but no object is relevant.

### `typeof` null 
```javascript
typeof null; // "object" (not "null" for legacy reasons)
```

I've checked the differences of `null` and `undefined` in my notebooks and talked more about `null`, for more info read the notebooks.

for more info please read [this article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/null)

### 7.short-circutting
Short-circuiting in JavaScript refers to the behavior of logical operators (`&&` and `||`) where the evaluation of expressions is stopped as soon as the result is determined. This can lead to more efficient code execution and can also be used for conditional logic.
#qouteShort-circutting 

**Logical AND (`&&`)**
In the case of the logical AND operator (`&&`), if the first operand evaluates to false, JavaScript does not evaluate the second operand because the entire expression cannot be true. For example:
```javascript
let a = false;
let b = true;
let result = a && b; // result is false, b is not evaluated
```

In this example, since `a` is false, JavaScript does not check the value of `b`, and result is immediately determined to be false.

**Logical OR (`||`)**
For the logical OR operator (`||`), if the first operand evaluates to true, JavaScript does not evaluate the second operand because the entire expression will be true. For example:
```javascript
let x = true;
let y = false;

let result = x || y; // result is true, y is not evaluated
```
Here, since `x` is true, JavaScript skips evaluating `y`, and thus, result is immediately determined to be true.

this explanations above are brief and general, so I'm going to elaborate a little bit over that.

fist of all there are more operators that shirt-circtutting appears in their operands than `||`, `&&`.
the complete list contains these operators:
1. `||`(Logical OR)
2. `&&`(Logical AND)
3. `??`(Nullish coalescing operator)
4. `?.`(Optional chaining)
 
- the basic concept of short-circutting in `&&` and `||` is discussed above but it's not all, the        short-circutting may not only terminate the right hand side operand evaluation but it may terminate the whole expression or some other logical operators like `&&` or `||` operands evaluation.

####  General Logical Operators Rules
- in `||` if both operands are truthy, the left operand will be the answer, if both operands are falsy, the right operand is the answer, and if one of operands is falsy and another one is truthy, the answer is the truthy one, the same rule applies to `??` for picking the answer between the operands.

- in `&&` if both operands are truthy, the right operand will be the answer, if both operands are falsy, the left operand is the answer, and if one of operands is falsy and another one is truthy, the answer is the falsy one. 

- in Islam always the right-hand side represents the good and the left-hand side represents the evil, consider `&&` as the good guy which with two truthy operand always returns the right-hand side one and with two falsy always represents the left-hand side, meanwhile the `||` and `??` are like a evil person and they do everything opposite of `&&`, this method was a hint to remember these operators functionality.

#### Short-circuting VS Precedence
- in JavaScript these operators which are `||`, `&&` and `??`, they have precedence but if they have precedence, so what is this ***short-circut*** thing? the precedence and short-circut are 2 different terms for different places and both terms are correct.
  based on specs `&&` has higher precedence than `||` which means if there is a `&&` and `||` in an expression, the calculation related to `&&` gets done faster, this statement is both correct and wrong!

  look example below carefully:
#PrecedenceShort-circutSpecialExample
 ```javascript
function A() { console.log('called A'); return false; }
function B() { console.log('called B'); return false; }
function C() { console.log('called C'); return true; }

console.log(C() || B() && A());
// Logs:
// called C
// true

console.log(A() && C() || B());
// Logs:
// called A
// called B
// false

console.log((C() && A()) || B());
//// Logs:
// called C
// called A
// called B
// false
 ```
 in `console.log(C() || B() && A())` in example above, based on the precedence rule, first B() should be evaluated which returns false and logs `called B` , and when we have a falsy as the left operand of an `&&`, the answer is that left operand which is this case is `false`, then we have `C() || false`, so now system is supposed to evaluate the `C()`, which returns `true` and logs `called C` in console. and the final answer of this expression is `true`, but the final results in console is different from our expectation but why? because the interpreter doesn't give a fuck about precedence and precedence for logical operators like `||`,`&&` and `??`(not mathematical operators) is not defined for the interpreter, so how does the code gets interpreted? first when we have an expression, the interpreter check if there is a logical operator in it or not, every logical operator works like a gate i.e. the first operator from the left(the interpreter executes code from the left, so any operator in the left-most side, executed first), left-hand side gets evaluated and if it is necessary for it to evaluate the other side the operator and no short-circutting happens, it will allow the interpreter to evaluate the other side of the operator.
in the `console.log(A() && C() || B())`, first `A()` returns false and logs `called A` in console.
then because the left operand of `&&` is falsy, the right operands short-circuts, that's the reason we don't see `called C` in console, the second logical operator is `||` and because of that the rest of the expression doesn't get short-circuts after `&&` right operand, then we have `false || B()`, because `||` left operand is falsy, the right operand should be evaluated, that's where `B()` returns `false` and `called B` gets logged in the console, for the final result we have `false || false`, since both operands are falsy, the final result is the `||` right operand which is `false`. 

in `console.log((C() && A()) || B());` because I put `A() && C()` in `()`, the highest order logical operator became `||`, so its left operand should be evaluated, the left operand is `(C() && A())`, `C()` returns true and logs `called C` (we have no short-circutting here), `A()` return false and logs `called A`, the output is false, then we have `false || B()`, since left operand of `||` is falsy, the right operand should be evaluated, `B()` returns false and logs `called B` in console and now we have `false || false`, which the final output is `false`. 
 
 imagine code below: #PrecedenceShort-circutExample
 ```javascript
 const a= (10-4)-2*2 || 3**4-8*2 && 2+6-2**3
```
in this example interpreter spots two logical operators which are `||` and `&&`, the first one from left is `||`, so the left hand side of `||` should be grouped and executed based on their precedence, which in `(10-4)-2*2`, first we have `(6)-2*2`, then `(6)-4` and the final result is 2, since the result is a truthy as a left operand of `||`, the rest of expression short-circutts and the final result is 2, this short-circutting thing only for interpreters and as a human when we want to calculate the result of such expressions we should use precedence, which for this example since `&&` has higher precedence, we calculate its operands first which we start from its left operand `(81)-16=65`, then we have `65 && 2+6-2**3`, `65 && 8-8`, `65 & 0` and the answer is `0`, then we have `2 || 0`, which the answer is 2, you see in human approach we don't have such thing as short-circutting and we calculate each operand of every operator based on their precedence(`&&` has higher precedence than the `||` and `||` has higher precedence than `??`) (for operands of each operator, left-hand side operand has priority over the right operand) and both left and right operands get evaluated? so which one is correct? both of them are correct, in both approaches the result is equal, when we use short-circut approach we have `(6)-4||  rest of the expression`, because `(6)-4` is equal to `2`, therefore the left-hand side of the `||` is truthy, so the rest of the expression short-circuts and the final result is `2`, hence you see there is no difference in term of final answer in precedence (human approach) and short-circutting (machine approach), so why we have two different approach? first of all **technically** the short-circutting is the correct way to calculate the expression containing logical expressions because it's the approach of machine but if this short-circutting is the correct approach, we have an approach called precedence? because shor-circutting may seem confusing to some people and sometimes you may forget to apply and consider short-circutting rules while you're calculating your expression, that's why you use precedence approach when you as an individual want to handle the calculation due to less confusion and rules (in precedence approach you don't need to use short-circut and know the different short-circutting behavior of each operator and just calculate every operand of each logical operator based on their precedence).

so let's recap, technically short-circutting is the correct approach for calculating expressions containing logical expressions and there is no such thing as precedence approach and this precedence approach is a made-up solution for humans to reduce the confusion while working with logical expressions.

as we explained in #PrecedenceShort-circutExample, there is no difference in precedence and    short-circutting approach final results unless the operands have a side-effect like logging a result in console like in #PrecedenceShort-circutSpecialExample .

>However, note that short-circuiting does not change the final evaluation outcome. It only affects the evaluation of _operands_, not how _operators_ are grouped (it means the final result in short-circutting is the same as the precedence but if our operands have a side-effect, the side effects don't follow the precedence rule and follow short-circutting rule because short-circutting approach is what is getting carried out under the hood by the interpreter not the precedence approach) — if evaluation of operands doesn't have side effects (for example, logging to the console, assigning to variables, throwing an error), short-circuiting would not be observable at all.

the passage above is from the [MDN source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence) and it's approving our deduction.

the way the precedence and short-circut approach process the result is different, the short-circut approach the interpreter when checks the code, when spotting an expression containing the logical operators, since the code executes from the left and each operator works as a gate, so the interpreter, interprets the left-hand side the first operator based on their mathematical precedence till it reaches the operator it self, if the result was something that allows the short-circut, the process and calculation terminates here, the final result is calculated and the rest of the expression short-circuts but if short-circutting wasn't possible, the right side of the logical operator should be processed and calculated till we reach a new logical operator, then after the calculation of both side of the logical operator, we can find the result of that specific operator by using the general rules of logical operator we have explained earlier in this ****[[JavaScript + misc programming concepts#General Logical Operators Rules | section]]*** (like if both operands are falsy in `||`, the right operand is the answer), as you saw the logical operator works as a gate, it first process its left side and if there was a short-circut, the gate closes and expression short-circuts but if there is no short-circutting, the gate is open and rest of the expression can be evaluated.
each logical operator is a gate in its own `()` and they don't have power in other `()` to perform short-circutting, look at example above:

```javascript
const example= (3 || 0 &&/*2*/ 4)*4-5 &&/*1*/ 34; //34

const example2= 4-(3 && 2); //2
```

in the `const example` the interpreter first detects the `&&` with the `/*1*/` next to itself because that's the highest order logical order (how deep a logical operator is nested inside of a `()` or multiple `()` , that logical operator has lower precedence and gets detected by the interpreter later), so the left operand has to be evaluated, based on the mathematical precedence, first inside of the `()` should be evaluated, we have `(3 || 0 &&/*2*/ 4)`, as you see inside of this `()`, we have `||` and since its left operand is truthy the rest of the expression ***inside of the this `()`*** short circuts, as we know each logical operator has power for short-circutting in its own wrapping `()` not anywhere else,( we can assume a hypothetical `()` over our main expression which don't have `()` to understand functionality of `&&` with `/*1*/` next to it better, like this:
`((3 || 0 &&/*2*/ 4)*4-5 &&/*1*/ 34)`, so in this way you see that `&&/*1*/` has power in its own `()` and because it has the highest order among the other logical operators, it gets detected faster by the interpreter), after calculating the result of the `()` which is `3` now we have `3*4-5`  which the answer is `7`, so the left operand of `&&/*1*/` is truthy, therefore the right operand should be evaluated also, we have `7 && 34`, based on general logical operators rule we know the answer is `34`.
in the `const example 2`, first we have to detect the logical operators based on their order, which is `&&` inside of the `()`, its answer is `3`, now we have `4-(3)` which the final result is 1.

so in a nutshell this is how machine(interpreter) or the short-circutting method evaluates the final results: after reading the code by interpreter, if a expression had logical operators, the highest order logical operator from the left, left operand should be evaluated based on mathematical precedence, if short-circutting was possible, the short-circutting carries out and the rest expression in the `()` which that specific logical resides short-circuts and if there was a expression outside the `()`, that operation gets calculated, but if short circutting wasn't possible the whole expression gets evaluated based on the procedure it has, when we don't have short-circutting, we use general logical operators rules which we've learned them earlier, each `()` follow the same rule i.e. in eacj `()` we go, the interpreter looks for the logical operator with the highest order from the left to evaluate its left operand based on the mathematical precedence.

for evaluating an expression with precedence method, first we find the logical operator with the highest precedence and the highest order(the logical operator which resides in less nested `()` has highest order and that hypothetical `()` method which I introduced in short-circut section should be implemented here), when we found them we don't just evaluate the left operand, we evaluate both of its operand (first evaluate the left operand based on their mathematical precedence and then evaluate the right side of the operator by considering the mathematical precedence), and after finding the answer for that specific operator, we pick the answer and go for the next operator with highest precedence and highest order and so on. if two or multiple operators had the same precedence and same order, the one which is located in left-most has the priority, still the utilization of general logical operator rule and mathematical precedence applies here for finding the result or answer of an operator. because we don't consider short-circutting in this senario and approach, we don't consider logical operators as gates and when we have an logical operator we evaluates its both operand with using mathematical precedence and then finding the final result by using the general logical operators rule.
in MDN operators precedence, you may see logical operators precedence is lower than mathematical operators but in practice, they are not related at all, in any expression we first look for logical operators, then based on their precedence among each other( `||`, `&&` and `??` should be compared with each other and not with the mathematical operators), their operands gets evaluated based on their mathematical precedence.
the logical operator precedence is `&&` has the highest precedence, then is `||` and the lowest precedence belongs to `??`.

that MDN table gets used to find out which **mathematical operator** precedence is higher than other **mathematical operator**.

precedence table source: [precedence table](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence#table)

#### Operands precedence

```javascript
const obj={
  age:"hi"
}

const old=2*3-4+obj.age;
console.log(old);//2hi
```

in example above, in `const old=2*3-4+obj.age`, the `.` has the highest precedence comparing to mathematical operators (based on [precedence table](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_precedence#table)), so first `obj.age` gets evaluated in code above, which its result is `"hi"`, 
`2*3-4+"hi"`, then based on the mathematical precedence we have `6-4+"hi"`, then `2+"hi"`, and finally the output is `"2hi"`. 

#### Short-circutting difficulties for human
if a person wants to use short-circutting approach to calculate the output of an expression, due to forgetting to apply some rules like short-circutting, the output you calculate with the one computer calculates, may vary. that's the reason why we use precedence approach as a human to 
avoid such issues (since there is no short-circutting and you can calculate every operator each operand without concerning to make a mistake) that results in incorrect answers.

**example:**
```javascript
console.log(2 || 3 && 0);//2
```
the correct output of this expression is `2`, but if you forget to apply short-circutting in short-circut approach (which this forgetting seems to be a common mistake), your result will be wrong.

in short-circutting, interpreter start from left side of the expression and process the left operand of the highest order logical operator, in here we have `||` as the highest order logical operator from the left, if we forget to short-circut, the result of `2||3` will be `2` and then we have `2 && 0` which the final output is `0` which is wrong, but if we had applied short-circutting in the first place in `2||expression` the result would be `2`.

so if this short-circutting approach is such risky and confusing and as human we don't use it, why did we learn about it? because in some special cases like #PrecedenceShort-circutSpecialExample which the logical operators have side-effects e.g. logging a message in console, if you want to calculate the output by precedence approach, the side-effect can't be calculated properly (still the final output in both short-circut and precedence approach is equal but the side-effects are not), so we learn the short-circut approach to know why the side effects in these scenarios occur like this but because even in this scenario the output of both approaches are the same, we use precedence for calculation the output and for understanding the behavior of side-effects we use short-circuts method to understand them. 

#### how to use logical operators when coding
when we want to code and implement logic in our IDE, the thinking may differ with when we're trying to process and calculate the output of an expression.
we generally use logical operators as conditions in `if` statements in JavaScript or as default values.
for `if` statement scenario, we say if this expression was true (or truthy) ***and*** other expression was true, do something, if I want to transalte this sentence to code, it'll be this:
```javascript
if(expression1 && expression2 ){
console.log("do something");
}
```
you see we translated our English sentence into code, wherever we have used word `and`, we translated that to `&&` in our code.
in another scenario when we want to say if this expression was true(or truthy) ***or*** the other expression was true, do something, this get translated into code like this:
```javascript
if(expression1 || expression 2){
console.log("do something")
}
```
I haven't personally used `??` as condition in my `if` statements but it works like an `||`, so wherever in your sentence you use word `or`, you ca use `??` but the difference with `||` is that except for the `null` and `undefined`, everything is truthy, so if you wanted to use a `or` where things like `0` or `""` were true, you can use `??` (the application of `??` as a `if` statement condition is rare)

so we learnt that short-circutting and precedence rule is not the main thing we should concentrate while we're coding our application using logical operators and main thing is how to convert our English sentences into JavaScript code which we taught you here and this short-circutting and precedence approach is a collateral option we should consider while typing our own code. (we can use them as a approval to our code output when we finished typing our code) and the main application of this short-circutting and precedence approach is when you're trying to read other people or spec code and want to calculate and process the result. 

in default variable we usually use `||` or `??` (we don't use `&&`, because in default variable we want one of the items, if left-operand was truthy, we have that as our value but if it was falsy, we have the default value which is located as right-operand)

```javascript
const a="hi";
const value= a || "bye";//"hi"

const c="";
const value=c || "why";//why

const b=0;
const value=b ?? 100;//0

const d=undefined;
const value= d ?? "error";//error
```
we have to always put the value that we want to have it as default value as the right operand of `||` or `??` and locate the value we want to retrieve from the user or anywhere else (like `const a` or `const b` in example above) as the left operand because since default value is an alternative comparing to our retrieved value, so the retrieved value is more valuable than default value, so that why we locate our retrieved value in the left-operand because if our retrieved value is a truthy, that will be our output but if it's falsy, the right operand is the output, we usually use `||` for declaring default values but if we want to consider some values like `0`, `""` or false and etc. as truthy we have to use `??` (which using `??` in this scenario seems sensible because we may have some initial values like `const count=0` where we need to set it a zero as a base number, and then when user inserted any number in the website, that value will be replaced in that variable including number `0` itself, so only in case we have `undefined` and `null`, we want a default value which can be an error message )

```javascript
function numberInsertion(number){
const userInput= number ?? "Insert a number";
console.log(userInput);
}

numberInsertion(0);//0
numberInsertion();//when we don't pass an argument for our parameter, the value of that parameter becomes undefined, now in here output is undefined.
```
example above is one of the places that `??` can be used and `||` cannot, because in here `0` should be considered a truthy value since `0` is a number also and only when we don't insert value which `number` gets `undefined`, the default value which is `Insert a number` gets stored in `userInput`, if we had used `||` instead of `??`, for both function call the output would have been `Insert a number` and `0` didn't get logged in console despite of being a number.   

**Short-circutting in `||`**
for instance look at example below:
```javascript
console.log(2 || 3 && 4);//2

console.log(2 || 3 && 0);//2

console.log(0 || 3 && 4);//4

console.log(0 || 3 && false);//false

console.log(2 || false && 0);//2

console.log(false || 3 && 0);//0

console.log(false || 0 && 3);//0

console.log("" || false && 0);//false

console.log(2 || 3 || 4);//2

console.log(2 || 3 || 0);//2

console.log(0 || 3 || 4);//3

console.log(0 || 3 || false);//3

console.log(2 || false || 0);//2

console.log(false || 3 || 0);//3

console.log(false || 0 || 3);//3

console.log("" || false || 0);//0
```
if you notice whenever we have multiple logical operators like here which we have one `||` and one `&&`, short-circutting in one operator may affect the other operators, in the 1th, 2th, 5th, 9th, 10th and 13th `console.log()`, you see we have a truthy in left-hand side of the `||`, and the result is that truthy which is `2` in our examples, so whenever we have a truthy in the left-hnd side of the `||` the final is going to be that value which is located in the left hand-side of our `||` but remember our `||` should be the first logical operator from the left, otherwise the other first logical operator gets calculated in its own way, so in these examples the `2` is the answer and the right operand of the `||` and the rest of the expression which contain a `&&` or `||` doesn't get evaluated i.e. they get ***short-circutted***, in these examples only left operand of `||` gets evaluated and rest of the expression gets short-circutted because it doesn't matter if you calculate the rest of the expression, still the answer is going to be the truthy left-hand side operator `||` which is `2` but remember this short-circutting behavior which when we have a truthy in our left-hand side of our first from left `||`, rest of the expression short-circutts, only belong to `||`, for the other logical operator that can short-circut, the behavior is different.  

**so based on the info above, we conclude, whenever we have a truthy in left hand side of a `||` the answer is that value which is located in the left hand side of the `||` and the right hand-side of the `||` doesn't evaluates and the rest of the expression short-circutts but if our left hand-side is falsy, the answer of that `||` will be the right operand despite of right hand-side operand is falsy or truthy, and the rest of the expression may or may not short-circutts depends on the type of the right hand-side operand.**
but if the left hand side of our `||`(which this `||` is the first logical operator from left) is falsy, the right operand gets evaluated and other operands based on their character(falsy-ness or truthy-ness) and their logical operators, may or may not get short-circutted, for example in the last `console.log()` the left operand of first `||` is falsy, so the right operand gets evaluated, the answer of the first `||` is the right operand which is `false` and the second `||` compares `false` and `0` because the left operand is falsy, the right operand evaluates and the answer is the right operand which is `O`, so in this example no short-circutting occurred and every operand evaluated.

so based on the short-circutting behavior of `||` which we learned from passage above,           short-circutting happens wherever it is required to occur just like quote below form     #qouteShort-circutting.

>Short-circuiting in JavaScript refers to the behavior of logical operators (`&&` and `||`) where the evaluation of expressions is stopped as soon as the result is determined

you can check examples above for more info.

**Short-circutting in `&&`**
in `&&` operator if the left-operand is falsy, the answer of that operator (`&&`) comparison is that falsy value which is located in the left-hand side of the `&&` and the right hand-side of that `&&` doesn't get evaluated and short-circuts but we can't decide if the rest of the expression gets     short-circutted or not because the short-circut of the rest of the expression depends on type of other logical operators in the expression unlike `||`.

if the left operand of the `&&` was truthy, the answer of that `&&` comparison will be its right      hand-side operand either it is truthy or falsy and short-circutting depends on rest of the expression.

look at examples below:
```javascript
console.log(2 && 3 || 4);//3

console.log(2 && 3 || 0);//3

console.log(0 && 3 || 4);//4

console.log(0 && 3 || false);//false

console.log(2 && false || 0);//0

console.log(false && 3 || 0);//0

console.log(false && 0 || 3);//3

console.log("" && false || 0);//0

console.log(2 && 3 && 4);//4

console.log(2 && 3 && 0);//0

console.log(0 && 3 && 4);//0

console.log(0 && 3 && false);//0

console.log(2 && false && 0);//false

console.log(false && 3 && 0);//false

console.log(false && 0 && 3);//false

console.log("" && false && 0);//""
```
in the 3th `console.log()` at first left operand of `&&` gets evaluated and since it is falsy, the answer of this `&&` comparison is that falsy answer which is `0`, then the right operands short-circuts but because the second logical operator is `||` the rest of expression doesn't short-circuts, if we want to check it, the left operand of this `||` is the `0` from `&&` if the right operand of `||` is the truthy, the answer of whole expression will be that `||` right operand, so when we have `&&` at first and then we have `||` in the rest of the expression, short-circutting can't occur cause the right operand of the `||` should be evaluated so we can make a decision what the answer is, meanwhile in 11th `console.log()` we have two `&&` and the left operand of first `&&` is falsy, so the right operand of `&&` short-circuts, so the answer of first `&&` comparison is `0`, so this `0` becomes the left operand of the second `&&`, and the right operand of `&&` short circuts, so if our left operand in our `&&` is falsy, the rest of the expression short-circuts as where as we have `&&`, if we encounter `||` or `??` everything changes and short- circutting depends on type of operands.  

in the 1th `console.log()`, the left operand of `&&` is truthy, so the left operand of that `&&` should be evaluated, since the right operand is truthy also, the `&&` comparison answer is `3`(right operand), this `3` becomes the next operator left operand, the next operator is `||` and because its left operand is truthy, the right operand short-circuts and the answer of this expression is `3`.

in the 9th `console.log()` because the left operand of `&&` is truthy, the right operand should be evaluated  and the result is `3` because the right operand is truthy also, then because the second operator left operand is truthy, its right operand should be evaluated also.

for more info, check the examples above.

**short-circutting in `??`** #short-circuttingInNullishCoalescingOperator
`??` is exactly like `||` but the difference is in `??` only nullish values are falsy and values like: `0`, `""`,` `` `, `''`, `0n`, `NaN`, `false` are truthy in `??`.

- **Nullish values:** In JavaScript, a nullish value is the value which is either `null` or `undefined`.

- **Note:** `[]`(empty array) and `{}`(empty object) are truthy values in everywhere.

I'll explain about `??` later in its own topic and in here I only speak about its behavior in            short-circutting.

so in short-circutting term `??` and `||` are equal and behave same except in `??` everything is truthy except for `null` and `undefined` which are falsy.
```javascript
console.log(0 || 3);//3
console.log(0 ?? 3);//0
```
since `??` is a special form of `||`, so short-circutting behavior in `??` is same as `||`.
```javascript
console.log(2 || 3 && false);//2
console.log(2 ?? 3 && false);//2
console.log(false || 3 && 0);//0
console.log(false ?? 3 && 0);//false
```

**Short-circutting in `?.`** #short-circuttingInOptionalChaining
The `?.` operator is like the `.` chaining operator, except that instead of causing an error if a property value is nullish (`null` or `undefined`) or the property doesn't exist, the expression short-circuits with a return value of `undefined`. When used with function calls, it returns `undefined` if the given function does not exist.

**example:**
```javascript
const adventurer = {
  dog:{
    occupation:{
        department:"DEA"
    }
  },
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const adventurer2 = {
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const dogName1 =adventurer.dog.age;//1*
const dogName2 =adventurer.dog?.age;//2*
const dogName3 =adventurer.dog.age.city.car;//3*
const dogName4 =adventurer.dog?.age.city.car;//4*
const dogName5 =adventurer.dog.age?.city.car;//5*
const dogName6 =adventurer.dog?.age?.city.car;//6*
const dogName7 =adventurer2.dog.age;//error
const dogName8 =adventurer2.dog?.age;//undefined
const dogName9 =adventurer?.dog?.age;//undefined

console.log(dogName1);//undefined
console.log(dogName2);//undefined
console.log(dogName3);//error
console.log(dogName4);//error
console.log(dogName5);//undefined
console.log(dogName6);//undefined
console.log(dogName7);//
console.log(dogName8);//
console.log(dogName9);//
```

in `1*` the output is `undefined` and no error is thrown, when a property doesn't exist, it doesn't matter whether you're accessing that property with `.` or `?.`, it always returns `undefined` but this rule only applies to the first absent property we're trying to  access via `.`, if we chain another property to that absent property, the whole program terminates and an error throws like in `3`. 
and for `?.` never place the `?.` before the first absent property (bear in mind, that we don't know which property doesn't exist, we may suspect some of the properties are absent that why we use ?. or we are a place that we want if a property didn't exist, instead of an error and code termination, we receive an `undefined` and code ability to execute the rest of the code), because in that case `?.` is going to act like `.` and when we want to access the second absent property, chained to the first absent property, so there is no difference between `.` and `?.` in this specific situation, so if you doubt that the property may be absent or you don't want that in case of property absence, you receive error and code termination, you should use `?.` because figuring out what order each property has, is a boilerplate, so just use `?.` from the first place for the first, second and rest of other suspicious properties, in `4*` because `?.` is equal to `.` ( due to using `?.` before first absent property), their functionality is equal to each other, so you can see instead of short-circuting the rest of the expression after `city`(because this is where the error occurs), it throws error but in `5*` because we have used `?.` before the second absent property, the whole expression                short-circutted after `city` and `undefined` returned.
in `6*` we've used `?.` before the first absent property and second absent property (this is the most common scenario which we don't know which property is absent and where this absence will unveil), and you see short-circutting occurred after `city`(which is first absent property and we have used `?.` after first absent property i.e. `age` and before second absent property which is `city`)  

```javascript
const adventurer = {
  dog:null//or undefined
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const dogName1 = adventurer.dog.age;
const dogName2 =adventurer.dog?.age;
const dogName3 =adventurer.dog.age.city.car;
const dogName4 =adventurer.dog?.age.city.car;
const dogName5 =adventurer.dog.age?.city.car;

console.log(dogName1);//error
console.log(dogName2);//undefined
console.log(dogName3);//error
console.log(dogName4);//undefined
console.log(dogName5);//error
```
when the property value is `undefined` or `null`, everything is different, in the previous section we stated that if we use `.` before first absent property  and we want to access only the first absent property, console returns `undefined` but in this section when the property we want to access previous chained property value  is `null` or `undefined`, its order doesn't matter, even if it is the first one, an error will be thrown, that's why we say to use the `?.` even for the first accessed property (to avoid confusion) in places that instead of a error, we want the rest of the code to be executed and a default value returns like:

```javascript
function ObjGenerator(firstName){
this.name=firstName
this.occupation="developer";
let objName=this?.name?.lastName ?? "no Name is inserted"
console.log(objName);
}
ObjGenerator();
```
you see in example above, in `let objName=this?.name?.lastName ?? "no Name is inserted"`, if we put `.` instead of the second (for the first doesn't matter) `?.`, we encounter an error but now by using the `?.`, we can have a default value for our variable and code doesn't terminate due to error. (by the way we used `?.` instead of every `.` because we don't know the error might happen in where) in example above, the first absent property is `lastname` in                                           `let objName=this?.name?.lastName ?? "no Name is inserted"` if instead of name being `undefined`, was something like `john`, the `let objName=this.name.lastName ?? "no Name is inserted"` would return `undefined` but now the `name` property is `undefined`, the                     `let objName=this.name.lastName ?? "no Name is inserted"` will throw an error.

***in a nutshell, if the first absent property, previous property(which is present and exist) value was `undefined` and `null`, and we want to access that absent property via `.` like `obj.presentProperty.absentProperty` we'll encounter an error and we have to use `?.` before the first absent property which we have `obj.presentProperty?.absentProperty` (the rest of the properties don't need it because after the first absent property, rest of the expression              short-circuts and `undefined` returns but we use `?.` instead of  all `.` because we don't know where the error might happen and which property is the first absent property and not throwing error is important in our scenario), so the most complete version is `obj?.presentProperty?.absentProperty`.***

***if the present property before the first absent property value is something else than `null` and `undefined`, like `john`, if we want to access the first absent property with `.`, we don't encounter any error and `undefined` returns, the reason for it is , when the present property value is `undefined` and `null` and when the absent property wants to access `undefined` or `null`, since accessing an undefined or null via `.` throws an error that's why you face an error but when the present property value is something is like `john`, since `john` is not a nullish value, the access to this present property by an absent property returns `undefined` via `.` because the interpreter says I couldn't find any `absentProperty` in `john` , so this `absentProperty` is `undefined` and that's why when the second absent property is chained to the first absent property via `.`, throws an error because you're trying to access an undefined value, so we use `?.` in places where we don't want to encounter any error or code termination for absence of properties while accessing them like `obj?.presentProperty?.absentProperty`.***

```javascript
const adventurer = {
  dog:null//or undefined
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const adventurer2 = {
  dog:"lome",
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const adventurer3 = {
    name: 'Alice',
  cat: {
    name: 'Dinah',
  }
};

const dogName =adventurer.dog.age();
const dogName1 =adventurer.dog.age?.();//bad practice
const dogName2 =adventurer.dog?.age();
const dogName3 =adventurer2.dog.age();
const dogName4 =adventurer2.dog.age?.();
const dogName5 =adventurer2.dog?.age();//bad practice
const dogName6 =adventurer3?.age();//bad practice
const dogName7 =adventurer3.age?.();
const dogName8 =adventurer3?.age?.();//best practice
const dogName9 =adventurer3.dog.age();
const dogName10 =adventurer?.dog?.age?.();//best practice
const dogName11 =adventurer3?.dog?.age?.();//best practice

console.log(dogName);//error
console.log(dogName1);//error
console.log(dogName2);//undefined
console.log(dogName3);//eror
console.log(dogName4);//undefined
console.log(dogName5);//error
console.log(dogName6);//error
console.log(dogName7);//undefined
console.log(dogName8);//undefined
console.log(dogName9);//error
console.log(dogName10);//undefined
console.log(dogName11);//undefined
```
`dog` is the present property in this object and `age()` is an undefined method, since the present property value is nullish, if we want to chain an absent property or method to it, we encounter an error, but the difference is even if the present property wasn't nullish and we wanted to access an undefined method via `.` still we encounter an error, so we have to use `?.` instead of `.` before  the first absent method but when the present property or object value isn't nullish we have to put `?.` behind of the `()` of method call and not the name of the method. 

- since we don't know what's the value of present property, we have to put `?.` one before name of the method and one before its `()`. like `dogName10`.

```javascript
const array1=[23,"hi",null/*or undefined*/,89];

console.log(array1[2][3]);//error
console.log(array1[2]?.[3]);//undefined
console.log(array1[1][4]);//undefined
console.log(array1[1]?.[4]);//undefined
console.log(array1?.[1]?.[4]);//undefinrd and best practice
console.log(array1[1][4][5][6]);//error
console.log(array1[1]?.[4][5][6]);//error
console.log(array1[1][4]?.[5][6]);//undefined
console.log(array1?.[1]?.[4]?.[5]?.[6]);//undefined
console.log(array1[2][4]());//error
console.log(array1[2][4]?.());//error
console.log(array1[2]?.[4]());//undefiend
console.log(array1[2]?.[4]?.());//undefined
console.log(array1?.[2]?.[4]?.());//undefined and best practice
console.log(array1[1][4]());//error
console.log(array1[1][4]?.());//undefined
console.log(array1[1]?.[4]());//error
console.log(array1[1]?.[4]?.());//undefined
console.log(array1?.[1]?.[4]?.());//undefined and best practice
console.log(array1[6][4]());//error
console.log(array1[6]?.[4]());//undefined
console.log(array1[6][4]?.());//error
console.log(array1?.[6]?.[4]?.());//undefined and best practice
```
the same rule we have for objects, applies to arrays. we can use `?.` only in arrays and objects.
we can put `?.` behind of `[]` but not `.`, we use `?.` in arrays for same scenarios we had with objects, like where we need that instead of an error we receive a undefined while trying to access a property in object or element in an array.

- Optional chaining cannot be used on a non-declared object or array.

```javascript
undeclaredVar?.prop; // ReferenceError: undeclaredVar is not defined
```
- there is no such a operator in JavaScript to only identify `undefined` as falsy.
- there is no such a operator in JavaScript to only identify `null` as falsy.
### 8.Nullish coalescing operator
The **nullish coalescing (`??`)** operator is a logical operator that returns its right-hand side operand when its left-hand side operand is `null` or `undefined`, and otherwise returns its left-hand side operand.

#### `??` and `||`,`&&` with the same order
there are more info in #short-circuttingInNullishCoalescingOperator about this operator, you can check that section for more info.
It is not possible to combine both the AND (`&&`) and OR operators (`||`) directly with `??`. A syntax error will be thrown in such cases.

```javascript
null || undefined ?? "foo"; // raises a SyntaxError
true && undefined ?? "foo"; // raises a SyntaxError
```

but you can use it this way:

```javascript
(null || undefined) ?? "foo"; // returns "foo"
```
it's important that `??` and `||` or `&&` don't have the same order otherwise an error will be thrown.

#### `??` applications
1. first application and most important application is, the scenarios where we combine `??` with optional chaining `?.` which we've explained it in [[JavaScript + misc programming concepts#Optional chaining application|here]]. 
2. when we want to use this operator in an `if` statement as a condition while everything is truthy except for `undefined` and `null` like when we trying to check if the user input, stored in our variable is a number which `0` is a number also but if we use `||`, the operator identifies `0` as a falsy and not a number.
   **example:**
 
 ```javascript
 let number=0;
 let text=null;
 if (number || text){
 console.log(we have an input)
 }//logs nothing!

 if (number ?? text){
 console.log(we have an input)
 }//logs 0
 ```
   this can be useful, when we store user input in a variable and then we want to use that variable value as a condition like condition above which this input can be a `0`.

3. Earlier, when one wanted to assign a default value to a variable, a common pattern was to use the logical OR operator (`||`):

```javascript
let foo;
// foo is never assigned any value so it is still undefined
const someDummyText = foo || "Hello!";
```

However, due to `||` being a boolean logical operator, the left-hand-side operand was coerced to a boolean for the evaluation and any _falsy_ value (including `0`, `''`, `NaN`, `false`, etc.) was not returned. This behavior may cause unexpected consequences if you consider `0`, `''`, or `NaN` as valid values.

The nullish coalescing operator avoids this pitfall by only returning the second operand when the first one evaluates to either `null` or `undefined` (but no other falsy values):

```javascript
const myText = ""; // An empty string (which is also a falsy value)

const notFalsyText = myText || "Hello world";
console.log(notFalsyText); // Hello world

const preservingFalsy = myText ?? "Hi neighborhood";
console.log(preservingFalsy); // '' (as myText is neither undefined nor null)
```
you can see more about this application in [[JavaScript + misc programming concepts#how to use logical operators when coding|here]].

### 9.Optional chaining
The `?.` operator is like the `.` chaining operator, except that instead of causing an error if a property value is nullish (`null` or `undefined`) or the property doesn't exist, the expression short-circuits with a return value of `undefined`. When used with function calls, it returns `undefined` if the given function does not exist.

I've explained its syntax, short-circutting scenarios and all of the conditions in                       #short-circuttingInOptionalChaining, you can refer to that section for more info.

#### Optional chaining application 
we explained in #short-circuttingInOptionalChaining that we use `?.` in places we don't want to encounter error and code termination when we're trying to access an absent property (encountering error while looking for an absent property isn't a bad thing and actually a good thing because it warns you but in some scenarios like the default variable situation this error can turn everything terrible and ruin our code base but if instead we had something like `?.` which helps us to have `undefined` instead of that error and code doesn't terminate, that would be great) like when we want to store a value in a variable with default value option. (there is an example in #short-circuttingInOptionalChaining )
the application of `?.` is not something common and it's almost rare and only scenario that can cross my mind that `?.` application can be useful is when it's used with `??` for assigning a value to a variable with default value option.

**example:**
```javascript
function printCustomerCity(customer) {
  const customerCity = customer?.city?.cityName ?? "Unknown city";
  console.log(customerCity);
}

printCustomerCity({
  name: "Nathan",
  city:{
 cityName:"paris"
 }
}); // "Paris"
printCustomerCity({
  name: "Carl",
  details: { age: 82 },
}); // "Unknown city"
```
in this scenario if we had used `.` instead of `?.` to access the object properties, an error would be thrown and code terminated but by using the `?.`, `undefined` returned and `"Unknown city"` as a default value got assigned to the `customerCity` variable in the second function call.  
if I want to elaborate about optional chaining application, I have to say in situations like this one which we have a function that requires an input from user or the input should be retrieved from somewhere else like a `fetch` method and it's in form of an object or array (in other data types, we don't have any property to want to access it)  and us, as  developers, have guessed
what kind of info we require from that user input and what kind of info he/she may insert or will be retrieved, if that input contained those info, we grab those info and use it in our code but if the input lack that info, we have set a default value that will be used in our code to give us a different output, in these scenarios even we had only one property after the object or array (which in term of our function, is the function parameter) despite of it will return `undefined` even with`.` but use `?.` because you may add another properties later.

- in the first function call you can see if all the required info is available, there is no difference between the `.` and `?.` and their result is the same.

### 10.expressions in JavaScript
I've explained about difference and relation of expression and statement before, only thing I wanted to mention is that `x=9` is a expression, so basically it's a statement also.
statements in JavaScript are piece of codes that perform actions like `if`, `for` and etc.

### 11.hexadecimal representation of binary, Unicode
Hexadecimal numbers are used in computers to represent binary data for several reasons:

1. Compactness: Hexadecimal (base 16) is more compact than binary (base 2). Each hexadecimal digit represents four binary digits (bits). For example, the binary number `1111` can be represented as `F` in hexadecimal. This means that a large binary number can be expressed in a much shorter form using hexadecimal, making it easier to read and write.

2. Human Readability: Hexadecimal is more human-readable than long strings of binary digits. For instance, instead of writing `11111111 11111111 11111111 11111111` for a 32-bit value, you can write `FFFFFFFF` in hexadecimal. This makes it easier for programmers and engineers to work with and debug code.

3. Alignment with Byte Structure: Computers typically process data in bytes (8 bits). Since one byte can be represented by two hexadecimal digits (e.g., the byte `10101100` is represented as `AC`), this alignment simplifies the representation of data structures and memory addresses, for example the ASCII table (which is the fundamental of conversion of human language (English as the most common language) into computer language (binary)) has 128 characters and each character has a binary value (you can see in ***[[JavaScript + misc programming concepts#why ASCII table character takes 1 byte (8 bit) while there are 128 character in this table (128=7 bit)|here]]*** why ASCII table character occupy 1 byte       (8 bit) while they are only 128 (7 bit) of them) has 128-256 (extended version) characters, representing these characters in binary can result in a long and confusing number but in hexadecimal number with two digits you can cover all of the ASCII characters (since hexadecimal system has 16 digits, and by considering in our number each take can take one of these hexadecimal digits, we have 16\*16=256 ) and each ASCII table character can be represented in a format like `0x1F` which `0x` get used to specify this number format is hexadecimal, so you ***may*** see it in every hexadecimal number in different occasions, the next two elements which are `1F` are hexadecimal digits (`1` & `F`) that in this case `1F` represents `26` in decimal system.
   so as you saw, using hexadecimal to represent ASCII table characters comparing to binaries, gives us a shorter format which reduces confusion.
   you can see full ASCII table characters and their binaries and hexadecimal representation in ***[this link](https://www.eso.org/~ndelmott/ascii.html)***.

4. Ease of Conversion: Converting between binary and hexadecimal is straightforward because each hex digit corresponds directly to a group of four bits. This makes it easy to switch between the two representations without complex calculations.

5. Common Usage in Programming: Many programming languages and systems use hexadecimal notation for various purposes, such as defining color values in graphics programming or representing memory addresses, which further reinforces its use.

Overall, using hexadecimal provides a balance between compactness and readability while maintaining a close relationship with the underlying binary representation used by computers.
so we may encounter something like `0x1F` while browsing the internet which is a hexadecimal number (I elaborate about this syntax later), this hexadecimal number is used to represent a binary number, since the binary version can be long sometimes and confusing, this hexadecimal number get used in different location to display that binary number in a shorter and more comprehendible form to the user.

in some cases the user insert a hexadecimal number as a input like the `color` attribute in `CSS`, under the hood the rendering engine (part of the browser that has the responsibility of `CSS` and `HTML` interpretation and rendering which firefox rendering engine name is Gecko and google chrome one is Blink) converts that hexadecimal number into binary for computer, so you as a user while inserting that color code didn't have any difficulty since hexadecimal is short and concise and thanks to the rendering engine that hexadecimal number converts to the binary and computer understands that binary and evaluates that specific color.

the numbering system humans use to count, called `decimal` numbering %% system %% because there are 10 digits in this system (0,1,2,3,4,5,6,7,8,9). 

in `hexadecimal` system we have 16 digits which they get represented in this way: 0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F.

you can see equivalent of numbers from 0-15 (which is the numbers of digits in hexadecimal system) in decimal or human numbering system in hexadecimal (the numbering system, made that human can understand the language of computer better) and binary format (the language that computer understands).

| Decimal | Hexadecimal | Binary |
| ------- | ----------- | ------ |
| 0       | 0           | 0000   |
| 1       | 1           | 0001   |
| 2       | 2           | 0010   |
| 3       | 3           | 0011   |
| 4       | 4           | 0100   |
| 5       | 5           | 0101   |
| 6       | 6           | 0110   |
| 7       | 7           | 0111   |
| 8       | 8           | 1000   |
| 9       | 9           | 1001   |
| 10      | A           | 1010   |
| 11      | B           | 1011   |
| 12      | C           | 1100   |
| 13      | D           | 1101   |
| 14      | E           | 1110   |
| 15      | F           | 1111   |

#### Bit, Byte, Binary
In programming, a "bit" is the most basic unit of data in computing and digital communications. The term "bit" is short for "binary digit," and it can have one of two values: `0` or `1`. These values represent the two states of a binary system, which is the foundation of all digital computing.

in programming and computer science, a byte is a unit of digital information that typically consists of 8 bits.

in other words, bits and bytes are units used to measure the size of digital files and data.
- Bit: The smallest unit of data in computing, represented as a binary value of either `0` or `1`. It is often used to measure data transfer rates (e.g., kilobits per second).
- Byte: A group of 8 bits, commonly used as a basic unit of storage in computers. Bytes are typically used to measure file sizes (e.g., kilobytes, megabytes, gigabytes).

To summarize:
- 1 byte = 8 bits
- File sizes are usually expressed in bytes and its multiples (e.g., KB for kilobytes, MB for megabytes, GB for gigabytes).


***Binary*** refers to the base-2 numeral system, which uses only two symbols: `0` and `1`. This system is fundamental to computer science and digital electronics because it aligns with the way computers operate at a low level.

Key Points about Binary in Programming:

1. Data Representation: 
   - All data in computers, including numbers, characters, images, and sounds, is ultimately represented in binary form. For example, the decimal number 5 is represented as 101 in binary.

 binary is a numeric system that contains only two digits which are `0` and `1` and  bits and bytes are units for measuring files size or data transfer rate speed which their measuring system is based how many `0` and `1` a file has, so consider you want to measure 1kg of potatoes, those potatoes are `0` and `1` (binary system digits) and that 1kg which is a unit for measuring the weight is like the bit and bytes and this 1kg is 1kg because of the numbers of potato we're weighing.
 
when we say a file is 8 bit, it means it has 8, `0` or `1`s. so a 8 bit file is like a number with 8 digits that these digits are `0` or `1`s. based on the probability subject at high school a 8 digit number which each digit is whether `0` or `1` can have 256 possibility for different numbers, since there is 2 possibility for each digit and we have 8 digit, so we have to multiply eight 2's together which result is `256`.

- a binary number is a number which only has `0` and `1`s. 

- a 25KB (kilo byte) means 25\*1000 (kilo)\*8 (byte to bit conversion)=200000 bit which means if a file size is 25KB it contains 200000, `0` and `1`s or this file is like a 200000 digit number that each digit is either `0` or `1`.

- a hexadecimal number is a number which its digits can vary from `0` to `F`.

 While some ASCII characters could theoretically be represented with fewer bits (e.g., 3 bits can represent up to 8 values), using a full byte allows for easier manipulation and storage of data. It avoids complications that would arise from variable-length encoding schemes when processing text. Computers are designed to process data in bytes. A byte is the smallest addressable unit of memory in most computer architectures. By using a full byte for each ASCII character, it simplifies memory addressing and access patterns, The reason computers reserve 1 byte (8 bits) for each ASCII character, even though some characters can be represented with fewer bits, is primarily due to standardization and efficiency in data processing.

Computers store everything as 1s and 0s, right? That's called binary and like you'd have 10 digits in decimal or 16 digits in hexadecimal, in binary we have just two - 0 and 1 - and you would count like 0,1,10,11,100,101,110,111,1000,... and since 16 = 2\*2\*2\*2 , it turns out that biggest hexadecimal digit is equal to a binary number with 4 digit or an number with four digits that each digit can be `0` or `1` (since each digit in 4 digit number in binary can be either `0` or `1`, so there are 16 possibilities for different numbers, so you can display a four digit binary number or a 4-bit number with just a single hexadecimal digit). So we use hexadecimal to write binary numbers but shorter. In particular (I'll prefix binary with 0b): 0xF = 0b1111 0xFF = 0b11111111

so basically hexadecimal is  4 times lighter in its maximum (I use term maximum because a hexadecimal digit like `8` only represent a 3-bit number 8=2\*2\*2 which is 3 times shorter than binary) than binary i.e. each hexadecimal digit can represent up to 4 binary digit next to each other for example: `F`(hexadecimal)=`1111`(binary).

this shortening doesn't have any impact on computer calculation , since at the endo f the day, the computer only processes binary and this shortening is useful for humans since it reduces confusion while seeing these number in hexadecimal than binary.

there is a `0x` before the hexadecimal numbers which is a specification for hexadecimal numbers and a hexadecimal format is `0xXXXXXXXXX` which the `0x` is to specify the hexadecimal number and other `XXXXX` is to represent hexadecimal digits.

- hexadecimal numbers can have a infinite value and not limited to 255 numbers, for showing numbers greater than 255, a digit gets added to the hexadecimal format like 0x23F and so on.

- for displaying a byte we need two hexadecimal number because a hexadecimal digit can represent up to 4-bit or four `0`and `1`, since a byte is 8-bit or eight `0` and `1`, then we have like 10101001 which each 4 digits can be replaced by a hexadecimal number i.e. `1F`, so for displaying a byte we need 2 hexadecimal digit. 

#### why ASCII table character takes 1 byte (8 bit) while there are 128 character in this table (128=7 bit)
The reason most computers reserve 1 byte (8 bits) for ASCII characters, despite the fact that the standard ASCII set only includes 128 characters (which can be represented with 7 bits), is primarily due to historical and practical considerations:
1. Byte Alignment: Computers are designed to process data in chunks called bytes, which are typically 8 bits. Using a full byte for each character simplifies memory addressing and data manipulation. It allows for efficient access and processing since most computer architectures are optimized for handling data in byte-sized units.

2. Extended ASCII: The 8th bit in a byte allows for the representation of additional characters beyond the standard ASCII set. This leads to what is often referred to as "extended ASCII," which includes an additional 128 characters (from 128 to 255). These can include various symbols, accented letters, and other special characters that are useful in different languages and applications.

#### why we use byte over bit for file size unit?
1. Grouping of Bits: A byte typically consists of 8 bits. This grouping allows for more efficient representation of data. For example, a single byte can represent 256 different values (from 0 to 255), which is sufficient for representing a wide range of characters in text (like ASCII) and other data types.

2. Ease of Use: Working with bytes rather than individual bits simplifies programming and data manipulation. Many data types (like integers, characters, and floating-point numbers) are defined in terms of bytes rather than bits, making it easier for programmers to understand and work with data.

3. Memory Addressing: Most computer architectures are designed to address memory in terms of bytes rather than bits. This means that memory is organized into byte-addressable units, making it more efficient to read and write data.

4. Standardization: The byte has become a standard unit for measuring data storage and transmission (e.g., kilobytes, megabytes). This standardization helps in communicating the size of files and memory capacities more intuitively.

5. Performance Considerations: Modern processors are optimized to handle data in chunks that are multiples of bytes (often 32 or 64 bits). Using bytes aligns with the architecture's design, leading to better performance when processing data.

6. Data Types: Many programming languages define their basic data types (like char, int, float, etc.) based on bytes rather than bits, which makes it easier for developers to work with these types without needing to manage individual bits manually.

In summary, while bits are the fundamental building blocks of digital information, using bytes as a higher-level unit provides practical advantages in terms of efficiency, ease of use, standardization, and alignment with computer architecture.


#### why we use hexadecimal numbers to represent binaries and not a system with more digits like a system with 128 digits?
Hexadecimal (base-16) is commonly used to represent binary numbers for several practical reasons, which make it more efficient and manageable than using a system with many more digits, such as a base-128 system. Here are some key points explaining why hexadecimal is preferred:

1. Compact Representation: Hexadecimal can represent a larger range of values with fewer digits compared to binary. Each hexadecimal digit corresponds to four binary digits (bits). For example, the binary number 1111 can be represented as F in hexadecimal. This compactness makes it easier to read and write large binary numbers.

2. Ease of Conversion: Converting between binary and hexadecimal is straightforward because each hex digit directly maps to a 4-bit binary sequence. In contrast, converting between binary and a base-128 system would be more complex, requiring more calculations and potentially leading to errors.

3. Human Readability: Hexadecimal is easier for humans to read and understand than long strings of binary digits. A base-128 system would produce even longer strings that would be cumbersome for programmers and engineers to work with.

4. Standardization: Hexadecimal has become a widely accepted standard in computing, particularly in programming, memory addressing, and color representation in graphics (e.g., HTML color codes). This standardization means that tools, documentation, and practices are already established around the use of hexadecimal.

5. Simplicity in Representation: Using 16 symbols (0-9 and A-F) allows for a simple representation without needing an extensive set of characters or symbols that would be required for higher bases like 128.

6. Error Reduction: Fewer digits reduce the likelihood of errors when entering or reading values. Longer representations increase the chance of mistakes due to misreading or miswriting characters.

In summary, we can achieve the best performance in our computations with hexadecimal system with lower number of digits which reduces complication and processing in calculation and computation. while it is theoretically possible to use a base-128 system or any other higher base for representing binary data, the practicality of using hexadecimal—due to its compactness, ease of conversion, readability, standardization, simplicity, and error reduction—makes it the preferred choice in computing contexts.

#### why each byte is 8 bit?
The choice of 8 bits for a byte is largely historical and practical, stemming from the evolution of computer architecture and data representation. Here are some key reasons why 8 bits became the standard size for a byte:

1. Historical Context: Early computers used various bit sizes for bytes, including 4, 6, and 9 bits. However, as technology evolved, the 8-bit byte became more common due to its balance between complexity and capability.

2. Character Representation: An 8-bit byte can represent 256 different values (from 0 to 255). This range is sufficient to cover standard character sets like ASCII (which uses 7 bits) and extended character sets that require up to 256 characters. This made it practical for text representation in computing.

3. Alignment with Hardware: Many early microprocessors were designed with an architecture that efficiently handled data in chunks of 8 bits. Using an 8-bit byte allowed for easier manipulation of data in registers and memory.

4. Memory Efficiency: An 8-bit byte allows for efficient use of memory when storing small integers or characters. It strikes a good balance between being large enough to represent a wide range of values while still being small enough to conserve memory space.

5. Standardization: As computing technology advanced, the industry began to standardize on the use of the 8-bit byte, leading to widespread adoption across different systems and platforms.

6. Compatibility: The adoption of the 8-bit byte facilitated compatibility among different hardware and software systems, making it easier for developers to create applications that could run on various machines without modification.

In summary, while there is no inherent reason why a byte must be exactly 8 bits, historical developments in computing led to its widespread adoption as a practical compromise between efficiency, capability, and compatibility.

#### do same letters in different unicode encoding system have a different binary number?
the same letters can have different binary representations in different Unicode encoding systems. This is because different encoding systems may represent the same character using different byte sequences. Below are some examples of characters encoded in various encoding systems, including UTF-8, UTF-16, UTF-32, and other encodings like ISO-8859-1 and Windows-1252.

Example Character: `é` (Latin Small Letter E with Acute)
1. UTF-8
   - Hexadecimal: `C3 A9`
   - Binary: `11000011 10111001`

2. UTF-16 (Little Endian)
   - Hexadecimal: `E9 00`
   - Binary: `11101001 00000000`

3. UTF-32 (Little Endian)
   - Hexadecimal: `E9 00 00 00`
   - Binary: `11101001 00000000 00000000 00000000`

4. ISO-8859-1
   - Hexadecimal: `E9`
   - Binary: `11101001`

5. Windows-1252
   - Hexadecimal: `E9`
   - Binary: `11101001`

Example Character: `中` (Chinese Character for "Middle")

1. UTF-8
   - Hexadecimal: `E4 B8 AD`
   - Binary: `11100100 10111000 10101101`

2. UTF-16 (Little Endian)
   - Hexadecimal: `AD 4E`
   - Binary: `10101101 01001110`

3. UTF-32 (Little Endian)
   - Hexadecimal: `AD 4E 00 00`
   - Binary: `10101101 01001110 00000000 00000000`

4. ISO-8859-1 
   Note: This character cannot be represented in ISO-8859-1 as it only supports Western European characters.

5. Windows-1252 
   Note: Similar to ISO, this character cannot be represented in Windows-1252.

Summary
As shown in the examples above, the same character can have different hexadecimal and binary representations depending on the encoding system used.

#### why everything is in binary in computers?
Everything in computers is in binary primarily due to the following reasons:

1. Simplicity of Design: Binary systems use only two states (`0` and `1`), which simplifies the design of electronic circuits. Transistors, the building blocks of modern computers, can easily represent these two states as "off" (`0`) and "on" (`1`).

2. Reliability: Binary representation is more robust against noise and signal degradation. In a binary system, even if a signal is slightly distorted, it can still be interpreted correctly as long as it remains within the range that represents `0` or `1`.

in a nutshell because the electronic circuits and devices are the components of the computers and the main element in these circuits are transistors, the transistors have gates which the opening and closing of these gates can be defined with binary (`0` and `1`) which this simple numeric system reduces the complexity of calculation and processes meanwhile gives the best output.

#### How can another unicode encoding system designed for a specific language like Hebrew (something rather than English), specify only 1 byte to each of that language letters while the first 128 binary numbers are allocated to ASCII table characters?
In all of the unicode encoding system, the first 128 (0-127) are reserved for ASCII table members with the same exact order, in UTF-8 the rest of the places to reach a byte (128-255) can be occupied by some currency marks like `$`, euro or pound or some other Latin letters (since this encoding system primarily focuses on English language), in a encoding system like ISO 8859-8 which is designed specifically for Hebrew language, the remaining from (128-255) allocates to Hebrew language, that's why in encoding system like ISO 8859-8 each Hebrew character occupies  1 byte but in a encoding system like UTF-8 those Hebrew characters occupy 2byte or more due to those letters location and ordering in that encoding system and binary number that encoding system assigns to that letter which increase or decrease the size of that letter.
so English letters due to the application in coding which is the letter and alphabet we type and code always has the same position in all of the encoding system and uses the least amount of storage because we use it often, we don't want our files to get too large.

Character: "A"
1. UTF-8
   - Hexadecimal: 41
   - Binary: 01000001

2. UTF-16 (Little Endian)
   - Hexadecimal: 41 00
   - Binary: 01000001 00000000

3. UTF-32 (Little Endian)
   - Hexadecimal: 41 00 00 00
   - Binary: 01000001 00000000 00000000 00000000

4. ISO-8859-1
   - Hexadecimal: 41
   - Binary: 01000001

5. Windows-1252
   - Hexadecimal: 41
   - Binary: 01000001

as you can see in [this link](https://www.eso.org/~ndelmott/ascii.html),  letter`A` has the same hexadecimal and binary number in ASCII table which has in other encoding system we've mentioned above.

in character encoding systems, the way characters are represented in binary and how much space they occupy can vary significantly between different encodings. Let's break down your question regarding ISO-8859-8 and UTF-8, particularly in relation to Hebrew letters.

Character Encoding Basics

1. ASCII: The ASCII encoding uses 7 bits to represent characters, which allows for 128 unique characters (0-127). Each character occupies 1 byte (8 bits) in memory.

2. ISO-8859-8: This is an 8-bit character encoding that supports Hebrew characters. It extends the ASCII set by using the additional bit to represent more characters, allowing for a total of 256 unique values (0-255). In ISO-8859-8:
   - The first 128 values (0-127) are identical to ASCII.
   - The next range (128-255) is used for Hebrew letters and some additional symbols.

3. UTF-8: This is a variable-length encoding system that can represent every character in the Unicode standard. It uses one or more bytes per character:
   - Characters from the ASCII range (0-127) are represented with a single byte.
   - Characters outside this range, including many Hebrew letters, may require two or more bytes.

How Hebrew Letters Are Stored

In ISO-8859-8:
- Each Hebrew letter is assigned a specific code point within the range of 128 to 255.
- For example, if a specific Hebrew letter corresponds to the value 0xE1 in ISO-8859-8, it will be stored as 11100001 in binary form.
  
This means that each Hebrew letter occupies exactly 1 byte when encoded in ISO-8859-8 because it fits within the single-byte structure of this encoding scheme.

Comparison with UTF-8

In UTF-8:
1. A basic Latin character would still take up 1 byte.
2. However, many Hebrew letters would take up 2 bytes or more because they fall outside of the basic ASCII range and require additional bits for representation.

Summary

To summarize:
1. In ISO-8859-8, each Hebrew letter occupies exactly 1 byte, as it is designed specifically for languages that use those characters.
2. The storage of these letters occurs directly within the allocated byte values defined by this encoding scheme.
3. In contrast, UTF-8 uses a variable-length approach where some characters may take up more than one byte depending on their Unicode code points.

This design allows ISO encodings like ISO-8859 series to be efficient for specific languages while UTF encodings provide broader support across multiple languages at the cost of potentially increased storage requirements for certain characters.

In UTF-8 encoding, the first 128 code points (0-127) correspond directly to the ASCII character set. The remaining code points from 128 to 255 are used for various characters from different character sets and languages, as well as additional symbols.

Here’s a brief overview of what occupies the code points from 128 to 255 in UTF-8:

1. Extended Latin Characters: Many characters used in Western European languages, such as accented letters (e.g., é, ñ, ü), are included in this range. These characters are often part of ISO-8859-1 (Latin-1) and other extended Latin encodings.

2. Special Symbols: This range includes various punctuation marks, currency symbols (like the Euro sign €), and other special characters.

3. Control Characters: Some control characters that were not included in the original ASCII set may also be represented here.

4. Other Language Scripts: Depending on the specific implementation or standard being followed, some code points may be allocated to characters from other scripts or languages that require additional glyphs beyond those provided by ASCII.

it's important to note that UTF-8 is a variable-length encoding system; while ASCII uses one byte per character (0-127), UTF-8 can use one to four bytes for other characters beyond this range. For example:
- Characters from U+0080 to U+07FF use two bytes.
- Characters from U+0800 to U+FFFF use three bytes.
- Characters from U+10000 and above use four bytes.

Thus, while the first 128 positions are straightforwardly mapped to ASCII, the subsequent positions encompass a wide variety of characters based on different linguistic and symbolic needs.

#### do 0 behind of a digit counts like in decimal numbers i.e. in 00011001, those 3 zeros behind 1 count as a bit or not?
Yes, in binary representation, leading zeros (the zeros that come before the first '1') do not count towards the value of the number but do count as bits. For example, in the binary number 00011001, there are 8 bits total, including the three leading zeros. 

So to clarify:
- The binary number `00011001` has 8 bits.
- The value of this binary number is equivalent to the decimal number 25, but the leading zeros are still counted as part of its bit length. 

In general, when discussing bit length or size in digital systems, all bits are counted regardless of their value.

we know that ASCII table members in any encoding system will occupy 1 byte, that's why in ***[here](https://www.eso.org/~ndelmott/ascii.html)***
each letter contains eight `0` and `1` in its binary format and two digit in its hexadecimal one despite of being able to display each letter as minimum as its need for example for digit `3` we could display as `110011` instead of `00110011` and avoid 2 extra bits but since each ASCII table member occupies 1 byte, that why each letter represents in a 8 digit binary number and a 2 digit hexadecimal number while when we want to display these character, since the amount of space they occupy doesn't matter, we can show them with their minimum amount like we can display digit `3` as `110011` and not `00110011`.

#### byting & byte order matters in interpretation
for example for letter A, the binary number in different encoding systems is as below: 
Character: "A"
1. UTF-8
   - Hexadecimal: 41
   - Binary: 01000001

2. UTF-16 (Little Endian)
   - Hexadecimal: 41 00
   - Binary: 01000001 00000000

3. UTF-32 (Little Endian)
   - Hexadecimal: 41 00 00 00
   - Binary: 01000001 00000000 00000000 00000000

4. ISO-8859-1
   - Hexadecimal: 41
   - Binary: 01000001

5. Windows-1252
   - Hexadecimal: 41
   - Binary: 01000001

as you can see, binary number in every encoding system is same except for UTF-16 and UTF-32     (the reason we have 01000001 00000000 instead of 00000000  01000001 is because of BOM which I explain it further, in another point but in another version of UTF-16 which is BE (Big Endian), we have 00000000 01000001 for letter A, I told you this to show that the binary value is the same in all of the encoding systems and the reason for their difference is because of the number of bytes and BOM), so we know that first 128 place in any encoding system is reserved ASCII table members but it doesn't mean that an ASCII letter can be re-opened in any encoding system without replacement character and issue, the reason is byting and BOM, so we know that every encoding system reserves its first 128 place for ASCII table characters due to their popularity and  high application (English is highest spoken language in the world and that's the language all developers code their programming syntax), so letter A place in every encoding system is 65 (in decimal number), so if we re-open `A` in any encoding system, we see `A`, but NO! why? because the binary value and placement of a character is only one of the factors, in ASCII table each character occupies 1 byte and that why every character is typed in a 8 digit format as its binary number, same situation applies to UTF-8 and each ASCII table character occupies 1 byte, so if you type `A` in ASCII encoding table and re-open the same text with UTF-8, you wont face any issue.
in some encoding system like UTF-16 the byting is different due to their special behavior they supposed to have for specific applications, in uTF-16 each ASCII table character occupies 2 byte, that why when you have `A` in UTF-8 and re-open it with UTF-16, the UTF-16 expects 2 byte but because in UTF-8 this letter has 1 byte, the UTF-16 is unable to encode this letter despite of same binary ***value*** (which is equal 41 is hexadecimal and 65 in decimal) for the same letter and if you type `A` in UTF-16 and re-open with UTF-8, the character will misinterpret because the UTF-8 expects one byte but you gave it 2 bytes, so it won't display `A`.

another reason for encoding corruption in ASCII letter is BOM (I explain it in subsequent points),
in UTF-16, we have two ways to display the binary number which we call it BOM, one of them called little endian (LE) which in that we place the least significant byte in the right-hand side (I think by least significant number, it means the smallest number based on value) for example the letter `A` in UTF-16 LE is `01000001 00000000`, the another BOM called Big Endian (BE) which we place the most significant byte (I think it means the biggest binary number) in right-hand-side, so for letter `A`, we have  `00000000  01000001`, you see these two binary numbers in UTF-16 LE and UTF-16 BE have the same binary value (in calculating the binary value, I consider everything in BE even the LE one), same number of bytes (both have 2 bytes) but because the order of their byte placement is different, if we type `A` in UTF-16 BE and re-open it inUTF-16 LE, the letter `A` misinterprets and instead of `A`, we see some broken character and vice versa.

as you saw in description above, byting and byte order along side the placement of that character in the encoding system (binary value) is important for a correct interpretation.

in a encoding system like UTF-16  we have BOM and in UTF-8 we don't have anything as BOM and everything is like a typical decimal (rank or placement of the character in the encoding system) to binary number conversion.

in a encoding system like ISO 8859-8 which belongs to Hebrew language and has nothing to do with English, since its 128 first places are reserved for ASCII table characters. and like UTF-8, each ASCII table character occupy 1 byte, so if I type `A` in ISO 8859-8  and re-open that text in UTF-8, I see `A` without any issue, because the letter `A` has the same place in both UTF-8 and ISO 8859-8 system, both of the encoding system have the same byting order and they occupy the same byte.
despite of different and distant purposes in each encoding system, they can interpret ASCII table character in each other correctly because of the reasons we mentioned earlier.

#### what's the difference between utf-8 and utf-16 and utf-32?
UTF-8, UTF-16, and UTF-32 are all character encoding schemes used to represent Unicode characters, but they differ in how they encode these characters and the amount of memory they use. Here’s a breakdown of the differences:

1. UTF-8
- Byte Size: Uses 1 to 4 bytes per character.
  - ASCII characters (U+0000 to U+007F) are encoded in 1 byte.
  - Characters from U+0080 to U+07FF use 2 bytes.
  - Characters from U+0800 to U+FFFF use 3 bytes.
  - Characters from U+10000 to U+10FFFF use 4 bytes.
- Compatibility: Backward compatible with ASCII; any valid ASCII text is also valid UTF-8 text.
- Usage: Commonly used on the web and in many programming languages due to its efficiency with English text.

1. UTF-16
- Byte Size: Uses either 2 or 4 bytes per character.
  - Most common characters (U+0000 to U+D7FF) are encoded in 2 bytes.
  - Supplementary characters (U+D800 to U+10FFFF) are encoded using a pair of surrogate halves, totaling 4 bytes.
- Endianness: Can be stored in big-endian or little-endian format, which affects how the byte order is interpreted.
- Usage: Often used in environments like Windows and Java.

1. UTF-32
- Byte Size: Uses exactly 4 bytes (32 bits) for every character, regardless of its value.
- Simplicity: Simplifies indexing since each character takes up the same amount of space; however, it is less memory efficient for texts that primarily consist of ASCII or other characters that could be represented with fewer bytes in UTF-8 or UTF-16.
- Usage: Less common for storage but can be useful for internal processing where fixed-width representation is beneficial.

Summary
In summary:
- UTF-8 is space-efficient for texts primarily using ASCII and variable-length for other characters.
- UTF-16 uses more space than UTF-8 for ASCII but can be more efficient for certain scripts that require many non-Latin characters.
- UTF-32, while simple and consistent in size, uses more memory overall compared to both UTF-8 and UTF-16.

The choice between these encodings often depends on specific application requirements regarding compatibility, memory usage, and performance.

#### BOM & endianness 
he difference in the binary representation of the letter "A" between UTF-8 and UTF-16 is due to how these encoding schemes are designed.

1. ASCII and UTF-8:
   - The letter "A" has an ASCII value of 65, which is represented in binary as 01000001. 
   - UTF-8 is backward compatible with ASCII for the first 128 characters (0-127). Therefore, the UTF-8 representation of "A" remains 01000001.

2. UTF-16:
   - UTF-16 uses a different structure. It typically represents characters using 2 bytes (16 bits). For characters in the Basic Multilingual Plane (BMP), like "A", it uses a single 2-byte code unit.
   - In UTF-16, the character "A" is represented as 00 41 in hexadecimal, which corresponds to 00000000 01000001 in binary.
   - However, when stored or transmitted, it may be prefixed with a Byte Order Mark (BOM) to indicate endianness (byte order). The BOM for little-endian systems is FF FE, while for big-endian systems it is FE FF.

Endianness
The confusion might arise from endianness:

- Little-endian: The least significant byte comes first. So for "A", it would be stored as:
  `
  01000001 00000000
  `
  
- Big-endian: The most significant byte comes first. So for "A", it would be stored as:
  `
  00000000 01000001
  `

Summary
So, depending on whether you're looking at little-endian or big-endian encoding of UTF-16, you can see different orders of bytes. In practice:

- Little-endian: 01000001 followed by 00000000
- Big-endian: 00000000 followed by 01000001

Make sure to check which endianness is being used when interpreting the binary data!

#### what kind of unicode encoding system windows 10 uses?
Windows 10 primarily uses UTF-16 as its default Unicode encoding system for internal string representation in the Windows API. This means that most applications and system components handle text using UTF-16 encoding, which allows for a wide range of characters from various languages and scripts.

#### What is Basic Multilingual Plane (BMP)?
The Basic Multilingual Plane (BMP) is the first of the 17 planes (a layer that holds specific code points in itself) defined in the Unicode standard, specifically covering code points from U+0000 to U+FFFF. This range includes a wide variety of characters used in many languages, as well as control characters and symbols.

-  Character Coverage: The BMP contains characters for most of the world's writing systems, including Latin, Greek, Cyrillic, Arabic, Hebrew, and many others. It also includes punctuation marks, mathematical symbols, and various other character sets.

#### why windows 10 uses UTF-16 as its encoding system while they can use    UTF-8 which is more memory efficient?
Windows 10 primarily uses UTF-16 for several reasons, despite UTF-8 being more memory-efficient in many scenarios:

2. Legacy Compatibility: Windows has a long history of using UTF-16, dating back to       Windows NT. Many applications and APIs were built around this encoding, and changing the underlying encoding would require significant changes to existing software.

3. Unicode Support: UTF-16 can represent all Unicode characters using a fixed number of code units (2 bytes for most common characters). This makes it easier to handle certain operations, such as string manipulation and indexing, especially for languages that use a lot of non-Latin characters.

4. Performance Considerations: For many applications that primarily deal with languages that fall within the [[JavaScript + misc programming concepts#what is Basic Multilingual Plane (BMP)?|Basic Multilingual Plane (BMP)]], UTF-16 can be more efficient in terms of processing speed. Operations like string length calculation and character access can be faster with fixed-width encodings, basically what it's said in this point is, because windows 10 is an application that too many languages can be used and displayed in it like Arabic, Persian, Hebrew and etc. we need to deal lots of characters, in UTF-16, all of the characters that are part of 1 byte and   2 byte and almost 80% of 3 byte character of UTF-8 encoding system, all of them occupy        2 byte in UTF-16 (drawback of this UTF-16 system to UTF-8 is, for 1 byte characters in UTF-8, we have to reserve 2 byte in UTF-16 but the bonus is for almost 80% of 3 byte characters in UTF-8, we reserve 2 byte), so this UTF-16 encoding system is useful in an application like windows 10 which deals with lots of languages, and when we deal with lots of languages, if we have a fixed amount of byte for all of the characters, it would improve the speed of calculation and processing.  

5. API Design: The Windows API was designed with UTF-16 in mind, which means that many system calls expect strings to be in this format. Changing this would require extensive redesigns of the API and could lead to compatibility issues.

6. Memory Usage Patterns: While UTF-8 is generally more memory-efficient for ASCII characters (1 byte per character), it can become less efficient for languages with larger character sets or when dealing with a lot of non-Latin scripts, where characters may take up 3 or 4 bytes in UTF-8 compared to 2 bytes in UTF-16.

In summary, while UTF-8 has its advantages, particularly for web applications and data interchange formats where space efficiency is critical, the choice of UTF-16 by Windows is largely driven by historical context, performance considerations for specific use cases, and compatibility with existing software ecosystems.

#### why someone use UTF-16 as its encoding system while they can just use    UTF-8?
Choosing between UTF-8 and UTF-16 as an encoding system depends on various factors, including the specific use case, compatibility requirements, and performance considerations. Here are some reasons why someone might choose UTF-16 over UTF-8:

1. Fixed Width for Certain Characters: 
   - UTF-16 uses a fixed width of 2 bytes for most common characters (those in the Basic Multilingual Plane), which can simplify certain types of processing, such as indexing or calculating string lengths.

2. Compatibility with Legacy Systems:
   - Some older systems and APIs were designed around UTF-16 (e.g., Windows APIs). Using UTF-16 can facilitate easier integration with these systems.

3. Performance Considerations:
   - In environments where characters are predominantly from the BMP (Basic Multilingual Plane), using UTF-16 can lead to better performance in terms of memory access patterns and processing speed since it avoids the variable-length nature of UTF-8.

4. Language Support:
   - For applications that primarily deal with languages that have a lot of characters outside the ASCII range (like many Asian languages), using UTF-16 may result in less overhead compared to UTF-8, where many characters would require more than 2 bytes.

5. Ease of Use in Certain Programming Languages:
   - Some programming languages or frameworks (like Java) use UTF-16 natively for their string representations, making it more convenient to work with strings without needing to convert between encodings.

6. Memory Alignment:
   - In some cases, using a 2-byte encoding like UTF-16 can align better with certain hardware architectures, potentially leading to performance benefits due to reduced cache misses or better memory alignment.

7. Data Interchange Formats:
   - Certain data interchange formats or protocols may specify or prefer UTF-16 encoding for consistency or historical reasons.

While both encodings have their advantages and disadvantages, the choice often comes down to specific application needs and existing infrastructure considerations.

#### What is the most common encoding system around the web for websites?
The most common encoding system used for websites is UTF-8 (Unicode Transformation Format - 8-bit). UTF-8 is widely adopted because it can represent any character in the Unicode standard, making it suitable for internationalization and supporting a vast array of languages and symbols. It is also backward compatible with ASCII, which makes it a versatile choice for web content.

Most modern web technologies, including HTML and CSS, default to UTF-8 encoding, and it's recommended to specify this encoding in the HTML document using the following meta tag:

```HTML
<meta charset="UTF-8">
```

This ensures that browsers correctly interpret the text content of the webpage.

#### Why website choose UTF-8 as their encoding system?
Websites often choose UTF-8 as their encoding system for several important reasons:
1. Universal Character Support: UTF-8 can represent every character in the Unicode standard, which includes characters from virtually all writing systems in use today. This makes it ideal for websites that need to support multiple languages and special characters.

2. Compatibility: UTF-8 is backward compatible with ASCII, meaning that any valid ASCII text is also valid UTF-8 text. This compatibility ensures that older systems and software that only understand ASCII can still process UTF-8 encoded data without issues.

3. Efficiency: For texts primarily composed of ASCII characters (like English), UTF-8 is efficient because it uses one byte per character. For other characters, it uses a variable number of bytes (up to four), which helps balance storage efficiency and the ability to represent a wide range of characters.

4. Widespread Adoption: UTF-8 has become the dominant character encoding on the web, supported by all major browsers and web technologies. This widespread adoption means that developers can rely on consistent behavior across different platforms and devices.

5. Ease of Use: Many programming languages and frameworks have built-in support for UTF-8, making it easier for developers to work with text data without worrying about encoding issues.

6. Standardization: The World Wide Web Consortium (W3C) recommends using UTF-8 as the default character encoding for HTML and XML documents, promoting its use across the web.

7. Avoiding Encoding Issues: Using a single encoding like UTF-8 helps prevent common problems associated with mixed encodings, such as garbled text or errors when displaying content.

Overall, these factors make UTF-8 a practical choice for modern web development, ensuring broad compatibility and ease of use while supporting diverse linguistic needs.

#### Why websites choose UTF-8 as their encoding system rather than               UTF-16?
Websites typically choose UTF-8 as their encoding system over UTF-16 for several reasons:
1. Compatibility: UTF-8 is backward compatible with ASCII, which means that any valid ASCII text is also valid UTF-8 text. This compatibility makes it easier to handle legacy systems and data that were originally encoded in ASCII.

2. Efficiency: For texts primarily composed of ASCII characters (like English), UTF-8 is more space-efficient because it uses only one byte per character for these characters, while UTF-16 uses at least two bytes. This can lead to significant savings in storage and bandwidth for many web pages.

3. Variable Length Encoding: UTF-8 uses a variable-length encoding scheme, where characters can be represented using one to four bytes. This allows it to efficiently encode a wide range of characters from different languages without wasting space on single-byte representations for non-Latin scripts.

4. Widespread Adoption: UTF-8 has become the dominant character encoding on the web, supported by all major browsers and web technologies. This widespread adoption means that developers are more likely to encounter and work with UTF-8, leading to a network effect where its use reinforces itself.

5. Simplicity in Handling: Many programming languages and libraries have built-in support for handling UTF-8 strings, making it easier for developers to work with text data without worrying about byte order marks (BOM) or other complexities associated with multi-byte encodings like UTF-16.

6. Interoperability: Since most web protocols (like HTTP) and formats (like JSON and XML) are designed with UTF-8 in mind, using this encoding ensures better interoperability across different systems and platforms.

7. Avoiding Byte Order Issues: UTF-16 can have issues related to byte order (endianness), which can complicate data exchange between systems that may use different byte orders. In contrast, UTF-8 does not have this issue since it has a consistent byte order.

Overall, these factors make UTF-8 a more practical choice for web development compared to     UTF-16, especially given the global nature of the internet and the diversity of languages used online.

#### I have created a plain text file in vs code like "hi, I'm Lome" and it's encoding is UTF-8, I know that windows 10 uses UTF-16, and I know that If I want to open a UTF-8 text with UTF-16 encoding system, the text with be displayed in replacement character and broken character, so why when I open this text file with windows 10 note pad instead of broken character and replacement character, I see the "hi I'm Lome" text? if note pad detects utf-8, so why it doesn't detect ISO 8859-8 encoding system and when I I type some Hebrew text like אָלֶף־בֵּית עִבְרִ in vs code while my encoding system is ISO 8859-8 and opens it with note pad, it shows me replacement characters and broken characters?

The behavior you're observing with text encoding in Windows Notepad can be explained by how Notepad handles different encodings and the presence of a Byte Order Mark (BOM).

UTF-8 vs. UTF-16

1. UTF-8 Encoding: 
   - When you create a text file in UTF-8, it can be opened by applications that support this encoding without issues. If the file does not have a BOM, Notepad will still recognize it as UTF-8 based on the content.
   - If you open a UTF-8 encoded file in an application that expects UTF-16, you may see replacement characters (�) or broken characters because the byte sequences do not correspond to valid UTF-16 characters.

2. Notepad's Behavior:
   - Windows Notepad has improved over time and can automatically detect the encoding of text files. If it detects that a file is encoded in UTF-8, it will display the content correctly.
   - If your file contains valid UTF-8 sequences, Notepad will render them correctly even if it's running on a system that primarily uses UTF-16.

ISO 8859-8 Encoding

1. ISO 8859-8: 
   - This is an 8-bit character encoding for Hebrew characters. If you create a file using ISO 8859-8 and then open it in Notepad without specifying the correct encoding, Notepad may not recognize it as ISO 8859-8.
   - Since ISO 8859-8 uses different byte sequences than those used in UTF encodings, if Notepad interprets these bytes incorrectly (for example, as if they were encoded in another format like UTF-16 or even ASCII), you'll see replacement characters or broken text.

Why Does It Work for Some Encodings but Not Others?

2. Detection Mechanism: 
   - Notepad has built-in heuristics to detect common encodings like UTF-8 and ANSI (which includes various code pages). However, it may not have robust detection for all specific encodings like ISO 8859 series unless explicitly specified.

In summary:
- Your text "hi I'm Lome" displays correctly because it's valid UTF-8 and recognized by Notepad.
- The Hebrew text shows replacement characters when opened as ISO 8859-8 because Notepad does not automatically detect this encoding and defaults to another interpretation.


so basically while windows encodes text in UTF-16 but notepad can detect UTF-8 and has no problem in encoding it, but this detection doesn't apply to other encoding system in notepad, like if you encode a text with ISO 8859-8 which is a encoding system for Hebrew and then open that text file with notepad, because the notepad can't detect ISO 8859-8 encoding system, it's unable to encode it and we see broken characters, the reason notepad has the ability to encode UTF-8 is because of this encoding system popularity but since ISO 8859-8 isn't popular, the developers of notepad didn't bother themselves to add a code to notepad to detect ISO 8859-8.

#### What's the encoding system for HTML,CSS and JavaScript?
we know the encoding system that you save your file in VS code is for our system (as the owner of the file or the developer) and there is a tag in HTML as ```<meta charset="encoding system">``` which its role is to tell the browser how to encode HTML file in the user or person visiting your site, computer i.e. you have encoded an HTML file in your system via VS code in UTF-16, every ASCII character occupies 2 bytes in your computer, in this specific HTML file we have                        ```<meta charset="UTF-8">```, so when the user visits our site every HTML content ( I mention ASCII because it's more straightforward for exampling), those contents get encoded in UTF-8 and each ASCII character occupies 1 byte, so exactly what in a HTML file gets encoded, in terms of encoding in vs code and saving that file in our computer, everything in a file gets encoded. for example:
```HTML
<p class="today">"hi bro"</p>
```
in example above including `p` tag, `class` attribute, the class name which is `today`, the HTML tag content which is "hi bro" gets encoded by our computer as the developer or the owner of the file but when this HTML file wants to be encoded by the user browser and allocate space to itself, the `p` tag and the class attribute and class name (`today`) are part of the code and they get ***executed (not encode)*** by the browser (so you may so why it got encoded in our own pc, because in our pc we don't execute HTML and HTML markup structure is just a plain text outside the browser bounds) and only the "hi bro" which is a string gets encoded by the browser (everything between HTML tag is a string,```<p>23</p>```, 23 in this example is an string).

for CSS files in both browser and our file everything from CSS property name and Property value gets encoded, for example:

```CSS
p{
color:red;
}
```
the whole code above including `p`,`color`,`red` and `{}`, all of them get encoded by browsers (the reason why HTML tags don't get encoded but CSS properties do, its something that browsers have set and they have decided that everything works best in this way). the encoding system they accept depends on different parameters.
in CSS we have `@charset` which specifies the encoding system of the CSS which browser should encodes (for the file in our own PC, that's VS code which decides), example:

```CSS
@charset "UTF-8";

p{
color:red;
}
```
for more info about this CSS rule, please read ***[this link](https://developer.mozilla.org/en-US/docs/Web/CSS/@charset)*** .

in most of CSS files I've seen, I haven't witnessed that anybody use this `@charset` in their CSS, so how the CSS file encodes its content on a browser? in absence of the `@charset` rule, if the CSS file is linked (of course the CSS file we create is linked to our HTML, the distinguish I've made in here by using word `link` is because of the some CSS approach like CDN which we can see their application in tailwind) to our HTML file via `<link` tag, the CSS file will adopt the encoding system specified by    `meta charset="encoding system"` tag in HTML which usually is `UTF-8`but some say if we don't use `@charset` in our CSS file, the browser automatically chooses `UTF-8` as the encoding system to encode our CSS file, so basically I don't know which statement is correct but one thing which is clear that `@charset` has the precedence to encode our CSS file, then the precedence is either with HTML `<meta charset=encoding system` tag or the browser default `UTF-8`, there is something that has precedence over `@charset` CSS tag for encoding which is the `charset` attribute, we specify in our HTTP headers, this is the quote from [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/@charset#section-content):

> The value given by the `charset` attribute of the `Content-Type:` HTTP header or the equivalent in the protocol used to serve the style sheet.

but this last method is super rare for a CSS file, so we can neglect it.
basically the precedence for CSS file encoding approaches is:
 1. charset attribute in an HTTP header
 2. `@cahrset` in CSS file
 3. `<meta charset="encoding system"` tag in HTML if the CSS file is linked to our HTML via `link` tag or the default UTF-8 by the browsers.

what if we use `tailwind` CDN for our CSS styling? tailwind typically use UTF-8 as its encoding system for CSS and you can change it.

for JavaScript in browsers every ***String*** (by string, I mean everything located between ` `` `,`""` and `''` or in some places like objects that keys are string without any punctual annotation) gets encoded with UTF-16 encoding system because UTF-16 is the default encoding system for JavaScript, what about other data types, I talk about it later and the code parts like `const`,  `function`, `if` and everything basically is part of JavaScript syntax gets ***executed and not encoded*** (again, that's how browsers have decided to things go on) and in the VS code everything gets encoded including the JavaScript syntax.

#### does javascript only encodes its string in UTF-16 or it encodes other data types like array, number and etc. in UTF-16, if javascript only encodes string in UTF-16, what happens to other data types?

JavaScript primarily uses UTF-16 encoding for its string data type. This means that when you work with strings in JavaScript, they are represented in memory using UTF-16 encoding. However, other data types in JavaScript, such as numbers, arrays, objects, and booleans, do not have a specific character encoding like strings do.

Here's a breakdown of how different data types are handled:

1. Strings: As mentioned, strings in JavaScript are encoded using UTF-16. Each character is represented by one or two 16-bit code units (for characters outside the Basic Multilingual Plane).

2. Numbers: JavaScript uses the IEEE 754 standard for representing numbers, specifically double-precision floating-point format (64 bits). This representation does not involve any character encoding like UTF-16; instead, it encodes numeric values directly in binary.

3. Booleans: Boolean values (true and false) are stored as simple binary values (1 for true and 0 for false). There is no character encoding involved.

4. Arrays: Arrays in JavaScript are objects that can hold multiple values of any type (including other arrays). The elements themselves can be of any type (strings, numbers, objects), but the array structure itself does not have an encoding; it simply holds references to those elements.

5. Objects: Objects are collections of key-value pairs where keys are strings (or Symbols) and values can be of any type. The keys are stored as strings using UTF-16 encoding when they are created or accessed.

6. Other Data Types: Other types like null, undefined, and symbols also do not have a specific character encoding associated with them.

In summary, only strings in JavaScript use UTF-16 encoding for their representation. Other data types like numbers and booleans use binary representations appropriate to their types without any character encoding scheme involved.

#### why data types like `undefined`, `null` and `symbol` and etc. in JavaScript doesn't get encoded in terms of encoding systems and unicode  but `boolean` can be encoded while `boolean` doesn't represent textual data?

In JavaScript, data types like undefined, null, and symbol are not directly related to textual representation or encoding systems like Unicode because they serve different purposes in the language. Let's break down the reasoning behind this:

1. Data Types Overview:
   - Primitive Types: JavaScript has several primitive data types, including:
     - undefined: A type with a single value, indicating that a variable has not been assigned a value.
     - null: A type with a single value representing the intentional absence of any object value.
     - boolean: Represents a logical entity and can have two values: true or false.
     - number: Represents numeric values (both integers and floating-point).
     - string: Represents textual data.
     - symbol: A unique and immutable primitive value often used as object property keys.

2. Encoding Systems:
   - Encoding systems like UTF-8 or Unicode are designed to represent characters in text form. They map characters to specific byte sequences for storage and transmission.
   - Data types that represent textual information (like strings) can be encoded because they correspond to characters in a character set.

3. Non-Textual Data Types:
   - Undefined and Null: These types do not represent any character or string; they signify the absence of value or object. Therefore, they do not have an encoding representation because there is nothing to encode.
   - Symbol: This is meant for creating unique identifiers for object properties. It does not represent any textual information, so it also does not require encoding.

4. Boolean Type:
   - While booleans (true and false) do not represent textual data per se, they can be easily represented in binary form (1 for true, 0 for false). This binary representation is fundamental in computing and can be encoded as part of data structures or protocols.

Summary:
- The distinction lies in the purpose of these data types:
  - Textual data types (like strings) need encoding because they represent characters.
  - Non-textual types (like undefined, null, symbol) do not need encoding since they don't correspond to any character or string representation.
  
In conclusion, only those data types that have a direct correlation with text need an encoding system like Unicode; others serve different roles within the language's structure and logic without requiring such representations.

in a nutshell, only strings gets encoded by unicode encoding system, numbers have their own storing system which is not related to encoding system and `boolean` because it is like 0 and 1, its like binary and computer stores them easily and again `boolean` doesn't have anything to do with encoding systems and unicode. other data types like symbol, null, undefined don't get encoded because they don't have any textual content. for data types like function, object and array, they're combination of primitives data types and they follow what rule we've applied on them.

#### if null, undefined, symbol, bigint ,NaN, number,bolean, object, array, function don't get encoded by the unicode encoding system, how do they get stored in user computer and how much space they occupy based on byte?

In JavaScript, different data types are stored in memory in various ways, and their representation can vary based on the environment (like a web browser or Node.js). Here's a breakdown of how each of the mentioned types is typically stored and their approximate memory usage:

1. Null: 
   - Storage: Represents an intentional absence of any object value.
   - Size: Typically occupies 4 bytes (in some environments) or 8 bytes (in others) as a pointer.

2. Undefined: 
   - Storage: Represents a variable that has been declared but not assigned a value.
   - Size: Similar to null, it usually occupies 4 or 8 bytes.

3. Symbol:
   - Storage: A unique and immutable primitive value often used as object property keys.
   - Size: The size can vary, but it generally takes up more space than other primitives due to its uniqueness; around 8 bytes is common.

4. BigInt:
   - Storage: Used for integers larger than Number.MAX_SAFE_INTEGER.
   - Size: The size can vary based on the number's magnitude, but it typically requires at least 8 bytes and can grow larger depending on the value.

5. NaN (Not-a-Number):
   - Storage: A special numeric value representing an undefined or unrepresentable value in floating-point calculations.
   - Size: Occupies 8 bytes since it's stored as a floating-point number.

6. Number:
   - Storage: Represents both integer and floating-point numbers.
   - Size: Always occupies 8 bytes in JavaScript (double-precision floating-point format).

7. Boolean:
   - Storage: Represents true/false values.
   - Size: Typically occupies 4 bytes, though it may be optimized to use less space depending on the implementation.

8. Object:
   - Storage: A collection of properties, which can include functions and other objects.
   - Size: The size varies widely based on the number of properties and their types; overhead for an object itself is usually around 8-16 bytes plus additional space for each property.

9. Array:
   - Storage: A special type of object used for storing ordered collections of values.
   - Size: Similar to objects; overhead is around 8-16 bytes plus additional space for each element stored in the array.

10. Function:
    - Storage: Functions are first-class objects in JavaScript.
    - Size: Functions have overhead similar to objects (around 8-16 bytes), plus additional space for any closures they may capture.

Summary
The actual memory usage can depend on various factors including the JavaScript engine implementation (like V8 in Chrome), optimizations made by the engine, and how variables are managed during execution. 

In general:

- Primitives like null, undefined, boolean, number, NaN, symbol, and bigint have fixed sizes that are relatively small compared to complex structures like objects, arrays, and functions which have variable sizes based on their contents.
  
- Objects and arrays will consume more memory as they grow in complexity due to their dynamic nature.

Note
The above sizes are approximations; actual memory consumption may vary based on specific implementations and optimizations by JavaScript engines.

these byting and spaces, all of them get stored in our PC RAM, I've elaborated them in point below.

#### each ASCII table character in an string occupy 2 bytes in memory in JavaScript, what does this memory mean, by memory we maen RAM or what?

In JavaScript, when we talk about memory usage for strings and characters, we are typically referring to how data is stored in RAM (Random Access Memory) while a program is running. 

Understanding Memory in JavaScript:
1. Character Encoding: 
   - JavaScript uses UTF-16 encoding for strings. In UTF-16, most common characters (like those in the ASCII range) are represented using 2 bytes (16 bits). This means that even though ASCII characters only require 1 byte in standard ASCII encoding, they occupy 2 bytes in JavaScript due to the UTF-16 representation.

2. Memory Allocation:
   - When you create a string in JavaScript, the engine allocates memory in RAM to store that string. The amount of memory allocated depends on the length of the string and its character encoding.
   - For example, a string with 5 ASCII characters would occupy 10 bytes (5 characters × 2 bytes per character).

3. RAM Usage:
   - RAM is where your program's data and instructions are stored while it is running. When you create variables or objects (including strings), they reside in RAM until they are no longer needed and can be garbage collected.

4. Garbage Collection:
   - JavaScript has an automatic garbage collection mechanism that frees up memory that is no longer being used by your program.

Summary:
So when we say each ASCII character occupies 2 bytes in memory in JavaScript, we mean that due to the UTF-16 encoding used by JavaScript for strings, each character takes up 2 bytes of RAM while the program is executing. This is important for understanding how much memory your application might consume based on the strings it handles.

#### How a JSON string gets encoded in JavaScript?
The string you provided is a JavaScript template literal that contains JSON-like content with HTML entities (like &quot; for quotes). However, the encoding of a string in JavaScript is not explicitly defined by the string itself but rather by how it is stored and transmitted.

In JavaScript, strings are typically encoded in UTF-16. This means that when you create a string like your example, it is stored in memory using UTF-16 encoding. However, when you send this data over the network (for example, as part of an HTTP request), it can be encoded in different formats such as UTF-8 or UTF-16 depending on the context and how you handle the data.

To summarize:

1. In Memory: The string is stored as UTF-16.
2. Transmission: It can be encoded as UTF-8 or another encoding based on how it's sent (e.g., HTTP headers might specify Content-Type: application/json; charset=utf-8).

If you're working with JSON data specifically, it's common to encode it in UTF-8 when transmitting over networks because it's more space-efficient for ASCII characters and widely supported.

so because these JSON in JavaScript are string, they get encoded in UTF-16 but if I want to transmit this string over internet (usually we use API in our website to access allowed data from other websites, these data get retrieved as a JSON, so when we want to transmit data in a JSON string with `fetch` method and place our JSON data in our headers body, it is better to set it to UTF-8 for memory efficiency and speed in transmission but when thsi JSON string is going to be used in a website, when the web is opened by the the user and the engine starts to encode the JavaScript, this JSON gets encoded in UTF-16 like other JavaScript code)

#### Why JavaScript encodes string in UTF-16?
JavaScript uses UTF-16 encoding for strings primarily due to historical and practical reasons. Here are some key points explaining this choice:

1. Historical Context: JavaScript was created in the mid-1990s, a time when UTF-16 was becoming a popular encoding format, especially in environments like Windows and Java. The decision to use UTF-16 allowed JavaScript to handle a wide range of characters from different languages, which was important for web development.

2. Character Representation: UTF-16 can represent all Unicode characters using one or two 16-bit code units. Most common characters (like those in the Basic Multilingual Plane) are represented with a single 16-bit unit, while less common characters (like certain emoji or historic scripts) require two units (known as surrogate pairs). This allows JavaScript to efficiently handle a vast array of characters.

3. Compatibility with Other Technologies: Many other technologies and platforms that were prevalent at the time of JavaScript's creation also used UTF-16, making it easier for developers to work across different systems without worrying about character encoding issues.

4. Memory Efficiency: For many Western languages and symbols, using 16 bits per character (as in UTF-16) can be more memory-efficient than using 32 bits per character (as in UTF-32), while still allowing for a wide range of characters.

5. String Manipulation: JavaScript's string methods and operations are designed around the idea of working with code units rather than individual bytes or larger code points, which aligns well with how UTF-16 encodes most common characters.

6. Web Standards: As web standards evolved, maintaining compatibility with existing systems became crucial. Since JavaScript is deeply integrated into web technologies, sticking with UTF-16 helped ensure that existing applications continued to function correctly.

In summary, JavaScript's use of UTF-16 is rooted in historical decisions made during its development and has been maintained for compatibility and efficiency reasons as the language has evolved over time.

#### does JavaScript use UTF-16 for encoding its strings because java use it and JavaScript wanted to copy java (since JAVA is released earlier than JavaScript and JavaScript used the name of Java which was a popular programming language back in then for marketing purposes)(JVA got created in 1991 and JavaScript in 1995)?

JavaScript uses UTF-16 for encoding its strings, but the reason for this choice is not directly because it wanted to copy Java. Instead, it is more about the historical context and design decisions made during the development of JavaScript.

Key Points:

1. Historical Context: JavaScript was created in the mid-1990s, a time when UTF-16 was becoming a common encoding format for representing Unicode characters. The decision to use UTF-16 was influenced by existing technologies and standards at that time.

2. Compatibility with Browsers: Since JavaScript was designed to run in web browsers, using UTF-16 allowed for better compatibility with various text rendering systems and platforms that were already adopting Unicode.

3. Java Influence: While Java did use UTF-16 for its String class, it's important to note that JavaScript's design was influenced by many factors beyond just Java. The language aimed to be simple and lightweight for web development.

4. String Representation: In JavaScript, strings are sequences of 16-bit code units (UTF-16), which means that most common characters (like those in the Basic Multilingual Plane) can be represented with a single 16-bit unit, while less common characters may require two units (known as surrogate pairs).

5. Modern Developments: While JavaScript uses UTF-16 internally, it also supports other encodings through APIs like TextEncoder and TextDecoder, allowing developers to work with different character encodings as needed.

In summary, while there is some influence from Java in terms of string handling, the choice of UTF-16 in JavaScript is more about historical context and practical considerations rather than a direct attempt to copy Java's design choices.

#### Why js doesn't change its encoding system for encoding strings from      UTF-16 to UTF-8?

JavaScript uses UTF-16 as its internal string representation primarily for historical and compatibility reasons. Here are some key points to understand why JavaScript has not changed its encoding system from UTF-16 to UTF-8:

1. Historical Context: JavaScript was created in the mid-1990s, a time when UTF-16 was becoming a popular choice for representing Unicode text in many programming environments. The decision to use UTF-16 allowed JavaScript to handle a wide range of characters from different languages effectively.

2. Compatibility: Changing the internal string representation from UTF-16 to UTF-8 would break compatibility with existing code and libraries that rely on the current string handling mechanisms. This would create significant challenges for developers who have built applications over the years.

3. Performance Considerations: While UTF-8 is more space-efficient for ASCII characters (which are common in many applications), UTF-16 can be more efficient for certain languages and scripts that use a lot of non-Latin characters, as they may require fewer bytes per character in UTF-16.

4. Web Standards: JavaScript is deeply integrated into web standards, which also use various encodings (like UTF-8) for data interchange (e.g., HTML, JSON). However, the internal representation of strings in JavaScript remains consistent across different environments and platforms.

5. Interoperability with Other Systems: Many systems and APIs expect strings to be in a specific format. By using UTF-16 internally, JavaScript can easily interoperate with other systems that also use this encoding.

6. String Manipulation: The design of string manipulation functions in JavaScript is based on the assumption of 16-bit code units (the basis of UTF-16). Changing this would require rewriting many core functions and could introduce new complexities.

7. UTF-8 Support: While JavaScript uses UTF-16 internally, it does support conversion between encodings when necessary (e.g., when dealing with network requests or file I/O). Developers can encode and decode strings as needed using various APIs available in modern browsers.

In summary, while there are advantages to using UTF-8, especially regarding storage efficiency for ASCII-heavy text, the decision to stick with UTF-16 is rooted in historical context, compatibility concerns, performance considerations for certain languages, and established web standards.



### 12. RAM
RAM, or Random Access Memory, is a type of volatile memory used in computers and other devices to temporarily store data that the CPU (Central Processing Unit) needs to access quickly. Here are some key functions and characteristics of RAM:

8. Temporary Storage: RAM holds data and instructions that the CPU is currently using or processing. This allows for quick read and write access, which is essential for efficient computing.

9. Volatility: RAM is volatile memory, meaning it loses all stored information when the power is turned off. This contrasts with non-volatile storage like hard drives or SSDs, which retain data even when powered down.

10. Speed: RAM is much faster than traditional storage options (like HDDs or SSDs). This speed enables quick access to data, which helps improve overall system performance.

11. Multitasking: More RAM allows a computer to run multiple applications simultaneously without slowing down. When you open programs, they are loaded into RAM so that the CPU can access them quickly.

12. Data Buffering: RAM can act as a buffer for data being transferred between the CPU and other components (like graphics cards or storage devices), helping to smooth out performance during intensive tasks.

13. Types of RAM: There are different types of RAM, including DRAM (Dynamic RAM) and SRAM (Static RAM), each with its own characteristics and uses in computing.

In summary, RAM plays a crucial role in a computer's performance by providing fast, temporary storage for active processes and data that the CPU needs to access quickly.

#### what is the difference of RAM with HDD and SSD in term of storing?

RAM (Random Access Memory), HDD (Hard Disk Drive), and SSD (Solid State Drive) are all types of storage used in computers, but they serve different purposes and have distinct characteristics:

14. Type of Storage:
   - RAM: 
     - Volatile memory, meaning it loses its data when the power is turned off.
     - Used for temporary storage of data that the CPU needs to access quickly while performing tasks.
   - HDD:
     - Non-volatile storage, retains data even when powered off.
     - Uses spinning disks to read/write data magnetically; generally slower than SSDs.
   - SSD:
     - Also non-volatile storage, retains data without power.
     - Uses flash memory to store data electronically; significantly faster than HDDs.

15. Speed:
   - RAM: 
     - Extremely fast access times (nanoseconds), allowing quick read/write operations for active processes.
   - HDD: 
     - Slower access times (milliseconds) due to mechanical parts; performance can degrade over time as the drive fills up or if it becomes fragmented.
   - SSD: 
     - Much faster than HDDs (microseconds), leading to quicker boot times, file transfers, and application loading.

16. Capacity:
   - RAM: 
     - Typically available in smaller capacities compared to HDDs and SSDs (commonly ranging from 4GB to 64GB or more in consumer devices).
   - HDD: 
     - Generally offers larger capacities at a lower cost per gigabyte (ranging from hundreds of gigabytes to several terabytes).
   - SSD: 
     - Available in various capacities but tends to be more expensive per gigabyte compared to HDDs; common sizes range from 128GB to several terabytes.

17. Use Cases:
   - RAM: 
     - Essential for running applications and processes; the more RAM a system has, the better it can handle multitasking and demanding applications.
   - HDD: 
     - Suitable for bulk storage of files, documents, media libraries, and backups where speed is less critical.
   - SSD: 
     - Ideal for operating systems, applications requiring fast load times, gaming, and any scenario where speed is a priority.

Summary:
In summary, RAM is used for temporary storage that allows quick access by the CPU during active tasks but loses its contents when powered off. In contrast, both HDDs and SSDs provide long-term storage solutions that retain data without power; however, SSDs offer significantly faster performance compared to HDDs. The choice between these types of storage depends on specific needs regarding speed, capacity, and cost.

#### What is swapping in computer?
Swapping in computer science refers to a memory management technique used by operating systems to manage the allocation of memory resources. It involves moving data between the main memory (RAM) and a secondary storage device (such as a hard drive or SSD) to free up RAM for other processes. Here’s how it works:

1. Memory Management: When a computer runs multiple applications, it may not have enough RAM to accommodate all of them simultaneously. Swapping allows the operating system to temporarily move inactive or less frequently used data from RAM to disk storage.

2. Swap Space: The area on the disk designated for this purpose is called swap space or swap file. When the system needs more RAM, it can "swap out" some data from RAM to this space.

3. Swapping Process:
   - Swapping Out: When an application is not actively being used, its data can be moved from RAM to swap space.
   - Swapping In: If that application needs to be accessed again, the operating system will move its data back into RAM, potentially swapping out another application if necessary.

4. Performance Considerations: While swapping allows for more efficient use of limited memory resources, it can lead to performance degradation if excessive swapping occurs (a situation known as thrashing). This happens when the system spends more time swapping data in and out of memory than executing processes.

5. Use Cases: Swapping is particularly useful in systems with limited physical memory or when running large applications that exceed available RAM.

Overall, swapping is a crucial mechanism that helps maintain system stability and performance by optimizing memory usage across multiple applications and processes.

#### Relation between a file size and encoding system
when for example, we store a JavaScript file in our own pc and we have selected its encoding system as UTF-16 in our VS code, it take twice more space than it is encoded with UTF-8 because the JavaScript syntax language is in English and English letters are part of the alphabets, so our JavaScript code in UTF-16 occupies 2 byte per character while it's 1 byte per character in UTF-8, that how a file gets larger in our computer.

when we run a JavaScript code, we either run in browser console or in node, in both of them the string encoded with UTF-16 which default encoding system for JavaScript string dat type and after the app executed and its execution, terminated the amount of space was allocated in RAM for our JavaScript code gets garbage collected. (I explained earlier how much other JavaScript data type occupy in the RAM).

so the effect of the VS code encoding system is permanent on our file size but the effect of JavaScript default encoding system for strings (UTF-16) and other space allocation is temporary and those space allocates only during execution and then garbage collect when the code execution terminates. 

#### Why local storage saves everything in utf-16 encoding system?
Local Storage in web browsers does not specifically save data in UTF-16 encoding; rather, it stores data as strings, which are typically encoded in UTF-16 by the JavaScript engine. Here’s a breakdown of how this works:

1. JavaScript Strings: In JavaScript, strings are represented as sequences of UTF-16 code units. This means that when you store a string in Local Storage, it is inherently treated as UTF-16.

2. Storage Mechanism: When you use Local Storage (via `localStorage.setItem()`), the JavaScript engine converts the string into a format suitable for storage. While the internal representation may be UTF-16, browsers handle the conversion to and from this format transparently.

3. Cross-Browser Compatibility: Different browsers may have different implementations, but they all adhere to the Web Storage API specifications, which dictate that data should be stored as strings.

4. Data Retrieval: When you retrieve data from Local Storage (using `localStorage.getItem()`), it is returned as a string in JavaScript's native format (UTF-16).

5. Limitations and Considerations: While Local Storage can handle most characters due to its support for Unicode through UTF-16, it's important to note that certain characters or large amounts of data may require special handling or encoding (like Base64) if you're storing binary data or complex objects.

In summary, while Local Storage itself doesn't explicitly save everything in UTF-16 encoding, it uses JavaScript's string representation (which is based on UTF-16) for storing and retrieving text data.

#### When I save a file in vs code with Hebrew text with ISO 8859-8 encoding system, and open it with notepad it displays replacement character and misinterpretation, then when I copy those broken and replacement characters in that file in vs code which its encoding system is still              ISO 8859-8, why I still see the same broken and replacement character which I saw in notepad after pasting them?

the things happen in here is, we know that notepad can't detect ISO 8859-8, so it uses UTF-16 or UTF-8 to interpret the text, hence it ends in misinterpretation and replacement characters, after that when we want to copy the characters from notepad, the characters bytes don't get copied but the Unicode i.e. the characters are interpreted in UTF-16 and they have a byte when copying those characters, the windows copying mechanism decodes those bytes and copy the Unicode code point, we know that code points are still and same in all Unicode encoding systems (Unicode code points are same in all of the encoding systems and the allocated byte is different for each code point, so by having the code point you can have the same character in all of the encoding systems but having byte of a character gives wrong character in each encoding system), therefore when we copy those Unicode code points in our file in vs code despite of encoding system in vs code, same characters get displayed to us.   

#### I just visiting a site and someone had commented a text in that site but there was replacement characters among its comment, i was wondering what's the reason for those replacement characters in that site, isn't the HTML in UTF-8, so some part of that text is misinterpreted?

 The presence of replacement characters, such as &#x27;, in a comment on a website typically indicates that the text has been encoded in HTML entities. In this case, &#x27;(replacement character) is the HTML entity for the apostrophe or single quote ('). 

 The text may have been encoded to ensure that special characters are displayed correctly in HTML. For example, using &#x27; instead of an apostrophe helps prevent issues with HTML parsing.

- so why we see replacement character instead of single quote in some sites?
  Some web applications may not properly handle special characters like single quotes, especially if they are not escaped correctly in HTML or JavaScript contexts.

- how to fix problem of displaying replacement character instead of single quote in website due to improper special character encoding handling by HTML or JavaScript? 

If you're dynamically inserting text into your HTML using JavaScript, ensure that you're properly escaping any special characters. For example:
```javascript

let text = "Here’s a single quote.";
document.getElementById("output").innerText = text; // Use innerText or textContent for safe insertion
```

If you're using innerHTML, make sure to escape any special characters:
```JavaScript
let text = "Here’s a single quote.";
document.getElementById("output").innerHTML = text.replace(/'/g, '&#39;'); // Escape single quotes if necessary
```

I haven't checked the does this solution really resolve the issue or not since I haven't faced this issue on my own, so consider this solution as a section which I put it here to use it as a stand by solution.   

for checking this rare but interesting incident you can look up word `transaction` in `abadis dictionary` site and in the user recommendation, there is a comment by `Mostafa Rashidi` which occurrence of this incident is visible.

here's the [link](https://abadis.ir/entofa/transaction/)

### 13. if I have a  `<p>true</p>` as my react code, what's the type of that text between `p` tag which is `true`, is it a `boolean` or `string`?

the text between the `<p>` tags is treated as a string. 
When you write HTML (or JSX in React), any text content inside an element is considered a string, regardless of whether it looks like a boolean value or a number (same rule applies in HTML) (like "true" or "false"). So in this case, the text "true" is a string, not a boolean.

### 14. Why some filtering by passing call their app DNS, while DNS  duty is to convert domain into IP?

The term "DNS" (Domain Name System) primarily refers to the system that translates human-readable domain names (like www.example.com) into IP addresses that computers use to identify each other on the network. However, in the context of applications and services, especially those related to filtering or security, "DNS" can refer to a broader set of functionalities beyond just name resolution.

Here are a few reasons why some filtering applications might refer to their service as "DNS":

1. DNS-Based Filtering: Many filtering solutions use DNS queries to determine whether a request should be allowed or blocked. By intercepting DNS requests, these services can filter out access to malicious or unwanted domains before any connection is established.

2. Content Control: Some applications provide content control features by using DNS queries to block access to specific categories of websites (e.g., adult content, gambling sites). This is often done at the DNS level, where requests for certain domains are resolved to a non-routable IP address or blocked entirely.

3. Security Features: Security-focused DNS services can protect users from phishing attacks and malware by preventing access to known malicious domains. This is often marketed as "secure DNS" or "DNS filtering."

4. Privacy Enhancements: Some apps offer privacy-focused DNS services that prevent tracking by using encrypted DNS protocols (like DoH - DNS over HTTPS). These services may be branded as "DNS" because they enhance user privacy while still performing the fundamental role of resolving domain names.

5. User-Friendly Terminology: Referring to an application as a "DNS app" can make it more relatable and understandable for users who may not be familiar with technical networking concepts but understand that it relates to internet navigation and security.

In summary, while the primary function of DNS is indeed name resolution, many modern applications leverage this functionality for additional purposes such as filtering, security, and privacy enhancements. Thus, they may refer to themselves as "DNS apps" even though their roles extend beyond simple domain-to-IP translation.

the 4th reason seem to be most reasonable answer to this question.

#### what is 1.1.1.1?
1.1.1.1 is a public DNS resolver service provided by Cloudflare in partnership with APNIC. It was launched to offer a fast and secure alternative to traditional DNS services (by DNS in this point we mean its filtering bypassing application we mentioned earlier in previous point 4th section). Here are some key points about 1.1.1.1:

- Speed: Cloudflare claims that 1.1.1.1 is one of the fastest DNS resolvers available, which can lead to quicker website loading times.
- Privacy: The service emphasizes user privacy, stating that it does not log your IP address or sell your data.
- Security: It supports DNS over HTTPS (DoH) and DNS over TLS (DoT), which encrypts DNS queries to enhance security and privacy.
- Usage: Users can configure their devices or routers to use 1.1.1.1 as their primary DNS server for improved performance and security.

To use it, you can set your device's DNS settings to 1.1.1.1 (primary) and 1.0.0.1 (secondary).

application like `1.1.1.1`, use DNS service of an server which use 1.1.1.1 as their DNS resolver service (basically this 1.1.1.1 is part of the DNS configuration which is technical and I can't understand) 

### 15. what is subnet masking?
Subnet masking is a technique used in computer networking to divide an IP address into two parts: the network portion and the host portion. This allows for the efficient allocation of IP addresses and helps in organizing and managing networks.

A subnet mask is a 32-bit number that accompanies an IP address and specifies which part of the IP address refers to the network and which part refers to the individual device (host) on that network. The subnet mask consists of a series of contiguous ones (1s) followed by a series of contiguous zeros (0s). The ones indicate the network portion, while the zeros indicate the host portion.

For example, in the IP address 192.168.1.10 with a subnet mask of 255.255.255.0 (or /24 in CIDR notation), the first three octets (192.168.1) represent the network, and the last octet (10) represents the specific host within that network. This means that all devices with IP addresses from 192.168.1.1 to 192.168.1.254 are part of the same subnet. (subnet mask number is 255, it means our network with this subnet mask can have 254 hosts (members) (subnet mask number -1))

Subnetting helps improve network performance and security by reducing broadcast domains and allowing for better management of IP address allocation.

### 16. Session, state, authentication and client-side storages
In programming, a "session" typically refers to a temporary and interactive information exchange between a user and a web application or service. Sessions are commonly used in web development to maintain state and track user interactions over multiple requests.

in simple words and in action, the term session in web development mentions to a ***duration*** which a user logs in a site and is able to access a site without logging in it again.

different things can impact on lifecycle of a session, closing the browser, tab and etc. we will discuss about them in here.

when we log-in a site usually they ask us to save the info and remember us, in this case we won't need to log-in for subsequent visits of that specific site, this is where we have to introduce a new term: **Authentication**.

Authentication in programming refers to the process of verifying the identity of a user, device, or system before granting access to resources or services. It is a critical component of security in software applications and systems, ensuring that only authorized individuals can access sensitive data or perform certain actions.

#### Methods of Authentication

***JWT***
 one of the most popular methods of authentication is token-based authentication.
 Users receive a token after logging in successfully, which they can use for subsequent requests without needing to re-enter their credentials.
 another method is session cookies which simply is a session id (a number refers to a specific session) usually stores in cookie storage.

when we log in a site, a token (in JWT term) or a session id (in terms of session cookie) gets generated for us and stores in storages (usually cookie but can be stored in local storage, session storage, index db and cookies storage). the simple illustration of this process is, when we use JWT as our authentication method, first time we log in in a site, a token gets generated in server containing our information which facilitate our subsequent visits and log-in process (the JWT doesn't contain our username or password, it stores our info in its own way which is a user id and other stuff (for more information, read the pink notebook)), this token gets encoded and set a expiration time by the server but it won't be stored in server, then it get sent to client side and stores in cookies storage (the reason it stores in cookies storage rather than other storage like local storage or session storage is, cookies get sent automatically to the server with each request, so next time user sends a request to the server, they don't need to use JWT manually in their HTTP request header and the JWT will be sent automatically to the server, meanwhile the JWT can be stored as other type of data like local storage or session storage data but due to automatic send and security reasons, cookie is preferred), we call JWT as stateless authentication because the information of the log in and authentication doesn't store in server (you may say how it is stateless while it is getting stored on client-side storage like cookies, when we mention ***stateless*** (you can check [[JavaScript + misc programming concepts#What's state?|here]] the definition of state) in our notes, we mean server-side stateless, it means if no info or state gets stored on the server side, we can call it stateless even if the action is stateful in    client-side like what we have here for JWT (the JWT (the state) stores in cookie which makes our client side stateful)), by JWT being stored in cookies, for subsequent requests, automatically this JWT will be send to the server and we can use the website without log in (you may how the server detect the JWT which I've explained it in pink notebook).

***Session ID***
we have another authentication method which is session id (for more info about what session id is, you can refer to pink notebook), when user logs in a site a session id gets generated at server and stores in server (it stores in a database like SQL based database) and get sent to the client side and stores usually in cookies, the cookie that get sent as session id usually doesn't have a `MAX-AGE` attribute and this cookie is not persistent, before I go further I have to explain different type of cookies:

***1. Persistent cookies***
persistent cookies are type of cookies which they have `MAX-AGE` or expiration date.

***2. Session cookies***
session cookies are type of cookies which they don't have `MAX-AGE` or expiration date.

now we know different type of cookies, I have to tell you that session id gets stored as session cookies since their cookie doesn't have `MAX-AGE` or expiration date.
we tell later that why session id get stored as session cookies.

since session id stores in server, we call this type of authentication stateful, also I forget to mention we also call JWT, bearer token because the token carries information about authentication within itself every time we send a request. 

- one prominent difference between JWT and session id is that JWT has its own expiration time but session id doesn't.

#### difference in application of JWT and session ID
JWT is designed to keep the user logged-in in multiple visits like you log in a website today then close the browser, next time you look up the same website in your browser due to presence of JWT, you are able to visit that website, so JWT is designed to keep you logged-in even when you close the browser or browser tab/window. (when we say that JWT is designed to persist in browser closure or browser tab/window closure, it's a general purpose and it doesn't mean it has to work always, there are scenarios that the JWT may not persist in browser closure or browser tab/window closure) like a shopping website like E-bay, you don't want to log in every time you visit the website and since there is no sensitive information on website, it doesn't matter you remain logged in. 

unlike JWT, session id is designed to log you out from a site the moment you close the tab/window in a browser or you close the browser. (like JWT, logging out from the site for closing the browser or browser tab/window closure is a general purpose but they are scenarios that session id persists against closing the browser or browser tab/window closure), so then you may ask if this kind of authentication is supposed to be invalidated and deleted from the server after closure of browser or its tab/window, so why they get stored in server from the first place, what kind of authentication they're applying and facilitate what kind of logging process? I have to tell when you log in a website for instance a website like Amazon, when you switch between different pages in that website, like you check the home page with some products in it then you go to your shopping cart page and then your profile info, these switching between different paths or pages of a website requires log-in and authentication, with session cookies you don't need to authenticate and when ever you switch page in the same website, a request get sent to server to retrieve the page info, alongside that the session id will be sent automatically (because session id usually is in cookies and get sent with each request automatically) and we get authenticated, that why these session cookies get stored on the server, JWT has the same process and does the same thing for authenticating between pages of a similar website, the only difference is JWT is for sites we don't want to log us out when we close browser or its tab/window but session id method is for when we want to user be logged out after browser or its tab/window closure like a banking website which has critical and sensitive information which we don't want them to be accessed by any stranger so we prefer to be logged out after browser or its tab/window closure. 

#### I have a website which I want the user to log-out after 17 minutes of inactivity, I think for this I have to use session id authentication method and set 17 minutes in my server side code for invalidation, is my deduction and statement correct?

Yes, your deduction is correct. To implement a logout mechanism after 17 minutes of inactivity, you can use session management on the server side. Here’s a general outline of how you can achieve this:

1. Session Management: When a user logs in, create a session for them on the server. This typically involves generating a unique session ID and storing it along with user information.

2. Set Session Timeout: Configure your server-side session settings to expire sessions after 17 minutes of inactivity. This means that if there are no requests from the user for 17 minutes, the session will be invalidated.

3. Inactivity Tracking: You can track user activity by updating the session's last activity timestamp on each request (e.g., when they click links or submit forms). If the current time exceeds the last activity time plus 17 minutes, you can consider the user logged out.

4. Client-Side Handling: Optionally, you can implement client-side JavaScript to provide feedback to users before they are logged out (e.g., showing a warning message a few minutes before timeout) and allow them to extend their session if they are still active.

5. Logout Logic: When checking for an active session on each request, if the session has expired (i.e., more than 17 minutes since last activity), redirect the user to the login page or show an appropriate message.

session cookies may not have a expiration time on their own (but you can set txpriation time like JWT in server) but you can set inactivity time to them as we've explained in example above (we can set inactivity time to JWT also but it takes more effort and it's more difficult i.e. we can implement example or question above with JWT but with session cookies it's easier).

so session id authentication get used for websites which needs to limit their user usage of that website to a specific duration or for sites which don't want to keep their user logged in after user closing browser or its tab/window (in both cases we want to stay logged in when navigating through different pages of a website)


***UPDATE:*** this method can be pulled off with JWT also and session id is not the only option

#### Inactivity time VS Expiration time
1. Time of Inactivity:
   - This refers to how long a user has been inactive (not interacting with the website) before their session is considered expired or invalidated.
   - Some web applications implement session management strategies where they will invalidate or delete session cookies after a certain period of inactivity (e.g., 15 minutes). This is often done for security reasons to prevent unauthorized access if someone leaves their computer unattended.

Key Differences
- Duration: Expiration time is fixed and predetermined when the cookie is created, while inactivity-based expiration depends on user behavior (like clicking a button or posting a form can reset the inactivity time)

in example above if I wanted user to be logged out exactly after 17 minutes (17 minutes of absolute time not inactivity time) like a transfer money page on a banking website which has a time limit, we could implement that with JWT and set its expiration time to 17 minutes, even example above is feasible with session id but we prefer to employ the easier approach which is session id.

- we can even enable to invalidate a specific authentication method like JWT after user web closure or its tab/windows (even though it's not that efficient or optimal but still works) but due to better efficiency of session id's in this field we use, session id's.

**Note**: ***session cookie is not an authentication method*** , session id is authentication method and because session id stores as a session cookie (a cookie without expiration date set for the cookie) in cookies stores, you may mistaken session id and session cookie.

JWT usually stores as a persistent cookie because it requires to be sent automatically with each request (cookie does that) and persistency against browser or its tab/windows closure which it can be achieved with persistent cookies because they have expiration time of their own cookie (if we store a JWT as a session cookie, it doesn't matter if our JWT has a expiration date, if we close the browser or its tab/window, that JWT will be deleted from cookies storage and we need to log in for our subsequent visits)

you can read more about JWT and session id in pink notebook.
#### What's state?
In programming, the term "state" refers to the current condition or status of a system, application, or object at a specific point in time. It encompasses all the data and variables that define how the system behaves and what it can do at that moment. Here are some key aspects of state in programming:

1. Variables and Data: The state is often represented by variables that hold data. For example, in a game, the state might include the player's score, position, health, and inventory.

2. Object State: In object-oriented programming (OOP), an object's state is defined by its attributes (or properties). For instance, a Car object might have attributes like speed, fuelLevel, and engineStatus.

3. Application State: In web applications, the application state can refer to user sessions, data fetched from databases, or any information that persists across different parts of the application.

4. State Management: Managing state is crucial in programming because it affects how applications respond to user inputs and external events. Various patterns and libraries (like Redux for React applications) help manage complex states effectively.

5. Immutable vs Mutable State: Some programming paradigms emphasize immutability (where state cannot be changed after it's created) to avoid side effects and make reasoning about code easier. Others allow mutable states where values can change over time.

6. State Machines: In certain contexts (like game development or UI design), systems may be modeled as state machines where they transition between different states based on events or conditions.

7. Concurrency and State: In concurrent programming, managing shared state between threads or processes becomes critical to avoid issues like race conditions.

Understanding how to manage and manipulate state is fundamental for building robust software systems across various domains of programming.

in the passage above the first and third points are the best definition, in a nutshell state is a data which is defining an action or a behavior.
#### when we say HTTP is stateless, what data it can store on server but doesn't due to statelessness?
When we say that HTTP is stateless, it means that each request from a client to a server is treated as an independent transaction. The server does not retain any information about previous requests made by the client. This statelessness has implications for what data could be stored but isn't due to the nature of the protocol.

Here are some types of data that could theoretically be stored on the server but aren't due to HTTP's statelessness:

1. User Session Information: In a stateful protocol, the server could remember user sessions, including login status, preferences, and other personalized settings. Instead, HTTP requires mechanisms like cookies or session tokens to manage this information across multiple requests.

2. Request History: The server could keep track of all previous requests made by a client (e.g., pages visited, actions taken). However, in HTTP's stateless model, each request is independent and does not carry context from previous interactions.

3. Temporary Data: Data related to ongoing transactions or processes (like items in a shopping cart) would need to be managed externally (e.g. through sessions or databases) because the server does not remember past interactions.

4. User Preferences: Any preferences set by users during their interaction with an application (like language settings or theme choices) would need to be sent with each request rather than being remembered by the server (user preferences and shopping cart item and info can be sent to server and stored in database via cookies but due to their size and can latency that can occur, it's prohibited)

5. Authentication State: While authentication can occur over HTTP (e.g. via session id), the server does not inherently remember whether a user is authenticated between requests unless additional mechanisms are implemented like cookies.

6. Application State: Any state related to an application’s workflow (like progress in a multi-step form) would need to be explicitly managed since HTTP does not maintain any context between requests.

To manage these types of data in a stateless environment, developers often use techniques such as:

- Cookies: Small pieces of data stored on the client side that can hold session identifiers or user preferences.
- Session Management: Using session IDs passed back and forth between client and server to maintain state.
- Databases: Storing user-related data persistently so it can be retrieved as needed for each new request.
- URL Parameters or Query Strings: Sending necessary state information directly within URLs for specific actions.

In summary, while HTTP itself doesn't store any stateful information between requests due to its stateless nature, developers implement various strategies to simulate statefulness when needed for web applications.

#### We know session cookies are stateful, so if session cookies are stateful, doesn't statefulness of session cookies violates statelessness of HTTP?
The relationship between session cookies and the statelessness of HTTP can be a bit nuanced. Here’s a breakdown to clarify:

1. Statelessness of HTTP: HTTP is designed to be a stateless protocol, meaning that each request from a client to a server is treated as an independent transaction. The server does not retain any information about previous requests from the same client.

2. Session Cookies: Session cookies are used to maintain state across multiple requests in web applications. They allow the server to remember information about the user (like login status or items in a shopping cart) across different requests.

3. How They Work Together:
   - When a user first interacts with a web application, the server may create a session and send back a session cookie to the client.
   - This cookie is stored on the client side and sent back with subsequent requests.
   - The server can then read this cookie and retrieve any associated session data, effectively allowing it to "remember" information about that user.

4. No Violation of Statelessness: While session cookies introduce stateful behavior at the application level, they do not violate the fundamental stateless nature of HTTP itself:
   - Each individual HTTP request remains stateless; it does not inherently carry knowledge of previous requests.
   - The statefulness comes from how applications use cookies to manage sessions, but this is an implementation detail rather than a change in how HTTP operates.

In summary, while session cookies enable stateful interactions in web applications, they do so without violating the underlying stateless nature of the HTTP protocol itself. The separation between protocol (HTTP) and application logic (session management) allows both concepts to coexist effectively.
basically it says that session cookies statefulness are not related to HTTP statelessness because HTTP is bottom layer of cookies and cookies are like an extension which their behavior is different 
to fullfill new desires but since the bottom layer is HTTP, so everything remains stateless.

#### What are distributed systems?
Distributed systems in programming refer to a model where multiple independent components or nodes work together to achieve a common goal, often over a network. These systems are designed to share resources, data, and processing power across different machines or locations, allowing for improved performance, scalability, fault tolerance, and resource utilization.

Key Characteristics of Distributed Systems:

1. Multiple Components: A distributed system consists of multiple autonomous entities (nodes) that communicate and coordinate with each other.

2. Network Communication: Nodes in a distributed system communicate over a network using various protocols (e.g., HTTP, TCP/IP).

3. Concurrency: Multiple processes can run simultaneously on different nodes, allowing for parallel processing and improved efficiency.

4. Scalability: Distributed systems can be scaled horizontally by adding more nodes to handle increased load or data.

5. Fault Tolerance: They are designed to continue functioning even when some components fail. This is often achieved through redundancy and replication.

6. Transparency: Ideally, the complexity of the distributed nature should be hidden from users and applications, making it appear as a single coherent system.

7. Resource Sharing: Resources such as storage and processing power can be shared among nodes in the system.

Types of Distributed Systems:

1. Client-Server Systems: A common architecture where clients request services from centralized servers.
  
2. Peer-to-Peer Systems (P2P): All nodes have equal roles and can act as both clients and servers (e.g., file-sharing networks).

3. Cloud Computing Platforms: Services provided over the internet that allow users to access computing resources on demand (e.g., AWS, Google Cloud).

4. Microservices Architecture: An approach where applications are built as a collection of loosely coupled services that communicate over APIs.

5. Distributed Databases: Databases that store data across multiple locations while providing mechanisms for consistency and availability.

Challenges in Distributed Systems:

1. Network Latency: Communication delays between nodes can affect performance.
  
2. Data Consistency: Ensuring all nodes have the same view of data can be complex due to network partitions or failures (CAP theorem).

3. Security: Protecting data during transmission and ensuring secure access across distributed components is critical.

4. Debugging and Monitoring: Identifying issues in a distributed environment can be more challenging than in centralized systems due to their complexity.

5. Synchronization: Coordinating actions among distributed components requires careful design to avoid conflicts or race conditions.

Examples of Distributed Systems:

- The Internet itself
- Content delivery networks (CDNs)
- Online multiplayer games
- Blockchain networks
- Distributed file systems like Hadoop HDFS

In summary, distributed systems play a crucial role in modern computing by enabling applications that require high availability, scalability, and resilience against failures while leveraging resources across multiple machines or locations.

#### between session ID and JWT, which approach is more popular and common for authentication?
Both session IDs and JSON Web Tokens (JWT) are popular methods for handling authentication, but their usage can vary based on the specific requirements of an application. Here's a comparison of the two:

**Session ID**
How it Works:
- When a user logs in, the server creates a session and stores it in memory or a database.
- A unique session ID is generated and sent to the client, typically stored in a cookie.
- On subsequent requests, the client sends this session ID back to the server for validation.

Pros:
- Simplicity: Easy to implement and understand.
- Server-side control: The server can easily invalidate sessions by removing them from storage.
- Security: Session data is stored on the server, reducing exposure of sensitive information.

Cons:
- Scalability: Requires server-side storage, which can be challenging in [[JavaScript + misc programming concepts#What are distributed systems?|distributed systems]] unless using shared storage solutions.
- Cookie management: Requires careful handling of cookies (e.g., secure flags, SameSite attributes).

**JSON Web Token (JWT)**
How it Works:
- Upon successful login, the server generates a JWT containing user information and signs it with a secret key.
- The token is sent to the client and typically stored in local storage or cookies.
- The client includes this token in subsequent requests for authentication.

Pros:
- Stateless: No need for server-side session storage; all necessary information is contained within the token itself.
- Scalability: Easier to scale across multiple servers (distributed systems) since no shared state is required.
- Flexibility: Can include additional claims (metadata) about users.

Cons:
- Token invalidation can be complex; once issued, tokens remain valid until they expire unless you implement additional mechanisms (like blacklisting).
- Larger payloads compared to simple session IDs due to encoding user data within the token.

**Popularity**
The choice between session IDs and JWT often depends on specific use cases:

1. Web Applications: Traditional web applications often use session IDs due to their simplicity and ease of management. However, many modern web applications that require statelessness or need to work with APIs may prefer JWTs.

2. APIs/Microservices: JWTs are increasingly popular for APIs and microservices architectures because they allow for stateless authentication across distributed systems without needing centralized session management and not requiring to maintain state on the server.

3. Mobile Applications: JWTs are commonly used in mobile applications due to their ability to easily handle authentication without maintaining state on the server.

**Conclusion**
In summary:
- Session IDs are still widely used for traditional web applications where simplicity and security are paramount.
- JWTs have gained popularity in modern architectures that require scalability and statelessness, especially in API-driven environments.

we concluded that JWT is much more popular in modern web, earlier I told that these two authentication methods (session id & JWT) have different applications but actually I had made a mistake and these two can be used interchangeably and whatever can one do, the other one can do also (maybe some tasks are easier in particular method but at the end of the day they can pull off the same tasks), the reason we recommend JWT is because of statelessness nature and the advantages this feature has which we have explained above, furthermore JWT is more recent than session id, so it has fixed the issues we could've had with session IDs. (session id:1990s, JWT:2015 for their invention year)

#### what are the challenges of using session id for distributed systems and what are benefits of using JWT in distributed systems?
Using session IDs in distributed systems and opting for JSON Web Tokens (JWT) both come with their own sets of challenges and benefits. Here’s a breakdown of the challenges associated with session IDs and the advantages of using JWTs in distributed environments:

**Challenges of Using Session IDs in Distributed Systems**

1. State Management:
   - Centralized Storage: Session IDs often require a centralized session store (like a database or in-memory store) to manage user sessions, which can become a bottleneck and single point of failure.
   - Scalability: As the number of users increases, managing sessions centrally can lead to performance issues and complicate scaling efforts.

2. Session Persistence:
   - Data Loss: If the session store crashes or is not properly replicated, active sessions may be lost, leading to poor user experience.
   - Sticky Sessions: Load balancers may need to implement sticky sessions (routing requests from the same user to the same server), which can limit scalability.

3. Cross-Domain Issues:
   - Managing sessions across different domains or microservices can be complex, as each service may have its own session management strategy.

4. Security Concerns:
   - Session hijacking is a risk if session IDs are not securely transmitted or stored.
   - Expiring sessions can lead to user frustration if not handled gracefully.

5. Complexity in Logout Mechanism:
   - Invalidating sessions across multiple services requires additional coordination and complexity.

**Benefits of Using JWT in Distributed Systems**

1. Statelessness:
   - JWTs are self-contained tokens that carry all necessary information about the user within themselves, allowing for stateless authentication. This reduces reliance on centralized storage.

2. Scalability:
   - Since JWTs do not require server-side storage, they scale more easily across distributed systems without becoming a bottleneck.

3. Decentralized Verification:
   - Any service that has access to the public key (in case of asymmetric signing) can verify the token without needing to contact a central authority, facilitating microservices architecture.

4. Cross-Domain Compatibility:
   - JWTs can be easily used across different domains and services without requiring complex session management strategies.

5. Built-in Expiration and Claims:
   - JWTs support expiration times (exp claim) and other claims that provide context about the token's validity, enhancing security by limiting token lifespan.

6. Flexibility with Claims:
   - Custom claims can be added to JWTs for additional context about users or permissions, making them versatile for various use cases.

7. Reduced Latency:
   - Since no round-trip is needed to validate tokens against a central store, this can reduce latency in authentication processes.

8. Easier Logout Mechanism (with caveats):
   - While invalidating tokens requires some strategy (like maintaining a blacklist), it allows for more flexible logout mechanisms compared to traditional session management where you must invalidate on all servers.

**Conclusion**

In summary, while using session IDs poses challenges related to state management, scalability, security concerns, and complexity in distributed systems, adopting JWT offers significant benefits such as statelessness, scalability, decentralized verification, cross-domain compatibility, built-in expiration features, flexibility with claims, reduced latency in authentication processes, and potentially easier logout mechanisms—though careful consideration must still be given to token invalidation strategies when using JWTs.

#### what is SQLite?
SQLite is a lightweight, serverless, self-contained SQL database engine. It is designed to be embedded into applications, making it an ideal choice for mobile apps, desktop software, and small to medium-sized web applications. Here are some key features of SQLite:

1. Serverless: Unlike traditional database management systems that require a separate server process, SQLite operates directly on disk files. This means there is no need for a separate server installation or configuration.

2. Self-Contained: SQLite is a single library that can be included in applications without external dependencies. The entire database engine is contained in a small binary file.

3. Cross-Platform: SQLite works on various operating systems, including Windows, macOS, Linux, iOS, and Android.

4. ACID Compliance: SQLite supports Atomicity, Consistency, Isolation, and Durability (ACID) properties for transactions, ensuring reliable data management.

5. Lightweight: The library size is relatively small (typically less than 1 MB), making it suitable for resource-constrained environments.

6. SQL Support: SQLite supports most of the SQL standard features such as transactions, subqueries, triggers, views, and more.

7. File-Based Storage: Data is stored in a single file on disk which simplifies backup and transfer processes.

8. Public Domain: SQLite is open-source and released into the public domain; it can be used freely in both open-source and proprietary software projects.

Due to these characteristics, SQLite is widely used in various applications ranging from web browsers (like Firefox) to mobile apps (like those on iOS and Android) and even embedded systems.

#### Client-side storages
we have 2 types of storages in web development, server-side storage and client-side storage.
server-side storages is like the database we use for instance the SQL or No-SQL based like MY SQL and etc. and for client side storages we have:
1. Local storage
2. Session storage
3. Cookies storage
4. IndexedDB

(there may be other client-side storages but these are the most important one)

each storage has its own characteristic and features, and we use them to store specific type of data.

Most major modern websites are dynamic — they store data on the server using some kind of database (server-side storage), then run server-side code to retrieve needed data, insert it into static page templates, and serve the resulting HTML to the client to be displayed by the user's browser.

Client-side storage works on similar principles, but has different uses. It consists of JavaScript APIs that allow you to store data on the client (i.e. on the user's machine) and then retrieve it when needed. This has many distinct uses, such as:

- Personalizing site preferences (e.g. showing a user's choice of custom widgets, color scheme, or font size).
- Persisting previous site activity (e.g. storing the contents of a shopping cart from a previous session, remembering if a user was previously logged in).
- Saving data and assets locally so a site will be quicker (and potentially less expensive) to download, or be usable without a network connection.
- Saving web application generated documents locally for use offline

you can store points mentioned above in a server-side storage but it might not be a good option or even an option, for instance we can only store JWT in client-side storage due to its statelessness.
or storing a user shopping cart item in server-side can cause latency to their lare size.

##### Local storages
Local storage is a web storage feature that allows websites to store data in a user's browser. It provides a way to persistently store key-value pairs in a web application, enabling the application to save data across sessions without needing to communicate with a server. Here are some key points about local storage:

1. Capacity: Local storage typically allows for storing up to 5-10 MB of data per origin (domain), which is significantly more than cookies.

2. Data Persistence: Data stored in local storage remains even after the browser is closed and reopened, unlike session storage, which only lasts for the duration of the page session.
   local storage keeps its data if you close the browser, browser tab/window.

3. Synchronous API: Local storage operations are synchronous, meaning that reading and writing data can block the main thread, potentially affecting performance if large amounts of data are handled, we know that local storages are part of web storage API which web storage API is web API, I thought that all web APIs are asynchronous but it seems it's not true, the web APIs related to request mechanism like `fetch()` are asynchronous beside majority of web API, but there are some web APIs like local storage and session storage which are synchronous, so if we have synchronous web API, why the event loop diagram had considered web APIs asynchronous? because In practice, developers frequently use web APIs in an asynchronous manner (e.g., making HTTP requests), so representing them as such aligns with common usage patterns and expectations.
 
4. Key-Value Pairs: Data is stored as strings in key-value pairs. You can set, get, remove, and clear items using methods like `setItem()`, `getItem()`, `removeItem()`, and `clear()`.

5. Same-Origin Policy: Local storage is subject to the same-origin policy, meaning that data stored by one domain cannot be accessed by another domain.

6. Use Cases: Common use cases include saving user preferences, caching application state, or storing temporary data for offline access.

###### what kind of data stores in local storage?
User Preferences: Settings such as theme choices (light/dark mode), language preferences, or layout configurations.
1. Session Information: Data related to user sessions, like whether a user is logged in or not, and session tokens.

2. Form Data: Temporary storage of form inputs so that users can return to partially filled forms without losing their progress.

3. Shopping Cart Contents: E-commerce sites often use local storage to keep track of items added to a shopping cart between sessions.

4. Game State: For web-based games, local storage can save the current state of the game, including scores and levels achieved.

5. User-generated Content: Small pieces of content created by users, such as notes or comments that don’t require server-side storage.

6. Application State: Information about the current state of a web application, which can help restore the app's state when revisiting.

7. Analytics Data: Non-sensitive usage statistics or tracking information that helps developers understand how users interact with their site.

8. Cached Data: Small amounts of data that can help speed up loading times by caching certain resources locally.
##### Session storages
Session storage is a type of web storage that allows you to store data for the duration of a page session. A page session lasts as long as the browser is open, and it persists across page reloads and restores. However, it is cleared when the tab or browser is closed.

**Key Features of Session Storage:**
1. Scope: Data stored in session storage is specific to a single tab or window. If you open a new tab or window, it will not have access to the session storage of another tab.

2. Lifetime: The data persists only for the duration of the page session. Once the user closes the tab or browser, all data stored in session storage is deleted.

3. Storage Limit: Most browsers allow you to store around 5-10 MB of data in session storage, though this can vary by browser.

4. Data Type: Session storage stores data as key-value pairs, where both keys and values are strings. You can use `JSON.stringify()` to store objects and `JSON.parse()` to retrieve them.

5. session storages are synchronous like local storage which means if we want to use session storage methods it'll be processed synchronously.
 
**Use Cases:**
- Temporary Data Storage: Useful for storing temporary data that should not persist beyond a single browsing session (e.g., form inputs).

**Limitations:**
- Not suitable for storing sensitive information since it's accessible via JavaScript and can be exposed through XSS attacks if proper security measures are not taken.
- Limited lifespan means it's not ideal for long-term data persistence; local storage or server-side databases would be better suited for that purpose.

Overall, session storage provides a convenient way to manage temporary data within web applications while ensuring that it does not persist beyond the user's current browsing context.

###### what kind of data stores in session storage?
User-Specific Data: It’s often used to store user-specific information that needs to persist only during a single session, such as:
   - User preferences (e.g., theme settings)
   - Form input values (to prevent loss of data if the user navigates away from the page)
   - Temporary authentication tokens

 State Management: Session storage can be used for managing state within single-page applications (SPAs), allowing developers to maintain application state without needing to send requests back to the server.

 Temporary Data: Any temporary data that does not need to persist beyond a single browsing session can be stored here, such as:
   - Shopping cart contents while a user browses an e-commerce site
   - Data needed for multi-step forms

##### IndexedDB
IndexedDB is a low-level API for client-side storage of significant amounts of structured data, including files and blobs. It allows developers to store and retrieve data in a way that is more powerful than traditional web storage options like localStorage or sessionStorage.

**Key Features of IndexedDB:**
1. Structured Data Storage: Unlike localStorage, which only supports string key-value pairs, IndexedDB can store complex data types such as objects, arrays, and even binary data (like image or video), in indexedDB evrtything stores in object store which I think is like a object that everything inside that object is like a key/value, that key data type can be:
   String: A sequence of characters.
   Number: A numeric value (integer or floating-point).
   Date: A JavaScript Date object.
   Array: An array of values, which allows for composite keys (keys made up of multiple values).
   Object: An object that can be used as a key if it is a structured cloneable object.
   in IndexedDB, keys must be either a primitive value (like a string, number, or date) or an object that can be serialized. Specifically:

   Primitive Values: You can use strings, numbers, and dates as keys.
   Objects: You can use objects as keys if they are structured in a way that they can be serialized into a string representation (like using JSON.stringify). However, the object must have a unique structure to serve as a key.

   Arrays
 - Arrays: You cannot directly use arrays as keys in IndexedDB. If you try to use an array as a key, it will not work as expected because arrays are reference types and do not have a unique identity when compared.

   Functions
 - Functions: Functions cannot be used as keys in IndexedDB. Functions are also reference types and cannot be serialized into a format suitable for storage in IndexedDB.

   Summary
 - Valid Keys: Strings, numbers, dates, and serializable objects (with unique structures).
 - Invalid Keys: Arrays and functions.

   If you need to use complex data structures like arrays or functions for indexing purposes, consider converting them into strings or using other methods to represent their data uniquely before storing them in IndexedDB.

   the value can be:
   IndexedDB is a low-level API for client-side storage of significant amounts of structured data, including files/blobs. When it comes to the types of values you can store in IndexedDB, here are the key points:

   JavaScript Objects: You can store plain JavaScript objects (i.e., objects created using object literals or constructors).

   Arrays: Arrays are also valid JavaScript objects and can be stored in IndexedDB.

   Primitive Types: You can store primitive types such as strings, numbers, booleans, and dates.

   Blobs and Files: You can store binary data using Blob or File objects.

   Structured Clones: IndexedDB uses a structured clone algorithm to serialize data for storage. This means that you cannot directly store functions or DOM elements because they are not serializable by the structured clone algorithm.

Summary:
- You can store:
  - Plain objects
  - Arrays
  - Primitives (strings, numbers, booleans)
  - Blobs/Files

- You cannot store:
  - Functions
  - DOM elements

If you need to store complex data structures that include functions or other non-serializable entities, you'll need to convert them into a serializable format (like JSON) before storing them in IndexedDB.


2. Asynchronous API: IndexedDB operations are asynchronous, meaning they do not block the main thread. This helps maintain a responsive user interface while performing database operations.

3. Transactions: IndexedDB supports transactions to ensure that multiple operations can be executed atomically. This means that either all operations succeed or none do, which helps maintain data integrity.

4. Indexes: You can create indexes on object stores to enable efficient querying of data based on specific properties.

5. Versioning: IndexedDB allows you to manage different versions of your database schema, making it easier to evolve your application over time without losing existing data.

6. Large Storage Capacity: It can handle larger amounts of data compared to other web storage options, making it suitable for applications that require offline capabilities or need to store large datasets.

7. Capacity: The capacity of IndexedDB is not strictly defined by a specific size limit, as it can vary based on several factors, including the browser being used and the device's available storage. However, here are some general guidelines:

   Browser Limits: Different browsers have different storage limits for IndexedDB. For example:
   - Chrome typically allows up to 6% of the available disk space.
   - Firefox has a similar approach but may allow more depending on user settings.
   - Safari has stricter limits and may prompt users when storage exceeds certain thresholds.

   User Settings: Users can often adjust their browser settings regarding storage limits, which can affect how much data can be stored in IndexedDB.
  
   Quota Management: Browsers implement quota management systems that may restrict storage based on factors like the total amount of data already stored by all web applications or specific site policies.

   Practical Limits: In practice, many applications find that they can store hundreds of megabytes to several gigabytes of data in IndexedDB without issues, but this varies widely.

For precise information about limits for a specific browser or version, it's best to consult the official documentation or resources related to that browser.
**Use Cases:**
- Offline web applications
- Storing user preferences
- Caching application state
- Managing large datasets in web applications

Overall, IndexedDB is a powerful tool for web developers looking to manage complex client-side storage needs efficiently and effectively.

###### if it's possible to store user preferences like language and dark theme on indexedDB, why local storage is preferred?
Both IndexedDB and Local Storage are web storage solutions that allow developers to store data on the client side, but they have different use cases and characteristics. Here are some reasons why Local Storage is often preferred for storing user preferences like language and dark theme settings:

1. Simplicity: Local Storage has a simpler API compared to IndexedDB. It uses a key-value pair storage model, which makes it easy to read and write data without needing to deal with transactions or complex queries.

2. Synchronous API: Local Storage operations are synchronous, meaning they execute immediately and block the main thread until the operation is complete. This can be beneficial for small amounts of data (like user preferences) where you want immediate access without the overhead of asynchronous operations.

3. Performance for Small Data: For small amounts of data (like user preferences), Local Storage is generally faster because it doesn't require the overhead associated with setting up a database structure as in IndexedDB.

4. Ease of Use: Developers often find Local Storage easier to implement for simple use cases like storing user preferences, as it requires less boilerplate code compared to using IndexedDB.

5. No Need for Complex Queries: User preferences typically involve simple key-value pairs that don’t require complex querying capabilities, which is one of the strengths of IndexedDB.

6. Browser Support: While both Local Storage and IndexedDB are widely supported in modern browsers, Local Storage has been around longer and may be more familiar to developers who have worked with web technologies for a while.

7. Data Size: For most user preference scenarios, the amount of data being stored is relatively small (usually just a few strings). Local Storage typically has a limit of about 5-10 MB per origin, which is sufficient for these use cases.

In summary, while IndexedDB offers more powerful features suitable for larger datasets and complex queries, Local Storage's simplicity and ease of use make it a preferred choice for straightforward tasks like storing user preferences such as language settings or theme choices.

###### why indexedDB operations are asynchronous while local storage and session storage are synchronous?
The difference in the synchronous and asynchronous nature of IndexedDB compared to local storage and session storage is primarily due to the design goals and use cases of these storage mechanisms.

Local Storage and Session Storage

1. Simplicity: Local storage and session storage are designed for simplicity and ease of use. They provide a straightforward key-value store that is easy to implement and understand.
  
2. Synchronous API: Both local storage and session storage operate synchronously, meaning that when you read from or write to these storages, the operation completes immediately before moving on to the next line of code. This makes them easy to use for simple tasks where performance is not a critical concern.

3. Use Cases: These storages are typically used for small amounts of data (like user preferences or session information) that do not require complex transactions or large-scale data handling.

IndexedDB

1. Complexity and Capability: IndexedDB is designed for more complex applications that require storing larger amounts of structured data, including files, blobs, or complex objects. It supports transactions, indexing, and querying capabilities similar to a database.

2. Asynchronous API: The operations in IndexedDB are asynchronous because they can involve more time-consuming processes (like reading from disk or performing complex queries). Making these operations asynchronous helps prevent blocking the main thread (UI thread) in web applications, which could lead to a poor user experience if the application becomes unresponsive during long-running operations.

3. Performance Considerations: By using an asynchronous model, IndexedDB can handle multiple requests without freezing the UI. This is particularly important for web applications that may need to perform heavy data manipulation while still providing a responsive interface.

4. Concurrency Control: The asynchronous nature also allows better management of concurrent operations through event-driven programming patterns, which can be crucial when dealing with multiple users or sessions accessing shared resources.

Summary

In summary, local storage and session storage are synchronous because they are intended for simple use cases with minimal performance concerns, while IndexedDB's asynchronous nature allows it to handle more complex scenarios involving larger datasets without blocking the main thread of execution in web applications. This design choice enhances performance and responsiveness in modern web applications where user experience is paramount.

###### we say that local storage is good for storing user preferences and etc., in what occasions indexedDB is useful?
IndexedDB is a powerful client-side storage solution that is particularly useful in several scenarios where local storage may not be sufficient. Here are some occasions when IndexedDB is advantageous:

1. Large Data Storage: IndexedDB can store significantly larger amounts of data compared to local storage, which is typically limited to about 5-10 MB. This makes it suitable for applications that need to handle large datasets, such as offline web applications or data-heavy applications (you can store video and pictures)

2. Structured Data: Unlike local storage, which only supports string key-value pairs, IndexedDB allows you to store complex structured data types (like objects) and supports transactions. This makes it ideal for applications that require more sophisticated data management.

3. Indexing and Searching: IndexedDB supports indexing, allowing for efficient querying of data based on specific fields. This is useful when you need to perform searches or filter results quickly without loading all the data into memory.

4. Transactions: IndexedDB provides support for transactions, ensuring that multiple operations can be executed atomically. This is crucial for maintaining data integrity in applications where multiple changes need to be made simultaneously.

5. Asynchronous Operations: IndexedDB operations are asynchronous, which helps prevent blocking the main thread of the application. This is particularly important in web applications where performance and responsiveness are critical.

6. Offline Capabilities: For Progressive Web Apps (PWAs) or any application that needs offline functionality, IndexedDB allows you to cache significant amounts of data locally so users can continue using the app without an internet connection.

7. Versioning and Schema Changes: IndexedDB supports versioning, allowing developers to manage changes in the database schema over time without losing existing data.

8. Complex Queries: If your application requires complex queries involving multiple fields or relationships between different datasets, IndexedDB's indexing capabilities make it easier to implement these features compared to local storage.

9. Data Relationships: If your application needs to manage relationships between different types of objects (like a relational database), IndexedDB's ability to store complex objects and use indexes can help facilitate this.

   In summary, while local storage is great for simple key-value pairs and small amounts of user preferences or settings, IndexedDB shines in scenarios requiring larger datasets, structured data management, complex queries, and robust offline capabilities.

- ###### Capacity of indexedDB: 
  The actual storage limits for IndexedDB can vary based on the browser and its settings. Most modern browsers allow a significant amount of storage for IndexedDB, often in the range of several hundred megabytes to several gigabytes per origin, but this can depend on factors such as:

1. Browser Implementation: Different browsers may have different default limits.
2. User Settings: Users can sometimes configure their browsers to limit storage.
3. Available Disk Space: The total available disk space on the user's device may also affect how much data can be stored.

   It's important to note that while there are limits, they are typically quite generous compared to other web storage options like localStorage or sessionStorage. 
##### Cookies storage
Cookies storage refers to the mechanism by which web browsers store small pieces of data (which can be sent to server automatically), known as cookies, on a user's device. These cookies are created by websites and can be used for various purposes, including:

1. Session Management: Cookies help maintain user sessions, allowing users to stay logged in as they navigate between pages.

2. Personalization: Websites can use cookies to remember user preferences and settings, such as language selection or theme choices.

3. Tracking and Analytics: Cookies can track user behavior on a website, helping site owners analyze traffic patterns and improve user experience.

4. Advertising: Cookies are often used in online advertising to track users across different sites and deliver targeted ads based on their browsing history.


user preferences like dark theme can be stored in any client-side storage like local storage or cookies, but what make this piece of data, when we store this piece of data in cookies storage, it can be sent to server automatically and has an expiration date (if it's persistent cookie), so the user preferences liked ark theme doesn't specify this piece of data is cookie or local storage data but the characteristics and the location of that data specifies the type of data.

**Types of Cookies**
1. Session Cookies: Temporary cookies that are deleted when the browser is closed. They are used to manage session information while a user is actively browsing.

2. Persistent Cookies: These remain on the user's device for a specified period or until they are manually deleted. They store information like login credentials or preferences for future visits.

3. First-party Cookies: Set by the website that the user is currently visiting.

4. Third-party Cookies: Set by domains other than the one the user is visiting, often used for tracking and advertising purposes.

- the first and second one are sorted based on the expiration date and third and fourth one based on what side is setting the cookie, when we talk about cookies and their types, referring to the first and second one.


**Storage Limitations**
- Browsers typically limit the size of individual cookies (usually around 4KB) and may also limit the total number of cookies that can be stored per domain.
- Users have control over cookie storage through browser settings, allowing them to delete existing cookies or block new ones from being set.
- The number of cookies that can be stored in a browser's cookie storage varies by browser and is subject to certain limitations. Generally, the following guidelines apply:

   Per Domain Limit: Most browsers allow a maximum of 20 to 50 cookies per domain. For example, if you have multiple subdomains (like sub1.example.com and sub2.example.com), each may have its own set of cookies.

   Total Size Limit: Browsers typically impose a size limit on the total amount of data that can be stored in cookies for a single domain, often around 4 KB per cookie. The total size limit for all cookies from a single domain can vary but is generally around 4 MB.

   Browser-Specific Limits: Different browsers may have different limits:
   - Chrome: Up to 180 cookies per domain.
   - Firefox: Up to 150 cookies per domain.
   - Safari: Similar limits, but with stricter privacy settings that may affect cookie storage.

   Expiration: Cookies can also have expiration dates, after which they are automatically deleted, which can affect how many active cookies are stored at any given time.

These limits are subject to change as browsers update their policies and features, especially with increasing focus on privacy and data management. Always refer to the latest documentation or specifications for the most accurate information regarding cookie storage limits in specific browsers.

**Privacy Considerations**
Due to privacy concerns related to tracking and data collection, many browsers now offer features that enhance user control over cookie storage, such as blocking third-party cookies or providing "Do Not Track" options. Additionally, regulations like GDPR (General Data Protection Regulation) require websites to obtain consent from users before storing certain types of cookies.

In summary, cookie storage is an essential part of web functionality that enhances user experience but also raises important privacy considerations.

- Cookies are synchronous like local storage and session storage.

- Cookies carried by the HTTP request/response header in a key/value format as below: (so key/value in HTTP request/response is the format of the cookie not things like `.txt`, they can be represented in `.txt` but that's not their inherent format)

```
Set-Cookie: sessionId=abc123; Expires=Wed, 21 Oct 2025 07:28:00 GMT; Domain=example.com; Path=/; Secure; HttpOnly; SameSite=Lax
```

- **Third party cookie**: A third-party cookie is a type of cookie that is set by a domain other than the one you are currently visiting. When you visit a website, it can store cookies on your device to remember information about your visit. These are known as first-party cookies. However, if the website includes content from other domains—such as ads, images, or social media plugins—those external domains can also set cookies on your device. These are called third-party cookies.
  Third-party cookies are often used for tracking users across different websites for purposes such as targeted advertising and analytics. For example, if you visit a site that has an advertisement from another company, that company can place a third-party cookie in your browser to track your browsing behavior across multiple sites.
  Due to privacy concerns, many web browsers have started to block third-party cookies by default or provide users with options to manage their cookie settings more strictly.

###### what kind of data stores in cookies storage?
Cookies are small pieces of data that websites store on a user's device to remember information about the user and their interactions with the site. Here are some common types of data that can be stored in cookies:

1. Session Information: Cookies can store session identifiers, allowing users to remain logged in as they navigate between pages.

2. User Preferences: Websites can save user preferences, such as language settings, theme choices, or layout configurations.

3. Authentication Tokens: Cookies often hold tokens that authenticate users, enabling them to access secure areas of a website without needing to log in repeatedly.

4. Tracking Information: Cookies can track user behavior across sessions and sites for analytics and advertising purposes, including pages visited, time spent on the site, and items added to a shopping cart.

5. Shopping Cart Contents: E-commerce sites may use cookies to remember items added to a shopping cart even if the user leaves the site and returns later.

6. Form Data: Some cookies can store information entered into forms (like names or email addresses) for auto-filling purposes on future visits.

7. User IDs: Unique identifiers for users can be stored in cookies to help personalize experiences or track user activity over time.

8. Consent Preferences: Cookies may also store information about user consent regarding privacy policies or cookie usage itself.

9. Expiration Dates: Cookies have expiration dates that determine how long they will remain on a user's device before being automatically deleted.

It's important to note that while cookies are useful for enhancing user experience, they also raise privacy concerns, especially when used for tracking purposes without explicit consent from users.

while we can store all items above, but the main purpose of cookies is to store authentication data like JWT or session id to be sent automatically to server by each request.

so why it is better to store data like user preferences like a dark theme or language on local storage than cookies? (the reason I compared local storage and cookies is because we don't want to store a user preference like theme in session storage or as session cookie because the data delete after closing the browser, tab/window but those data will persist in local storage (until you delete them manually) or as persistent cookie (until you delete them manually or their time expire) and these kind of data like theme and language is kind of data that user want to be saved and run automatically every time he/she visits the website) that's because data which store in cookies storage get sent automatically to server to tell server and help server to send some sort of information to user like what we had with authentication, we send JWT or session id to server, server identifies the user because of that JWT or session id then checks the database to create the HTML pages based on that specific user info (dynamic site concept), so storing data like user preferences in cookies to be sent to database doesn't help database to process any information, therefore storing such info in cookies is pointless and only causes extra load on server requests, hence it's better for such info to be saved in local storage than cookies storage.
Cookies are automatically sent with every HTTP request to the same domain, which can lead to unnecessary data being transmitted over the network, increasing bandwidth usage. Local storage data is only accessible via JavaScript on the client side and does not get sent with every request, making it more efficient.

for data which can be saved in cookies, the authentication methods data are the best choices such as JWT and session ID.

#### what is web storage API?
The Web Storage API is a feature of web browsers that allows websites to store data in a user's browser. It provides a way to store key-value pairs in a web application, enabling persistent data storage that can be accessed across sessions. The Web Storage API consists of two main components:

1. **Local Storage**:
   - Local Storage allows you to store data with no expiration time. The data persists even when the browser is closed and reopened.
   - It is accessible only within the same origin (protocol, host, and port).
   - Data stored in Local Storage can be retrieved using JavaScript and is limited to about 5-10 MB per origin, depending on the browser.

2. **Session Storage**:
   - Session Storage is similar to Local Storage but with a key difference: the data stored in Session Storage is only available for the duration of the page session. This means it is cleared when the tab or window is closed.
   - Like Local Storage, it also has a limit of about 5-10 MB per origin.


#### Location and format of the client-side storages on PC
for session cookies and session storages we don't have an actual physical location on our computer since they don't maintain their data after browser or its tab/window closure, so their data gets stored on RAM because RAM is a place for temporary data and after the operation is over. it removes all those data.

for local storage, indexedDB and persistent cookies, everything is different since they persist against web closure and its tab/window, they have actual physical path on our pc for storing and keeping their data, they are usually in SQLite format and their path may differ for each browser, cookies storage path is easy to find but for local storage and indexedDB, it's not an east task to find their exact location in our PC and you have to view some hidden files and do bunch of other stuff (cookies are easier to locate because they have a simpler structure and standardized file locations across browsers. In contrast, local storage and IndexedDB involve more complex implementations that abstract away their physical locations from users, focusing instead on providing developers with robust APIs for data management within web applications)

I have gathered here the (possible) places of theses storages on the PC:

##### Cookies
Cookies are typically stored in a specific location depending on the browser:

- **Google Chrome**:

```
- Windows: C:\Users\<YourUsername>\AppData\Local\Google\Chrome\User Data\Default\Cookies
  - macOS: ~/Library/Application Support/Google/Chrome/Default/Cookies
  - Linux: ~/.config/google-chrome/Default/Cookies
```

- **Mozilla Firefox**:

```
- Windows: C:\Users\<YourUsername>\AppData\Roaming\Mozilla\Firefox\Profiles\<ProfileName>\cookies.sqlite
  - macOS: ~/Library/Application Support/Firefox/Profiles/<ProfileName>/cookies.sqlite
  - Linux: ~/.mozilla/firefox/<ProfileName>/cookies.sqlite
```
##### Local Storage
Local Storage data is usually stored in a database file associated with the browser's profile:

- **Google Chrome**:
  - The data is stored in an SQLite database file located at:
```
  - Windows: C:\Users\<YourUsername>\AppData\Local\Google\Chrome\User Data\Default\Local Storage
    - macOS: ~/Library/Application Support/Google/Chrome/Default/Local Storage
    - Linux: ~/.config/google-chrome/Default/Local Storage
```
- **Mozilla Firefox**:
  - Local storage is also stored in an SQLite database file:
```
    - Windows: `C:\Users\<YourUsername>\AppData\Roaming\Mozilla\Firefox\Profiles\<ProfileName>\storage\
    - macOS: `~/Library/Application Support/Firefox/Profiles/<ProfileName>/storage/
    - Linux: `~/.mozilla/firefox/<ProfileName>/storage/
```

##### IndexedDB
IndexedDB data is stored similarly to Local Storage, often within a specific directory for each profile:

- **Google Chrome**:
  - IndexedDB files can be found at:
```
  - Windows: C:\Users\<YourUsername>\AppData\Local\Google\Chrome\User Data\Default\AppStorage
    - macOS: ~/Library/Application Support/Google/Chrome/Default/AppStorage
    - Linux: ~/.config/google-chrome/Default/AppStorage
```
- **Mozilla Firefox**:
  - IndexedDB data is also located within the profile directory:
    - All IndexedDB databases are typically found under the same storage directory as Local Storage.

Accessing These Files
1. You may need to enable viewing hidden files and folders on your operating system to access these directories.
2. The files may be in binary or SQLite format, so you might need specific tools (like SQLite Browser) to view their contents.
3. Be cautious when modifying or deleting these files, as it can affect your browsing experience.

Note
The paths mentioned above are for default profiles. If you have multiple profiles or have changed settings, the paths may differ. Always ensure that you back up any important data before making changes to these files.

#### capacity and access for client-side storages
- all of the capacity we've mentioned for each client-side storage is per origin (you can check what a origin is in pink notebook).

- each browser has its own data for the client-side storage i.e. if some specific data is stored for an specific origin in chrome, you don't have access those data in firefox and they haven't occupied the capacity of firefox.

- when you open a tab in incognito mode, no data in local storage, session storage, indexedDB and cookies persists and after closure of the browser or its tab/window for that incognito mode, any data in its client-side storage disappears.

- When you open a tab in incognito mode (or private browsing mode), it operates in a separate context from normal tabs. The data stored in IndexedDB, local storage, session storage and cookies storage in incognito mode is not shared with normal tabs, even if they are from the same origin.

- if you open multiple tabs/windows in a browser and all of them are running the same origin, what happen to data stored on their client-side storage? for local storage, indexedDB and cookies (any type), if we store data on any of these storages, that data is accessible in other tabs/windows (but the appearance of the recently inserted dat in other tabs may not be instant and it might need a refresh to show the inserted data in these storages in one tab in another tab), for instance If you have stored 2 MB of data in one tab and the total capacity for local storage is 5 MB, then in another tab (or even in the same tab), you can store up to an additional 3 MB of data. The total amount of data stored across all tabs for that origin cannot exceed the 5 MB limit, they share the same amount of storage for the storage among all other tabs/windows which share same origin but for session storage story is different, if we have multiple tabs/windows sharing the same origin, the data stored in an specific tab/window session storage won't be accessed in another tab/window session storage, for instance
  if you have stored 2 MB of data in session storage from one tab, that data is isolated to that specific tab. If you open another tab for the same origin, it will have its own separate session storage. Therefore, you can still store up to 5 MB of data in the second tab's session storage.

- when we are offline, the data stored in locals storage, indexedDB and cookies storage (persistent cookies) is accessible because they have a physical location on our PC but for session storage data and session cookies since they get get stored on RAM and they are temporary, they cannot be accessed while we're offline but there is one situation which they can be accessible in offline mode and that is when you haven't closed the browser or its tabs/windows then you lose your connection and you get offline. If you're offline and try to navigate to a website for which you have never visited before (or if the site does not support offline capabilities), your browser will show an error page indicating that there is no internet connection. However, if you've previously visited a site that utilizes local storage and has offline capabilities (like Progressive Web Apps), you may still be able to interact with some features of that site using the locally stored data.

#### Different behavior of client-side storages in keeping the data
client side storages have different behavior in keeping the data, this is how they keep them:

**local storage**: if you store data in local storage, they will remain in local storage even if we close the browser or its tab/window, data will be deleted if we delete them explicitly and manually or the data expiration time ends (for authentication methods), for instance if we store a JWT or session ID in our local storage, they will be deleted if we do it manually in our JavaScript code or the expiration time for that JWT or session ID ends.

**session storage**: if you store data in session storage, they will be deleted if we close the browser or its tab/window, also they can be deleted explicitly or manually, another way that data can be deleted is, if their expiration time ends (the expiration time should be short because the data deletes when we close the browser, so it should be short enough to data be deleted before we close the browser) (for authentication methods), for instance if we store a JWT or session ID, they will be deleted if I close the browser or its tab/windows, if the browser or its tab/window still open and the expiration time of the JWT or session ID ends, they will be deleted or JWT and session id can be deleted manually in JavaScript code.

**Persistent cookies**:  if you store data as persistent cookies in cookies storage, they will remain in cookies storage even if we close the browser or its tab/window, data will be deleted if we delete them explicitly and manually or the data expiration time ends (for authentication methods),another way that data will be deleted is, if the expiration time for persistent cookies end (we know persistent cookies have expiration time) ,for instance if we store a JWT or session ID in our cookies storage as persistent cookies, they will be deleted if we do it manually in our JavaScript code or the expiration time for that JWT or session ID ends or the expiration time of the expiration cookie ends, for example we have a JWT or session ID as our persistent cookies, the expiration time for the JWT or session id is 2 days and expiration time for persistent cookie is 3 days, so in 2days the JWT will be deleted from cookies storage, in another example the expiration time for JWT or session ID is 5 days and the expiration time for persistent cookie is 1 day, after 1day JWT or session id will be deleted from cookies storage. (but JWT is not invalidated since it has still time, so if anybody has kept the JWT, they can access your info, therefore you should black list those deleted but not invalidated JWT (I've explained the blacklisting process in pink notebook))

**session cookies**: the same rules for session storage applies for session cookies.

**indexedDB**: the same rules for local storage applies for indexedDB.


#### We know that when  a JWT deletes from a client-side storage but still has expiration time, it can be accessed so we put it in blacklist, for session IDs, what happens to their server side info if they get deleted from client-side storage?
When a session ID is deleted from client-side storage (such as cookies or local storage), the server-side information associated with that session ID remains intact until it is explicitly invalidated or expires. Here’s a breakdown of what happens:

1. Session Persistence: The server typically maintains session data in memory, a database, or another form of persistent storage. This means that even if the client deletes the session ID from their side, the server still retains the associated session data.

2. Session Expiration: Most session management systems have an expiration mechanism. If a session is not used for a certain period, it may automatically expire on the server side. This means that after a defined timeout period, the server will invalidate the session and remove any associated data.

3. Security Risks: If a user deletes their session ID but does not log out properly (which would typically involve notifying the server to invalidate that session), there could be security risks. For example, if someone else gains access to that session ID (e.g., through interception before deletion), they could potentially use it to access resources until it expires.

4. Manual Invalidation: To enhance security, many applications implement mechanisms to manually invalidate sessions when users log out or when certain conditions are met (like password changes). This ensures that even if a user deletes their client-side token/session ID, they can still ensure their server-side data is no longer accessible.

5. Blacklisting: Similar to JWT blacklisting, some systems may implement a blacklist for active sessions where specific IDs can be marked as invalidated on the server side even if they haven't expired yet.

In summary, deleting a session ID from client-side storage does not affect its state on the server side unless additional steps are taken to invalidate it there. Proper management of sessions and clear logout mechanisms are essential for maintaining security in web applications.

#### Does logging out from a website invalidates JWT on server side?
Logging out from a website does not automatically invalidate a JSON Web Token (JWT) on the server side. JWTs are stateless and self-contained, meaning that once they are issued, they remain valid until they expire or are explicitly revoked. Here’s a breakdown of how this works:

1. Stateless Nature: JWTs typically contain all the information needed for authentication within the token itself, including claims like user ID and expiration time. The server does not store session information about the token.

2. Expiration: JWTs usually have an expiration time (exp claim). Once this time is reached, the token is no longer valid, but until then, it can be used for authentication.

3. Revocation: To invalidate a JWT before its expiration (e.g., during logout), you would need to implement a revocation mechanism. This could involve:
   - Blacklist: Keeping track of invalidated tokens in a database or in-memory store (like Redis). When a user logs out, you add their token to this blacklist.
   - Short-lived Tokens: Using short-lived access tokens with refresh tokens that can be revoked when logging out.
   - Session Management: If you want more control over sessions, consider using traditional session management instead of JWTs.

4. Client-Side Handling: When a user logs out, you should also remove the JWT from client storage (like localStorage or cookies) to prevent further use on the client side.

In summary, logging out does not inherently invalidate a JWT on the server side unless you implement additional mechanisms to handle token revocation or session management.

if you have other preferences like dark theme and other stuff besides your JWT in local storage, if you can choose what to get deleted after log out, only the JWT or even other data like user preferences, usually we only set everything in this mechanism that only JWT or session ID gets deleted, so after log out only JWT or session ID deletes from local storage and other data like user preferences remain after implementation of this mechanism.   

#### Places that JWT and session id can be stored
JWT and session id can be stored in any client-side storage as any type (local storage, session storage, cookies storage (stored as persistent or session cookies ) and indexedDB), but usually they get stored in cookies storage (session id as session cookie and JWT as persistent cookie) so they can be sent automatically to server.

we can also store JWT on server, but it's idiotic if we want to do this because one of the main advantages of JWT is its stateless nature, by storing them on server, we're making them stateful and taking away all their privileges.

for session IDs we know they can be stored on server because they're stateful.

there is some mechanism which can be implemented by developers that when user logs out the JWT gets deleted from any client-side storage that it's located that this action ends our session, like for instance if our JWT is located in local storage or in cookies storages as persistent cookie, the JWT can be deleted and therefore the session ends only when the data gets deleted explicitly in code or the expiration time of JWT or the persistent cookie ends, so even if the user logs out, when the user next time searches for that site in his/her browser, they will be authenticated since the JWT still is in their local storage or cookies storage (persistent cookie) ( or in their indexedDB), so when a user logs out a site it means I want this session ends so without implementation of     log out session ending logic, the user will stay authenticated which is opposite of what the user wanted, so by help of this logic, when a user logs-out if the JWT is stored in a client-side storage which doesn't delete data after browser or its tab/window closing like local storage, persistent cookies and indexedDB (for other storages that delete data after user closing the browser or its tab/window, because usually after log-out the user close the browser or tab, basically session ends and there is no need for implementation of such logic and even if they don't close the browser or its ta/windows, they can't have access and the reason for that is kind of too long and useless so I preferred not to mention it here), the data will be deleted and you  are no longer authenticated on that website.

for session ID we have the same situation, if we don't implement such a logic, the authentication data will persist in local storage, session storage and indexedDB, if we implement the logic the session ID will be deleted both from client-side storage (that keep data after web or its tab/window closure) and server-side storage after our log-out.
#### Session ending
we know what session is:
>in simple words and in action, the term session in web development mentions to a ***duration*** which a user logs in a site and is able to access a site without logging in it again.

when user logs in the website by inserting his/her info, we sent a request to the server for that specific page, in there server generates a JWT or session id and send it back as response (JWT doesn't store in server but session ID does), then that JWT or session id stores in a client-side storage (usually cookies) and from now on session starts.

but when a session ends? based on conclusion we had in points above like [[JavaScript + misc programming concepts#Does logging out from a website invalidates JWT on server side?|here]] , [[JavaScript + misc programming concepts#Different behavior of client-side storages in keeping the data|here]] and [[JavaScript + misc programming concepts#Places that JWT and session id can be stored|here]]when the JWT or session ID gets deleted from the **client-side storage**, the session ends, bear in mind that implementation of log out session termination logic can end the logic and their absence keeps the session.

refreshing and reloading the page while the session is active , like when you are still logged in in your account, reloading and refreshing the page doesn't end your session under any circumstances ( like it doesn't matter which client storage is keeping the JWT or session ID)

restarting the computer while the browser open (this happens when a electrical crash occurs and your computer restarts all of a sudden), may or may not keep the session active, because some browsers have the default recovery process that keeps the sessions active despite of presence of  JWT or session ID in which local storage that ends up keeping up the session active but some browsers may or may not follow this rule.


### 17. Dynamic & static sites, server-side and client-side programming

#### Static sites
The diagram below shows a basic web server architecture for a _static site_ (a static site is one that returns the same hard-coded content from the server whenever a particular resource is requested). When a user wants to navigate to a page, the browser sends an HTTP "GET" request specifying its URL.

![](Images/static-sites.png)

#### Dynamic sites
A dynamic website is one where some of the response content is generated _dynamically_, only when needed. On a dynamic website, HTML pages are normally created by inserting data from a database into placeholders in HTML templates (this is a much more efficient way of storing large amounts of content than using static websites).

A dynamic site can return different data for a URL based on information provided by the user or stored preferences and can perform other operations as part of returning a response (e.g. sending notifications).

Most of the code to support a dynamic website must run on the server. Creating this code is known as "**server-side programming**" (or sometimes "**back-end scripting**").

The diagram below shows an architecture for a _dynamic website_. As in the previous diagram, browsers send HTTP requests to the server, then the server processes the requests and returns appropriate HTTP responses.

Requests for ***static resources*** are handled in the same way as for static sites (***static resources are any files that don't change — typically: CSS, JavaScript, Images, pre-created PDF files, etc.***)

- HTML is not an static resource because the data (which represents information provided by the user) stored in the database can be injected into it automatically i.e. dynamically to create new pages based on the user info and inserted data while for other type of files like the CSS and JavaScript, no code gets added to them and code inside these file are static and because that stored data in database isn't typed by the developer yet gets injected  to HTML and displayed by HTML, we say HTML isn't an static resource.

![](Images/dynamic-sites.png)

Requests for dynamic resources are instead forwarded (2) to server-side code (shown in the diagram as a _Web Application_, so server-side code which is the piece of the code that handles procedure of transferring data from database to HTML called web application in this diagram ). For "dynamic requests" the server interprets the request, reads required information from the database (3), combines the retrieved data with HTML templates (4), and sends back a response containing the generated HTML (5,6).

#### Are server-side and client-side programming the same?
Let's now turn our attention to the code involved in server-side and client-side programming. In each case, the code is significantly different:

- They have different purposes and concerns.
- They generally don't use the same programming languages (the exception being JavaScript, which can be used on the server- and client-side).
- They run inside different operating system environments.

Code running in the browser is known as **client-side code** and is primarily concerned with improving the appearance and behavior of a rendered web page. This includes selecting and styling UI components, creating layouts, navigation, form validation, etc. By contrast, server-side website programming mostly involves choosing _which content_ is returned to the browser in response to requests. The server-side code handles tasks like validating submitted data and requests, using databases to store and retrieve data and sending the correct data to the client as required.

Client-side code is written using HTML, CSS and JavaScript — it is run inside a web browser and has little or no access to the underlying operating system (including limited access to the file system).

Web developers can't control what browser every user might be using to view a website — browsers provide inconsistent levels of compatibility with client-side code features, and part of the challenge of client-side programming is handling differences in browser support gracefully.

Server-side code can be written in any number of programming languages — examples of popular server-side web languages include PHP, Python, Ruby, C#, and JavaScript (NodeJS). The server-side code has full access to the server operating system and the developer can choose what programming language (and specific version) they wish to use.

Developers typically write their code using **web frameworks**. Web frameworks are collections of functions, objects, rules and other code constructs designed to solve common problems, speed up development, and simplify the different types of tasks faced in a particular domain.

Again, while both client and server-side code use frameworks, the domains are very different, and hence so are the frameworks. Client-side web frameworks simplify layout and presentation tasks while server-side web frameworks provide a lot of "common" web server functionality that you might otherwise have to implement yourself (e.g. support for sessions, support for users and authentication, easy database access, templating libraries, etc.).

**Note:** ***Client-side frameworks are often used to help speed up development of client-side code, but you can also choose to write all the code by hand; in fact, writing your code by hand can be quicker and more efficient if you only need a small, simple website UI.***

***In contrast, you would almost never consider writing the server-side component of a web app without a framework — implementing a vital feature like an HTTP server is really hard to do from scratch in say Python, but Python web frameworks like Django provide one out of the box, along with other very useful tools.***

#### Benefits of dynamic sites
##### Efficient storage and delivery of information

Imagine how many products are available on Amazon, and imagine how many posts have been written on Facebook? Creating a separate static page for each product or post would be completely impractical.

Server-side programming (or dynamic sites) allows us to instead store the information in a database and dynamically construct and return HTML and other types of files (e.g. PDFs, images, etc.). It is also possible to return data (JSON, XML, etc.) for rendering by appropriate client-side web frameworks (this reduces the processing burden on the server and the amount of data that needs to be sent).

The server is not limited to sending information from databases, and might alternatively return the result of software tools, or data from communications services. The content can even be targeted for the type of client device that is receiving it.

Because the information is in a database, it can also more easily be shared and updated with other business systems (for example, when products are sold either online or in a shop, the shop might update its database of inventory).

##### Customized user experience
Servers can store and use information about clients to provide a convenient and tailored user experience. For example, many sites store credit cards so that details don't have to be entered again. Sites like Google Maps can use saved or current locations for providing routing information, and search or travel history to highlight local businesses in search results.

A deeper analysis of user habits can be used to anticipate their interests and further customize responses and notifications, for example providing a list of previously visited or popular locations you may want to look at on a map.

##### Controlled access to content
Server-side programming allows sites to restrict access to authorized users and serve only the information that a user is permitted to see.

Real-world examples include social-networking sites which allow users to determine who can see the content they post to the site, and whose content appears in their feed.

##### Notifications and communication
Servers can send general or user-specific notifications through the website itself or via email, SMS, instant messaging, video conversations, or other communications services.

A few examples include:

- Facebook and Twitter send emails and SMS messages to notify you of new communications.
- Amazon regularly sends product emails that suggest products similar to those already bought or viewed that you might be interested in.
- A web server might send warning messages to site administrators alerting them to low memory on the server, or suspicious user activity.

**Note:** The most common type of notification is a "confirmation of registration". Pick almost any large site that you are interested in (Google, Amazon, Instagram, etc.) and create a new account using your email address. You will shortly receive an email confirming your registration, or requiring acknowledgment to activate your account.

so in a nutshell your email or contact info stores in database on server and site sends you different type of messages via those stored emails automatically by using the advantages of dynamic sites.

##### Data analysis
A website may collect a lot of data about users: what they search for, what they buy, what they recommend, how long they stay on each page. Server-side programming can be used to refine responses based on analysis of this data.

For example, Amazon and Google both advertise products based on previous searches (and purchases).

**Note:** If you're a Facebook user, go to your main feed and look at the stream of posts. Note how some of the posts are out of numerical order - in particular, posts with more "likes" are often higher on the list than more recent posts.

Also look at what kind of ads you are being shown — you might see ads for things you looked at on other sites. Facebook's algorithm for highlighting content and advertising can be a bit of a mystery, but it is clear that it does depend on your likes and viewing habits!


#### Another overview of static and dynamic sites
Static and dynamic sites are two fundamental types of websites, each with distinct characteristics and use cases.

**Static Sites**
Definition: A static site consists of fixed content that does not change unless manually updated. Each page is a separate HTML file, and the same content is served to every user.

Characteristics:
- Content Delivery: The server delivers the same HTML files to all users.
- Speed: Generally faster because there’s no server-side processing; the browser simply retrieves and displays the files.
- Simplicity: Easier to host and deploy since they don’t require a database or server-side scripting.
- Use Cases: Ideal for portfolios, blogs, documentation, landing pages, or any site where content doesn’t change frequently.

Technologies Used:
- HTML
- CSS
- JavaScript (for client-side interactivity)

**Examples:**
1. Personal Portfolio: A web developer's portfolio showcasing their work, skills, and contact information. Each project might have its own HTML page.
2. Landing Pages: Marketing landing pages that provide information about a product or service without requiring user interaction beyond basic navigation.

**Dynamic Sites**
Definition: A dynamic site generates content on-the-fly based on user interactions or other variables. The content can change based on user input, database queries, or other factors.

Characteristics:
- Content Delivery: The server processes requests and generates HTML dynamically before sending it to the user.
- Interactivity: Can provide personalized experiences (e.g., user accounts, comments sections).
- Complexity: More complex to develop and maintain due to the need for databases and server-side programming languages.
- Use Cases: Suitable for e-commerce sites, social networks, forums, or any application requiring frequent updates or user interaction.

Technologies Used:
- Server-side languages (e.g., PHP, Python, Ruby)
- Databases (e.g., MySQL, PostgreSQL)
- Front-end technologies (HTML, CSS, JavaScript)

**Examples:**
1. Social Media Platforms: Websites like Facebook or Twitter where users can create accounts, post updates, comment on others posts, etc., all of which require real-time data processing.
2. E-commerce Sites: Online stores like Amazon that display products based on user preferences, search queries, and inventory levels; they also handle transactions dynamically.

#### does using a database for our website, makes our website dynamic?

Yes, using a database for your website typically makes it dynamic. Here’s how it works:
How a Database Contributes to a Dynamic Website
Content Generation: A dynamic website retrieves data from a database to generate content on-the-fly. For example, when a user requests a page, the server can query the database to fetch the relevant information (like user profiles, blog posts, or product details) and display it.
User Interaction: Dynamic sites often allow users to interact with the content. For instance, users can submit forms, leave comments, or make purchases. The database stores this information, allowing the site to update and reflect changes based on user actions.
Personalization: Dynamic websites can provide personalized experiences by tailoring content based on user preferences or behavior. For example, an e-commerce site might show different products to different users based on their browsing history, which is stored in the database.
Example
Blog: A blog that uses a database can allow users to create accounts, post comments, and manage their profiles. Each time a user visits the blog, the server queries the database to display the latest posts, comments, and user-specific content.
In contrast, a static website does not use a database; its content is fixed and does not change unless the developer manually updates the HTML files. Therefore, the presence of a database is a key characteristic of dynamic websites.

#### if I create a site which in that site user can insert a book name to a bar and by clicking a button, that book name gets added to a list and displayed on the screen but those name don't get added to any database and those name just get added to HTML code. I was wondering is this site, dynamic or static? 

In the scenario you described, the site would be considered dynamic in terms of user interaction, but it would not be dynamic in the traditional sense of using a server-side database, since by dynamism, we mean dynamism on server side, basically this site or application we have mentioned above isn't dynamic. 

Explanation
Dynamic Interaction:
The site allows users to input a book name and see it added to a list on the screen. This interaction is dynamic because the content displayed changes based on user input. The JavaScript code running in the browser is modifying the HTML in real-time to reflect the user's actions.
No Persistent Storage:
Since the book names are not being stored in a database and are only added to the HTML code in the user's browser, the changes are not persistent. If the user refreshes the page or navigates away, the list of book names will be lost. This means that while the interaction is dynamic, the data is not stored in a way that persists beyond the current session.

Conclusion
So, while the site exhibits dynamic behavior by allowing user input and updating the display accordingly, it lacks the persistence and server-side data management typically associated with fully dynamic sites. In summary, this site does not have the characteristics of a dynamic site.

#### if I use a fetch method in my JavaScript file to retrieve data from an API in my site, does using this API makes my site dynamic? 
Yes, using a fetch method in your JavaScript file to retrieve data from an API can make your site dynamic. Here’s how it works:

How Fetching Data from an API Contributes to a Dynamic Site

Real-Time Data Retrieval: When you use the fetch method to call an API, your site can retrieve data in real-time. This means that the content displayed on your site can change based on the data returned from the API, making it dynamic.
User Interaction: If your site allows users to interact with it (e.g., submitting forms, clicking buttons), you can use the fetch method to send requests to the API based on those interactions. The site can then update the displayed content without needing to reload the entire page.
Dynamic Content Updates: For example, if you have a weather application that fetches data from a weather API, the displayed weather information can change based on the user's location or the time of day. Each time the user requests new data (like searching for a different city), the fetch method retrieves the latest information from the API.
since a new data is getting added to the page from a database of another site or a database which is not ours and they are making changes in our code without developer doing anything to display those data **one by one** and each data changes dynamically and automatically like price of stock market shares which you get the API and display those prices in your website and they change every second automatically without needing to insert those prices manually in oiur code, theses price changes are persistent because if we reload the page, the changes go on.
While the use of an API and the fetch method does not necessarily mean your entire site is dynamic, it allows for dynamic behavior in specific parts of your site. The content can change based on user interactions or external data, which is a hallmark of dynamic websites.

using the fetch method in your JavaScript file to retrieve data from an API can make your site dynamic. Here's how it contributes to the dynamism of your site:

1. Real-Time Data: By fetching data from an API, you can display real-time information on your site. For example, you could show live updates, user-generated content, or data that changes frequently without needing to reload the page.

2. User Interaction: Dynamic sites often respond to user interactions. By using fetch, you can update parts of your webpage based on user actions (like form submissions or button clicks) without a full page refresh.

3. Content Updates: If the API provides updated content (like news articles, product listings, etc.), your site can automatically reflect these changes whenever new data is fetched.

#### if using local storage doesn't make my site dynamic ,why using fetch method make my site dynamic?
The distinction between using local storage and the fetch method in terms of making a website dynamic lies in how data is retrieved and updated.

**Local Storage**
- Definition: Local storage is a web storage mechanism that allows you to store data in the user's browser. This data persists even after the user closes the browser or navigates away from the page.
- Usage: It is typically used for storing small amounts of data, such as user preferences, session information, or cached data.
- Dynamic Nature: While local storage can help maintain state across sessions (e.g., remembering user settings), it does not inherently make your site dynamic. The content stored in local storage is static until explicitly updated by your JavaScript code. It does not change based on external factors or real-time updates.

**Fetch Method**
- Definition: The fetch method is an API that allows you to make network requests to retrieve resources from a server (like APIs) asynchronously.
- Usage: It is commonly used to get data from a server, such as fetching user profiles, product information, or any other dynamic content that can change over time.
- Dynamic Nature: Using fetch makes your site dynamic because it allows you to pull in fresh data from an external source whenever needed. For example, if you fetch live weather data from an API, your site can display current weather conditions that update automatically without needing a page refresh.

In summary:
- Local Storage provides persistence but does not inherently update content dynamically; it relies on manual updates through JavaScript.
- Fetch Method enables real-time interaction with external resources, allowing your site to display up-to-date information and respond to changes dynamically.

By combining both techniques—using fetch to retrieve fresh data and local storage to cache certain elements—you can create a more responsive and engaging web experience.

#### Final interpretation of a dynamic site
dynamic site, a site that the content and the behavior of the html page can not be made by the developer, like in fetch(), if we fetch price of a share in stock market, we don't know what price will be displayed in our html, for signing up in a site, we don't know what the info of the specific user is, so we can't create a page for it, that's why we add a database to our site and a place holder in our html that when user inserted its info in  the html inputs, those info gets stored in the database and then injected in our HTML and a new page creates.

in case of local storage because everything is set by the developer and no new things is not going to occur by the user and everything situation is anticipated by the developer, like we say if the user clicked on this button, save "dark" in the local storage and make the screen dark, you see everything is anticipated by the developer, so there is no dynamism in here and everything is static(dynamic=the html content is able to create content based on user inputs which developer hasn't predicted them and is persistent (that's why we use database for persistency because everything gets stored), the dynamic example of instance above is, when user insert a color in an input or box and then that color stores in a database (for persistency) then that color gets injected to our html placeholder and then the screen background gets that inserted color but if we don't store that color and that inserted color becomes the background color of our background, this background color isn't persistent because if I reload the site, that color will disappear and everything will becomes like its first, so two main feature of dynamism is persistency and unpredictability for a specific content (HTML placeholder and template code aren't predictable since they are typed to make our site dynamic) by the developer.

#### when we insert an API endpoint in our fetch() method to retrieve data from somewhere, where actually that data retrieves, a database?
When you use the fetch() method in JavaScript to retrieve data from an API endpoint, the data is typically retrieved from a server, which may be connected to a database. Here's a breakdown of how this process generally works:

1. Client-Side Request: When you call fetch() with a specific API endpoint, your client-side application (like a web app) sends an HTTP request to that endpoint.

2. API Endpoint: The API endpoint is usually part of a web server that is set up to handle requests. This server could be built using various technologies (e.g., Node.js, Python with Flask or Django, Ruby on Rails, etc.).

3. Server Processing: Upon receiving the request at the API endpoint, the server processes it. This may involve:
   - Validating the request.
   - Performing any necessary business logic.
   - Interacting with a database if needed.

4. Database Interaction: If the requested data is stored in a database (like MySQL, PostgreSQL, MongoDB, etc.), the server will query that database to retrieve the relevant information.

5. Response Generation: After retrieving the data from the database (or performing other operations), the server formats this data into a response format (commonly JSON) and sends it back to the client.

6. Client-Side Handling: Once your client-side application receives this response from fetch(), you can then manipulate or display this data as needed in your application.

In summary, while fetch() itself does not directly interact with databases, it facilitates communication between your client-side code and an API that often retrieves data from a database on behalf of your application.

### 18. AJAX
AJAX, which stands for Asynchronous JavaScript and XML, is a set of web development techniques that allows web applications to communicate with a server asynchronously without interfering with the display and behavior of the existing page. This means that data can be sent and received in the background, enabling a more dynamic and responsive user experience.

Key Components of AJAX:

1. Asynchronous Communication: AJAX allows web pages to send and receive data from a server asynchronously. This means that users can continue interacting with the page while data is being fetched or sent in the background.

2. JavaScript: AJAX relies heavily on JavaScript to make requests to the server and handle responses. JavaScript's ability to manipulate the Document Object Model (DOM) allows developers to update parts of a web page without reloading it.

3. `XMLHttpRequest`: This is the core technology behind AJAX. It is an API available in web browsers that allows scripts to perform HTTP requests to servers. Although XML was originally used for data interchange, other formats like JSON (JavaScript Object Notation) are now more commonly used due to their simplicity and ease of use with JavaScript.

4. Data Formats: While XML was traditionally used for data exchange, JSON has become more popular because it is easier to work with in JavaScript. Other formats like HTML or plain text can also be used depending on the application needs.

5. Server-Side Technologies: AJAX can work with various server-side technologies (like PHP, Node.js, Python, Ruby on Rails, etc.) that process requests and send back responses.

Benefits of Using AJAX:

- Improved User Experience: By allowing parts of a webpage to update without requiring a full reload, AJAX creates smoother interactions.
- Reduced Server Load: Since only specific data is requested rather than entire pages, this can lead to reduced bandwidth usage.
- Faster Interactions: Users experience faster response times as they do not have to wait for entire pages to reload.

`fetch()` method uses AJAX technology, since `fetch()` fetches data from an API into our website without reloading our website, this no reloading option causes the user to keep its state like something user is inserting in a from an by reloading the webpage can disappear and gives user better interaction, imagine a site that fetches currency rates every second, to reload every single second, you can't use that website with reloading in every second.

# 19. Web workers (Dedicated, Shared and Service web workers)

we know that JavaScript is a single-thread language, which means each task gets handled in a single core but you can turn the JavaScript into a multi-threaded language with the help of web workers, so why we should have multi-threaded language while the nature of our language is single-threaded? because in the single-threaded concept of JavaScript, some task which are     time-consuming like `setTimeout()` or `setInterval()` are predictable and we mark them as asynchronous task to not block our main UI but if we have some sort of tasks which are not sort of these methods? like we have a function that display the number in Fibonacci sequence based on the order we pass as argument, if the argument is large, this function process may last too long, so in this scenario, web workers can be handy to off-load this CPU-intensive task from main thread and transfer it to another thread, one prominent difference between multi-threaded language like Java and the web workers in JavaScript (which provides multi-threading feature) is in multi-threaded language, thread and main thread can access each other variables and values and theses values and variables get **shared**, so when we have variable `lome` in the main thread, the variable `lome` we have in another thread is the same thing, this feature causes ***race conditions*** but in    web workers the variable or value doesn't get shared and it gets copied so we won't have race condition, each web workers has its own context and scope and not connected to another thread or main thread therefore there is no race condition.

we have 3 types of web workers: ***Dedicated workers, Shared workers and Service worker***

service workers are usually adopted in `caching` mechanism and needs knowledge of `fetch()`, so I talk about it later.

## execution order in web workers
```javascript
//test.js (main thread)
const myworker= new SharedWorker("worker.js");

setTimeout(()=>console.log("hey81"),8);
setTimeout(()=>console.log("hey82"),280);
setTimeout(()=>console.log("hey83"),8000);

const pr=new Promise((resolve,reject)=>{
resolve();
})

pr.then(()=>{
  console.log("hey7")
})

console.log("hey1");

myworker.port.postMessage("hi worker from 1");

console.log("hey2");

myworker.port.onmessage=(e)=>{

setTimeout(()=>console.log("loooooo"),7);
setTimeout(()=>console.log("looooo2"),270);
setTimeout(()=>console.log("loooooo3"),7000);

  console.log(e.data);
  console.log("looooo4");

  pr.then(()=>{
    console.log("looooo5")
  })
}

setTimeout(()=>console.log("hey61"),6);
setTimeout(()=>console.log("hey62"),260);
setTimeout(()=>console.log("hey63"),6000);

console.log("hey3");

pr.then(()=>{
  console.log("hey5")
})

myworker.port.postMessage("hi worker from 1 second time");

myworker.port.onmessage=(e)=>{

  setTimeout(()=>console.log("hey71"),7);
  setTimeout(()=>console.log("hey72"),270);
  setTimeout(()=>console.log("hey73"),7000);

    console.log(e.data);
    console.log("hey4");
    pr.then(()=>{
      console.log("hey6")
    })
  }
  ```

```javascript
//test2.js (another thread)
const myworker= new SharedWorker("worker.js");

setTimeout(()=>console.log("hey81"),8);
setTimeout(()=>console.log("hey82"),280);
setTimeout(()=>console.log("hey83"),8000);

const pr=new Promise((resolve,reject)=>{

resolve();

})

pr.then(()=>{

  console.log("hey7");

})

console.log("hey1");

myworker.port.postMessage("hi worker from 1");

console.log("hey2");

myworker.port.onmessage=(e)=>{

setTimeout(()=>console.log("hey71"),7);
setTimeout(()=>console.log("hey72"),270);
setTimeout(()=>console.log("hey73"),7000);

  console.log(e.data);

  console.log("hey4");

  pr.then(()=>{
    console.log("hey6")
  })
}

setTimeout(()=>console.log("hey61"),6);
setTimeout(()=>console.log("hey62"),260);
setTimeout(()=>console.log("hey63"),6000);

console.log("hey3");

pr.then(()=>{
  console.log("hey5");
})
```

```javascript
//worker.js (shared worker)
const pr=new Promise((resolve,reject)=>{
  resolve();
})

pr.then(()=>{
  console.log("hi6")
})

setTimeout(()=>console.log("hey811"),8);
setTimeout(()=>console.log("hey822"),280);
setTimeout(()=>console.log("hey833"),8000);

onconnect=(e)=>{
const port=e.ports[0];

console.log("hi1");
console.log("hi2");

setTimeout(()=>console.log("hey711"),7);
setTimeout(()=>console.log("hey722"),270);
setTimeout(()=>console.log("hey733"),7000);

  pr.then(()=>{
    console.log("hi7");
  })

port.onmessage=(e)=>{
setTimeout(()=>console.log("hey611"),6);
setTimeout(()=>console.log("hey622"),260);
setTimeout(()=>console.log("hey633"),6000);

  console.log(e.data);

  console.log("hi3");
  port.postMessage("piss off pls");
  console.log("hi4");

  pr.then(()=>{
    console.log("hi8")
  })

  port.postMessage("woow2");
}
console.log("hi5");
}

console.log("what's this?");

pr.then(()=>{
  console.log("hi9")
})

onconnect=(e)=>{
const port=e.ports[0];
port.onmessage=(e)=>{
console.log(e.data);
port.postMessage("huuuuuuuuuuuuuu");
}
}
  
setTimeout(()=>console.log("hey511"),5);
setTimeout(()=>console.log("hey522"),250);
setTimeout(()=>console.log("hey533"),5000);
```

in example above, we have implemented a shared web worker example, which in that `test.js` and `test2.js` scripts are using the `worker.js` shared web worker, we could define `worker.js` as dedicated web worker but we didn't since in that scenario more RAM and CPU would be used for a task (code in web worker) which is mutual for both scripts, instead we used shared web worker to save resources.

for declaring the script, we use `new SharedWorker()` syntax, for communicating with the worker from scripts, first we have to use the variable that we've declared our shared web worker in it, which in this case is `my worker` (in both of the scripts), then we use a `port` property next to it which allows us to communicate with our workers life for sending message to worker we have: `myworker.port.postMessage("hi worker from 1")` and for receiving message we have `myworker.port.onmessage=(e)=>{}`, meanwhile in the worker, we have `onconnect`, which connect is an exclusive event for shared worker that enables multiple scripts use the shared worker while keeping the resources in our CPU and RAM at its minimum, then after that we have to use `event.ports` property to create a port that enables communication with script, for communicating with script we have to put the variable we have declared `events.ports[0]` in it which in this case is `port` (this `port` in worker is a random name and it can be anything and bear in mind that port in the script is a built-in property which we use to connect script to **shared worker** but port in the shared worker is a random variable that can be named anything)

**Note:** never try to implement message event with `addEventListener()` because in that case, the shared worker logic gets complicated and we have to use extra methods which makes our code complex.

to access message sent from/to workers, we use `event.data` or `e.data` (`e` or `evnet` can be any other names like `jack`) in `onmessage` event.

**Note:** `postMessage()` is for sending message and `onmessage` is for receiving message.

the execution order in shared web worker is like:
the interpreter starts to interpret the code, if it's a synchronous code it runs it, then if it confronts the `new SharedWorker()`, it starts to create the worker and connect it to our script, this creation is a synchronous take in our script but it takes a little bit of time to create, so when our interpreter reaches this web worker syntax, it cannot be executed ASAP and see the results of web worker instantly, so mean while that this worker is getting created, other code runs,  before we can see the result of web workers, the synchronous code in our script and promise run and sometimes we can see `setTimeout`s with short time like 8 ms in our results but this `setTimeout`s presence before web worker results is not certain and they can occur before web workers result, alongside of the short timed `setTimeout()` of workers or even before the long timed `setTimeout`s of whole code, their location differs each time, this difference and uncertainty is because of the load that CPU has while computing our code., in our script when we reach `postMessage()`, a message will be sent to worker, this method is synchronous, when we reach `onmessage`, this `onmessage` is synchronous also but it goes in the message queue and waits for any incoming message from workers.

in shared workers after it got created, `onconnect` is a synchronous code but comparing to other codes in the worker, it takes time to activate, so I think like `onconnect` it goes into message queue , since `onmessage` is inside `onconnect`, so first it takes time for `onconnect` to load, then it runs code inside `onconnect` but when it reaches the `onmessage` it takes time to load again.

so the code in a shared web worker runs like this, first the synchronous code and promises out of scope of `onconnect` runs, then maybe the `setTimeout`s with short time runs, after that the synchronous and promises inside `onconnect` runs then may be the `setTimeout` with short time runs, after that `onmessage` loads, so first the synchronous and promise code runs, then    `setTimeout`s with short time, after that all the `setTimeout`s (those aren't short) from the script and workers run based on their time.

so this is the whole execution order of script and shared worker: first the synchronous and promise in script runs, then maybe `setTimeout`s with short time in script run, then the the synchronous and promise in first shared web worker in script based on its code position, then maybe the short `setTimeout`s in the web worker ( not those in `onmessage` and `onconnect`), then the synchronous and promises in `onconnect`, then maybe the short `setTimeout` inside `onconnect` run, then synchronous code and promise in `onmessage`, then short `setTimeout`s in `onmessage`, after that all of the remaining `setTimeout`s ( not the short one) run based on their timing.

for the dedicated web worker we have same thing but the `onconnect` part omits: first the synchronous and promise in script runs, then maybe `setTimeout`s with short time in script run, then the the synchronous and promise in first shared web worker in script based on its code position, then maybe the short `setTimeout`s in the web worker ( not those in `onmessage`), then synchronous code and promise in `onmessage`, then short `setTimeout`s in `onmessage`, after that all of the remaining `setTimeout`s ( not the short one) run based on their timing.

**Note:** since we don't have short `setTimeout`s in real life and we only we have regular      `setTimeout`s, so that's why we shouldn't worry about long `setTimeout`s.

**Note:** in shared web workers, out of `onconnect` context you can't use `postMessage` and ` onmessage`.

**Note:** without using `onconnect` and `port` word in the shared web worker(`port` should be used both in shared web worker and script), shared web workers won't work. 

```javascript
//test.js (script)

const myworker= new Worker("worker.js");

setTimeout(()=>console.log("hey81"),8);
setTimeout(()=>console.log("hey82"),280);
setTimeout(()=>console.log("hey83"),8000);

const pr=new Promise((resolve,reject)=>{
resolve();
})

pr.then(()=>{
  console.log("hey7")
})

console.log("hey1");
myworker.postMessage("hi worker from 1");
console.log("hey2");
myworker.onmessage=(e)=>{

  

setTimeout(()=>console.log("loooooo"),7);
setTimeout(()=>console.log("looooo2"),270);
setTimeout(()=>console.log("loooooo3"),7000);

  console.log(e.data);

  console.log("looooo4");

  pr.then(()=>{

    console.log("looooo5")

  })

}

  

setTimeout(()=>console.log("hey61"),6);

setTimeout(()=>console.log("hey62"),260);

setTimeout(()=>console.log("hey63"),6000);

  

console.log("hey3");

  

pr.then(()=>{

  console.log("hey5")

})

  

myworker.postMessage("hi worker from 1 second time");

  

myworker.onmessage=(e)=>{

  setTimeout(()=>console.log("hey71"),7);

  setTimeout(()=>console.log("hey72"),270);

  setTimeout(()=>console.log("hey73"),7000);

    console.log(e.data);

    console.log("hey4");

    pr.then(()=>{

      console.log("hey6")

    })

  }

```

```javascript
//worker.js (web worker)

const pr=new Promise((resolve,reject)=>{
  resolve();
})

  

pr.then(()=>{
  console.log("hi6")
})

setTimeout(()=>console.log("hey811"),8);
setTimeout(()=>console.log("hey822"),280);
setTimeout(()=>console.log("hey833"),8000);


onmessage=(e)=>{
setTimeout(()=>console.log("hey611"),6);
setTimeout(()=>console.log("hey622"),260);
setTimeout(()=>console.log("hey633"),6000);

  console.log(e.data);
  console.log("hi3");
  postMessage("piss off pls");
  console.log("hi4");

  pr.then(()=>{
    console.log("hi8")
  })
  postMessage("woow2");
}

console.log("hi5");

console.log("what's this?");

pr.then(()=>{
  console.log("hi9")
})


onmessage=(e)=>{
console.log(e.data);
postMessage("huuuuuuuuuuuuuu");
}

setTimeout(()=>console.log("hey511"),5);
setTimeout(()=>console.log("hey522"),250);
setTimeout(()=>console.log("hey533"),5000);

```

there is no `onconnect` here and no need to mention `ports` in here, since these web workers are dedicated, they don't need ports to specify the script. 

## What is script in programming?

In programming, a "script" generally refers to a type of program or code that is written in a scripting language and is typically interpreted rather than compiled. Scripts are often used to automate tasks, manipulate data, or control other software applications. Here are some key characteristics and aspects of scripts in programming:

1. **Interpreted Language**: Scripts are usually written in interpreted languages, meaning that they are executed line-by-line by an interpreter at runtime rather than being compiled into machine code beforehand. Examples of scripting languages include JavaScript, Python, Ruby, Perl, and Bash.

2. **Automation**: Scripts are commonly used to automate repetitive tasks, such as file manipulation, data processing, and system administration. For example, a shell script can automate the process of backing up files or running a series of commands in a terminal.

3. **Ease of Use**: Scripting languages are often designed to be easy to write and read, making them accessible for beginners and allowing for rapid development. They typically have simpler syntax and built-in functions for common tasks.

4. **Short-lived Programs**: Scripts are often shorter and less complex than traditional programs. They are usually designed to perform specific tasks rather than being full-fledged applications.

5. **Integration**: Scripts can be used to integrate different software systems or components. For example, a script can be used to connect a web application to a database, fetch data from an API, or manipulate files on a server.

6. **Environment-Specific**: Scripts can be environment-specific, meaning they may rely on certain software or system configurations to run. For example, a Bash script is designed to run in a Unix-like shell environment.

7. **Execution Context**: Scripts can run in various contexts, such as web browsers (JavaScript), server environments (Node.js), or command-line interfaces (Python, Bash).

8. **Dynamic Behavior**: Many scripting languages support dynamic typing and other features that allow for flexible and dynamic behavior, making it easier to write code that can adapt to different situations.

In summary, a script in programming is a small program written in a scripting language that is typically interpreted and used to automate tasks, manipulate data, or control other software. Scripts are characterized by their ease of use, rapid development capabilities, and ability to integrate with other systems.

## we call a code file written in a interpretative language a script, what do we call same code file coded with a compiling language ?

A code file written in a compiled language is typically referred to as a **"source file."** The term "source file" indicates that the code is written in a high-level programming language (such as C, C++, Java, or Go) and needs to be compiled into machine code or bytecode before it can be executed.

Here are some key points regarding source files in compiled languages:

1. **Compilation**: Source files are processed by a compiler, which translates the high-level code into machine code or an intermediate representation (like bytecode) that can be executed by a computer's hardware or a virtual machine.

2. **File Extensions**: Source files usually have specific file extensions that indicate the programming language. For example:
   - C: `.c`
   - C++: `.cpp` or `.cc`
   - Java: `.java`
   - Go: `.go`

3. **Build Process**: The compilation process often involves multiple steps, including preprocessing, compiling, linking, and generating an executable file. This process can be managed using build systems or tools.

4. **Executable Files**: After compilation, the output is typically an executable file (e.g., `.exe` on Windows, or a binary file on Unix-like systems) that can be run directly by the operating system.

5. **Static vs. Dynamic Typing**: Compiled languages often have static typing, meaning that variable types are checked at compile time, whereas interpreted languages may support dynamic typing.

In summary, while code files written in interpreted languages are commonly called "scripts," those written in compiled languages are referred to as "source files."

## we call a code file written in a interpretative language a script, can we call same code file coded with a compiling language, an script?

While the term "script" is typically associated with code written in interpreted languages, it is not strictly incorrect to refer to a code file written in a compiled language as a "script" in certain contexts. However, doing so may lead to confusion, as the terms have different connotations in the programming community. Here are some considerations:

1. **Common Usage**: The term "script" is most commonly used to describe small, often short-lived programs written in interpreted languages (like JavaScript, Python, or Ruby) that automate tasks or perform specific functions. In contrast, "source file" is the more standard term for code written in compiled languages (like C, C++, or Java).

2. **Context Matters**: In some contexts, especially in discussions about automation or configuration (e.g., shell scripts, build scripts), you might hear the term "script" used to describe code written in compiled languages. For example, a Makefile or a build script that compiles C code could be informally referred to as a script.

3. **Flexibility of Language**: The programming community is flexible with terminology, and some developers may use "script" to refer to any small program, regardless of whether it is interpreted or compiled. However, this usage is less common and may not be universally understood.

4. **Clarity**: To avoid confusion, it's generally best to use "source file" for compiled languages and "script" for interpreted languages. This distinction helps clarify the nature of the code and the execution model being used.

In summary, while you can technically refer to a code file written in a compiled language as a "script" in certain contexts, it is more accurate and clearer to use "source file" for compiled languages and reserve "script" for interpreted languages.

***in a nutshell, a file coded in an interpretative language like JavaScript called a script but script can also refer to a part of a file, like a snippet or piece of code which is part of our file (not all of our file), it depends on the situation to adopt which aspect, also for the same file coded in a compiled language, although it's called a `source file` but we can still call them the script, same here, script is not supposed to be a whole file, it can also be an snippet.***

**Dedicated Worker:** in dedicated workers, we have a script which we declare the worker inside it and then we have the worker which we type our worker code in it. 

**Shared worker:** imagine you have a CPU-intensive task which we want to place inside of a worker, if this task only wants to be used by one script, then we use dedicated web worker, but if this task which we have in worker is a type of a task that we want to be used for multiple scripts i.e. there is a mutual CPU-intensive task that multiple scripts want to use that, if we declare this CPU-intensive task as dedicated worker and call it in our script, for each script that used that dedicated worker, beside the thread dedicated to that script, another script will be allocated to web worker, for instance we have 4 scripts that has the same CPU-intensive task, we create a dedicated              web worker for that CPU-intensive task and call that dedicated web worker in each of those 4 threads,  in total 8 threads will be occupied (4 for scripts and 4 for web workers) but for the same the same scenario, instead of dedicated web worker, we use shared web worker, only 5 threads will be occupied but how? when we call a shared web worker in an script, second another script wants to call that shared web worker, it checks if any thread allocated to that specific worker or not, if yes it connects to that specific thread but if not, it allocates a thread to that worker, that why in the example we brought up, only 5 threads will be occupied, (4 for the scripts and 1 for shared web worker), so if you have a task with heavy computation that is mutual in multiple scripts, define that web worker as shared web worker to save resources and your CPU and RAM, while if you had scripts that want different workers which each of them is for a distinct task, use 
dedicated web workers.

we use a dedicated web worker in our script with `new Worker()` syntax and for                       shared web workers, we use `new SharedWorker()` in our script, for communication, we use `postMessage()` (for sending messages from/to main thread) and `onmessage` for receiving messages.  


## why in a programming language like JavaScript which is designed to be single-threaded, we have a feature like web worker that enables multi-threading feature?

JavaScript is primarily designed to be single-threaded, meaning that it executes code in a single sequence, which helps avoid issues like race conditions and makes it easier to reason about the flow of execution. However, this single-threaded nature can lead to performance bottlenecks, especially when dealing with computationally intensive tasks or I/O operations that can block the main thread and make the application unresponsive.

To address these limitations, the Web Workers API was introduced. Here are some reasons why Web Workers are beneficial in a single-threaded environment like JavaScript:

1. **Non-blocking Execution**: Web Workers run in the background, separate from the main execution thread. This allows long-running tasks to be executed without blocking the user interface, keeping the application responsive.

2. **Parallel Processing**: While JavaScript itself is single-threaded, Web Workers allow developers to take advantage of multi-core processors by running multiple workers in parallel. Each worker can perform tasks independently, which can significantly improve performance for CPU-intensive operations.

3. **Isolation**: Web Workers operate in a separate global context, meaning they do not share the same memory space as the main thread. This isolation helps prevent issues related to shared state and makes it easier to manage concurrency.

4. **Asynchronous Communication**: Communication between the main thread and workers is done through a messaging system (using `postMessage`), which is asynchronous. This allows the main thread to continue executing while waiting for results from the worker.

5. **Use Cases**: Web Workers are particularly useful for tasks such as image processing, data manipulation, and handling large datasets, where the main thread would otherwise be blocked, leading to a poor user experience.

In summary, while JavaScript is single-threaded, Web Workers provide a way to perform multi-threaded operations, allowing developers to create more efficient and responsive applications by offloading heavy computations to background threads.

## what's a message?
A value that is cloned and not shared is called _message_. As you will probably know by now, _messages_ can be sent to and from the main thread by using `postMessage()`, and the `message` event's data attribute contains data passed back from the worker.

## I was reading a spec about web workers and confronted following text, what does it mean? "Data passed between the main page and workers is copied, not shared."

The statement "Data passed between the main page and workers is copied, not shared" refers to how data is handled when communicating between the main thread (the main JavaScript execution context in a web page) and web workers (background threads that can run scripts in parallel).

### Explanation

1. **Copying Data**:
   - When you send data from the main thread to a worker using the `postMessage()` method, the data is serialized and copied. This means that the worker receives a separate instance of the data, not a reference to the original data in the main thread.
   - For example, if you send an object or an array from the main thread to a worker, the worker gets its own copy of that object or array. Any changes made to the data in the worker do not affect the original data in the main thread, and vice versa.

2. **No Shared State**:
   - Because data is copied, there is no shared state between the main thread and the worker. This design helps avoid issues related to concurrency, such as race conditions, where multiple threads might try to read and write to the same data simultaneously.
   - Each thread operates independently with its own copy of the data, which simplifies the programming model and reduces the complexity of managing shared state.

3. **Structured Clone Algorithm**:
   - The copying process uses the **structured clone algorithm**, which can handle a variety of data types, including:
     - Primitive types (numbers, strings, booleans, etc.)
     - Objects and arrays
     - Dates, Maps, Sets, and other complex data structures
   - However, not all data types can be copied. For example, functions, DOM nodes, and certain types of objects (like `Window` or `Document`) cannot be transferred.

### Implications

- **Performance**: Copying data can have performance implications, especially for large data structures. If you frequently send large amounts of data between the main thread and workers, it may lead to increased memory usage and slower performance due to the overhead of copying.
  
- **Data Integrity**: Since the data is copied, you can be assured that the main thread and the worker do not interfere with each other's data. This isolation can help prevent bugs related to shared state.

### Example

Here’s a simple example to illustrate this concept:

```javascript
// Main thread
const data = { value: 42 };

const worker = new Worker('worker.js');

// Send data to the worker
worker.postMessage(data);

// In worker.js
self.onmessage = function(event) {
    const receivedData = event.data;
    console.log(receivedData.value); // Outputs: 42

    // Modify the received data
    receivedData.value = 100;
    console.log(receivedData.value); // Outputs: 100
};

// Back in the main thread
console.log(data.value); // Outputs: 42 (original data is unchanged)
```

In this example:
- The `data` object is sent to the worker, and the worker receives a copy of it.
- The worker modifies its copy of the data, but the original `data` object in the main thread remains unchanged.

### Conclusion

The statement emphasizes the design choice in web workers to copy data rather than share it, which simplifies concurrency and helps avoid common pitfalls associated with shared state in multi-threaded programming.

in a nutshell it means. that when we pass a data from main thread to worker and vice versa, they may have the same type and the same value but they are not the same thing since during the transfer that transferring data serializes (converts to string via probably `JSON,strihgify()`) and converts to its real type after transfer probably via `jSON.parse()`, so you can't access that specific variable from the main thread when you're coding in worker and vice versa but you can use it's value, in this case no race condition and other stuff doesn't happen because we have access to values and variables from only one spot and even we transferring them, we're cloning them not sharing them so we can use the value of them in another codes without any concern for bugs may appear to race conditions.

##  what's mutability and immutability in JavaScript?
In JavaScript, mutability and immutability refer to whether or not an object or value can be changed after it has been created.

### Mutability

**Mutability** means that an object or value can be changed after it is created. In JavaScript, most objects and arrays are mutable. This means you can modify their properties or elements without creating a new object or array.

#### Examples of Mutable Structures:

1. **Objects**:
   ```javascript
   const person = { name: 'Alice', age: 30 };
   person.age = 31; // Mutating the object
   console.log(person); // { name: 'Alice', age: 31 }
   ```

2. **Arrays**:
   ```javascript
   const numbers = [1, 2, 3];
   numbers.push(4); // Mutating the array
   console.log(numbers); // [1, 2, 3, 4]
   ```

### Immutability

**Immutability** means that once an object or value is created, it cannot be changed. In JavaScript, primitive values (like numbers, strings, booleans, `null`, `undefined`, and symbols) are immutable. If you want to change a primitive value, you create a new value instead of modifying the existing one.

#### Examples of Immutable Structures:

1. **Primitive Values**:
   ```javascript
   let x = 10;
   x = 20; // This creates a new value; the original value (10) is unchanged
   console.log(x); // 20
   ```

2. **Immutable Data Structures**: While JavaScript does not have built-in immutable data structures, you can create them using libraries like Immutable.js or by using techniques such as object spread syntax or `Object.freeze()`.

   - **Using Object Spread**:
     ```javascript
     const original = { name: 'Alice', age: 30 };
     const updated = { ...original, age: 31 }; // Creates a new object
     console.log(original); // { name: 'Alice', age: 30 }
     console.log(updated); // { name: 'Alice', age: 31 }
     ```

   - **Using `Object.freeze()`**:
     ```javascript
     const person = Object.freeze({ name: 'Alice', age: 30 });
     person.age = 31; // This will not change the object
     console.log(person); // { name: 'Alice', age: 30 }
     ```

### Summary

- **Mutable**: Objects and arrays can be changed after creation. You can modify their properties or elements directly.
- **Immutable**: Primitive values cannot be changed. If you want to "change" a primitive, you create a new value. You can also create immutable objects using techniques or libraries that enforce immutability.

Understanding mutability and immutability is important for managing state in applications, especially in functional programming paradigms and when working with frameworks like React, where immutability can help with performance optimizations and predictable state management.

## race conditions and cloning/sharing variables in modules and workers

in modules variables and values share between the main module and importing one and not cloned (I proved it, I see no reason to elaborate it) but in workers the value or variables clones in main thread or worker while communicating with each other, it means when you transfer `let a=90` with `postmessage(a)` from main thread to another worker, the `event.data` type is a number and its value is 90 but it's not the same `a` we had in main thread and they only look alike but they are not the same thing (I've tested it), the reason the variables and values in modules are the same thing, because it doesn't matter how many JavaScript scripts and modules you have, at the end they're going to run in a single thread, so no race conditions occurs, I couldn't find any reason why variables are read-only in other modules than their original and after asking chat GPT, I realized that the reason that variables are read-only in modules rather than the original module because of the nature of modules, module remain state should remain intact, so it can keep reusability feature while in workers, reusability is not a matter and we only use workers to transfer load from a thread to another one, so making variables in read-only in workers is not possible, still variables can be  re-assigned, the race condition may occur, therefore we have to implement the clone algorithm (clone algorithm is something similar like deep copy which we use `JSON.stringify()` and `JSON.parse()`) to prevent workers from **sharing** variables due to race condition issues.

you can't reassign a variable in modules but you can mutate them like `arr.name="hi"` is possible but
```JavaScript
let arr=[1,2,3];  
arr=90
```
is not, that's because mutating keeps the reference but re-assigning change the reference, in that case when we change the reference or replace it with a primitive value, we have violated and ruined the integrity of our module because that re-assigned variable changes the inherence and nature of our value but mutation doesn't.
## what is race condition in a multi-threaded language like Java? (the concept of race condition applies to any language including multi-threaded and single threaded)

A race condition in a multi-threaded environment, such as Java, occurs when two or more threads access shared data and try to change it at the same time. If the threads are not properly synchronized, the final outcome of the operations can depend on the timing of how the threads are scheduled, leading to unpredictable and erroneous behavior.

### Key Points about Race Conditions:

1. **Shared Resources**: Race conditions typically involve shared resources, such as variables, data structures, or files, that multiple threads can read from and write to.

2. **Timing Dependency**: The outcome of the operations performed by the threads can vary based on the order and timing of their execution. This means that the same program can produce different results in different runs, depending on how the threads are scheduled by the operating system.

3. **Synchronization**: To prevent race conditions, synchronization mechanisms must be used. In Java, this can be achieved using:
   - **Synchronized Methods**: Marking a method with the `synchronized` keyword ensures that only one thread can execute that method on the same object at a time.
   - **Synchronized Blocks**: You can also use synchronized blocks to limit the scope of synchronization to a specific section of code.
   - **Locks**: Java provides explicit lock mechanisms through the `java.util.concurrent.locks` package, allowing for more fine-grained control over synchronization.

4. **Example of a Race Condition**:
   Here’s a simple example to illustrate a race condition:

   ```java
   public class Counter {
       private int count = 0;

       public void increment() {
           count++;
       }

       public int getCount() {
           return count;
       }
   }

   public class RaceConditionExample {
       public static void main(String[] args) throws InterruptedException {
           Counter counter = new Counter();

           Thread t1 = new Thread(() -> {
               for (int i = 0; i < 1000; i++) {
                   counter.increment();
               }
           });

           Thread t2 = new Thread(() -> {
               for (int i = 0; i < 1000; i++) {
                   counter.increment();
               }
           });

           t1.start();
           t2.start();
           t1.join();
           t2.join();

           System.out.println("Final count: " + counter.getCount());
       }
   }
   ```

   In this example, both threads `t1` and `t2` increment the `count` variable. Without synchronization, the final count may not be 2000 as expected, due to race conditions.

5. **Avoiding Race Conditions**: To avoid race conditions in the above example, you can synchronize the `increment` method:

   ```java
   public synchronized void increment() {
       count++;
   }
   ```

By using synchronization, you ensure that only one thread can execute the `increment` method at a time, thus preventing race conditions and ensuring the integrity of the shared data.

## what's `event.ports` in `onconnect` in a shared worker?
In the context of a Shared Worker in JavaScript, `event.ports` refers to the `MessagePort` objects that are used for communication between the Shared Worker and the connected scripts (such as web pages or other workers).

When a Shared Worker is created, it can handle multiple connections from different contexts (like different tabs or iframes). Each time a new connection is made, the `onconnect` event is triggered. The event object passed to the `onconnect` event handler contains a `ports` property, which is an array of `MessagePort` objects.

Here's a brief overview of how it works:

1. **Creating a Shared Worker**: You create a Shared Worker using the `SharedWorker` constructor in your JavaScript code.

2. **Connecting to the Worker**: When a script connects to the Shared Worker, the `onconnect` event is fired in the worker's context.

3. **Handling the Connection**: In the `onconnect` event handler, you can access `event.ports`, which contains the `MessagePort` objects that represent the communication channels for the connected scripts.

4. **Using MessagePort**: You can use the `postMessage` method on the `MessagePort` objects to send messages back and forth between the Shared Worker and the connected scripts. Each `MessagePort` can be used to send messages to the specific context that is connected.

Here’s a simple example:

```javascript
// In the Shared Worker script
self.onconnect = function(event) {
    const port = event.ports[0]; // Get the first MessagePort
    port.onmessage = function(e) {
        console.log('Message received from client:', e.data);
        port.postMessage('Hello from Shared Worker!');
    };
};
```

In this example, when a client connects to the Shared Worker, the `onconnect` event is triggered, and the worker sets up a message handler for the `MessagePort`. When a message is received from the client, it logs the message and sends a response back.

This mechanism allows for efficient communication between multiple contexts and the Shared Worker, enabling shared state and functionality across different parts of an application.

## what's `MessagePort` object in connect event `port` property in a shared worker and what info this `messagePort` object contain?

In the context of a Shared Worker in JavaScript, the `MessagePort` object is a crucial component that facilitates communication between the Shared Worker and the connected scripts (such as web pages or other workers). When a new connection is established to the Shared Worker, the `onconnect` event is triggered, and the `port` property of the event contains a `MessagePort` object.

### Key Characteristics of the `MessagePort` Object:

1. **Communication Channel**: The `MessagePort` serves as a bi-directional communication channel. It allows the Shared Worker to send messages to the connected context and vice versa.

2. **Event Handling**: The `MessagePort` object has an `onmessage` event handler that you can set up to listen for incoming messages. When a message is received, the event handler is triggered, and you can access the message data through the event object.

3. **Sending Messages**: You can use the `postMessage` method of the `MessagePort` to send messages to the connected context. This method takes a single argument, which is the data you want to send.

4. **Transferable Objects**: The `MessagePort` can also be used to transfer ownership of certain types of objects (like `ArrayBuffer`, `ImageBitmap`, etc.) between contexts, which can improve performance by avoiding unnecessary copying of data.

5. **Port State**: The `MessagePort` has a `start()` method that you must call to begin communication. Until you call `start()`, the port is in a "closed" state and cannot send or receive messages.

6. **Close Method**: The `MessagePort` object has a `close()` method that can be called to close the port, which will prevent any further communication through that port.

### Information Contained in the `MessagePort` Object:

The `MessagePort` object itself does not contain a lot of properties or methods that expose internal state or information. Instead, it provides a simple interface for communication. Here are the main methods and properties associated with a `MessagePort`:

- **Methods**:
  - `postMessage(message)`: Sends a message to the connected context.
  - `start()`: Starts the port, allowing it to send and receive messages.
  - `close()`: Closes the port, preventing further communication.

- **Properties**:
  - `onmessage`: An event handler that is called when a message is received on the port.
  - `onmessageerror`: An event handler that is called when an error occurs while receiving a message.

### Example Usage:

Here’s a simple example to illustrate how a `MessagePort` is used in a Shared Worker:

**Shared Worker Script (shared-worker.js)**:
```javascript
self.onconnect = function(event) {
    const port = event.ports[0]; // Get the MessagePort from the event
    port.onmessage = function(e) {
        console.log('Message received from client:', e.data);
        // Respond back to the client
        port.postMessage('Hello from Shared Worker!');
    };
};
```

**Client Script (client.js)**:
```javascript
const worker = new SharedWorker('shared-worker.js');

// Get the MessagePort from the worker
worker.port.start(); // Start the port to begin communication

worker.port.onmessage = function(e) {
    console.log('Message received from Shared Worker:', e.data);
};

// Send a message to the Shared Worker
worker.port.postMessage('Hello from client!');
```

### Summary:

The `MessagePort` object in a Shared Worker is a communication channel that allows for sending and receiving messages between the worker and connected contexts. It provides methods for message handling and state management, enabling efficient communication in a multi-context environment.

## what do we mean by "channel" when we say "The `MessagePort` object in a Shared Worker is a communication channel"?

When we refer to the term "channel" in the context of the `MessagePort` object in a Shared Worker, we are describing a pathway or medium through which data (messages) can be transmitted between different contexts (such as web pages, iframes, or other workers) and the Shared Worker itself. Here’s a breakdown of what this means:

### 1. **Bi-Directional Communication**:
   - A "channel" implies that communication can flow in both directions. The `MessagePort` allows the Shared Worker to send messages to the connected context and also enables the connected context to send messages back to the Shared Worker. This two-way communication is essential for interactive applications.

### 2. **Message Transmission**:
   - The `MessagePort` acts as a conduit for messages. When you use the `postMessage` method on a `MessagePort`, you are sending data through this channel. The receiving end (either the worker or the connected context) listens for incoming messages via the `onmessage` event handler, effectively receiving data sent through the channel.

### 3. **Isolation**:
   - Each `MessagePort` represents a separate communication channel. This means that messages sent through one `MessagePort` do not interfere with messages sent through another. This isolation is important in scenarios where multiple contexts are connected to the same Shared Worker, as it allows each context to communicate independently without mixing messages.

### 4. **Concurrency**:
   - The concept of a channel also implies that multiple connections can exist simultaneously. Each connection to the Shared Worker gets its own `MessagePort`, allowing multiple clients to communicate with the worker at the same time without blocking each other.

### 5. **Event-Driven Model**:
   - The communication channel operates on an event-driven model. When a message is sent through the channel, it triggers an event (`onmessage`) on the receiving end. This allows for asynchronous communication, where the sender and receiver do not need to be synchronized in their operations.

### Summary:
In summary, when we refer to the `MessagePort` as a "communication channel," we are emphasizing its role as a dedicated pathway for sending and receiving messages between the Shared Worker and connected contexts. This channel facilitates bi-directional, isolated, and concurrent communication, enabling efficient interaction in web applications that utilize Shared Workers.

## consider I want to implement multiplication of two numbers, I want to have this multiplication process code as  a web worker in JavaScript, two different scripts are going to use this web worker, if I declare this multiplication process as dedicated web worker in both of my scripts, what's the difference with defining as shared web worker?

Great question! Let's break down the differences between using a **Dedicated Web Worker** vs. a **Shared Web Worker** for your multiplication example, where **two different scripts** (e.g., two tabs or windows) want to use the same multiplication logic.

---

### **Scenario: Multiplication in a Web Worker**
You want to offload multiplication of two numbers to a Web Worker, and **two separate scripts** (e.g., `script1.js` and `script2.js`) will use this worker.

---

### **Option 1: Dedicated Web Worker (Two Separate Workers)**
If you define the multiplication logic in a **Dedicated Web Worker**, **each script will create its own independent worker instance**:

#### **worker.js (Dedicated Worker)**
```javascript
// worker.js (Dedicated Worker)
onmessage = function(e) {
  const { a, b } = e.data;
  const result = a * b;
  postMessage(result);
};
```

#### **script1.js & script2.js (Each Creates Its Own Worker)**
```javascript
// script1.js
const worker1 = new Worker('worker.js');
worker1.postMessage({ a: 5, b: 3 });
worker1.onmessage = (e) => console.log('Result (Script 1):', e.data);

// script2.js
const worker2 = new Worker('worker.js');
worker2.postMessage({ a: 10, b: 4 });
worker2.onmessage = (e) => console.log('Result (Script 2):', e.data);
```

#### **Key Implications**
✅ **Isolation**: Each script has its own worker instance.  
✅ **Simple Communication**: Direct `postMessage` without port management.  
❌ **No Shared State**: The two workers are **completely independent**.  
❌ **Redundant Memory Usage**: Two instances of the same worker logic.  

---

### **Option 2: Shared Web Worker (Single Worker Shared Across Scripts)**
If you define the multiplication logic in a **Shared Web Worker**, **both scripts can connect to the same worker instance**:

#### **shared-worker.js (Shared Worker)**
```javascript
// shared-worker.js
onconnect = function(e) {
  const port = e.ports[0];
  port.onmessage = function(event) {
    const { a, b } = event.data;
    const result = a * b;
    port.postMessage(result);
  };
};
```

#### **script1.js & script2.js (Both Connect to the Same Worker)**
```javascript
// script1.js
const worker1 = new SharedWorker('shared-worker.js');
worker1.port.start(); // Required!
worker1.port.postMessage({ a: 5, b: 3 });
worker1.port.onmessage = (e) => console.log('Result (Script 1):', e.data);

// script2.js
const worker2 = new SharedWorker('shared-worker.js');
worker2.port.start(); // Required!
worker2.port.postMessage({ a: 10, b: 4 });
worker2.port.onmessage = (e) => console.log('Result (Script 2):', e.data);
```

#### **Key Implications**
✅ **Single Instance**: Both scripts use the **same worker**, reducing memory overhead.  
✅ **Shared State (if needed)**: You could maintain shared data inside the worker.  
❌ **More Complex**: Requires `port`-based communication.  
❌ **Browser Support**: Not supported in Safari (as of 2024).  

---

### **Key Differences Summary**
| Feature              | Dedicated Web Worker (Two Workers) | Shared Web Worker (One Worker)         |
| -------------------- | ---------------------------------- | -------------------------------------- |
| **Worker Instances** | 2 (one per script)                 | 1 (shared)                             |
| **Memory Usage**     | Higher (duplicate workers)         | Lower (single worker)                  |
| **Communication**    | Direct (`postMessage`)             | Port-based (`worker.port.postMessage`) |
| **Shared State**     | No (isolated)                      | Yes (if needed)                        |
| **Browser Support**  | All modern browsers                | Not in Safari                          |

---

### **Which One Should You Choose?**
- **Use Dedicated Workers** if:  
  - Each script needs **isolated computation**.  
  - You don’t care about memory duplication.  
  - You need **maximum browser compatibility**.  

- **Use a Shared Worker** if:  
  - You want **a single instance** handling requests from multiple scripts.  
  - You might later need **shared state** (e.g., caching results).  
  - You can **ignore Safari support**.  

---

### **Final Thoughts**
For **simple multiplication**, a **Dedicated Worker** is easier and works everywhere.  
But if you later want to **extend functionality** (e.g., cache results, share data between tabs), a **Shared Worker** becomes useful.  

## what's `onconnect` event role in a shared web worker?

In a **Shared Web Worker**, the `onconnect` event plays a crucial role in managing connections from multiple browsing contexts (like tabs, iframes, or windows). Here's how it works:

### **Role of `onconnect` in a Shared Web Worker**

1. **Handles New Connections**
    
    - When a new script (from a tab, window, or iframe) connects to the Shared Web Worker using `new SharedWorker()`, the `onconnect` event is triggered in the worker.
        
    - The worker can then set up communication with the new client.
        
2. **Provides a `MessagePort` for Communication**
    
    - The event object (`ConnectEvent`) contains a `ports` array, which includes a [`MessagePort`](https://developer.mozilla.org/en-US/docs/Web/API/MessagePort) for communication.
        
    - The worker uses this port to send and receive messages from the connected context.
        
3. **Allows Multi-Context Communication**
    
    - Unlike a **Dedicated Worker** (which serves only one context), a **Shared Worker** can handle multiple connections, enabling cross-tab/window communication.
        

### **Example Code**

#### **Shared Worker (worker.js)**

```javascript
onconnect = function(e) {
  const port = e.ports[0]; // Get the communication port

  port.onmessage = function(event) {
    console.log("Message from client:", event.data);
    port.postMessage("Worker replies: " + event.data);
  };

  port.start(); // Required to begin listening for messages
};
```


#### **Client Script (app.js)**

```javascript
const worker = new SharedWorker("worker.js");

worker.port.onmessage = function(event) {
  console.log("Received from worker:", event.data);
};

worker.port.postMessage("Hello Worker!");
```
### **Key Points**

- `onconnect` is **exclusive to Shared Workers** (Dedicated Workers use `onmessage` directly).
    
- Each new connection triggers `onconnect`, allowing the worker to manage multiple clients.
    
- The `ports` array in the event contains the `MessagePort` for bidirectional communication.
    
- You must call `port.start()` if you set up `onmessage` manually (some browsers do this automatically).
    

### **Use Cases**

- **Cross-tab communication** (e.g., syncing state between browser tabs).
    
- **Shared caching** (multiple pages using the same worker for cached data).
    
- **Centralized background tasks** (like WebSocket management).
    

## why we can only have one `messagePort` object in `onconnect` event port array at once?

In a **Shared Web Worker**, the `onconnect` event's `ports` array typically contains **only one `MessagePort`** per connection, even though it's technically an array. This design choice stems from several key reasons:

---

### **1. Single Port Per Connection is Sufficient**

- A single `MessagePort` allows **full bidirectional communication** between the worker and the client (tab/iframe/window).
    
- Since `postMessage` and `onmessage` work bidirectionally on the same port, there’s no need for additional ports for basic communication.
    

---

### **2. Historical and Spec-Driven Design**

- The `onconnect` event inherits from the **`MessageEvent`** interface, where `ports` is an array (for consistency with other APIs like `postMessage`).
    
- In other contexts (e.g., `postMessage` with `transferrables`), you _can_ transfer multiple ports, but `SharedWorker` connections are intentionally limited to **one port per client** for simplicity.
    

---

### **3. Security and Isolation**

- If multiple ports were allowed per connection:
    
    - **Complexity increases**: The worker would need to manage multiple channels per client.
        
    - **Risk of leaks**: Accidental port duplication could lead to unintended message broadcasts or memory issues.
        
- By restricting it to one port, the API ensures:
    
    - Clear 1:1 communication between the worker and each client.
        
    - No cross-talk between ports of the same client.
        

---

### **4. Future Extensibility (Array Reserved for Potential Use)**

- The `ports` array remains for **forward compatibility**.
    
- Future specs _could_ introduce multi-port connections (e.g., for prioritized channels), but currently, only `ports[0]` is used.
    

---

### **Example: Why One Port is Enough**

#### **Shared Worker (`worker.js`)**

```javascript
onconnect = (e) => {
  const port = e.ports[0]; // Only one port ever exists here.
  port.onmessage = (event) => {
    console.log("Client says:", event.data);
    port.postMessage("Worker replies!"); // Bidirectional on the same port.
  };
  port.start(); // Required to begin listening.
};
```
#### **Client (`app.js`)**

```javascript
const worker = new SharedWorker("worker.js");
worker.port.postMessage("Hello!"); // Uses the single assigned port.
worker.port.onmessage = (e) => console.log(e.data);
```
---

### **Key Takeaways**

1. **Simplicity**: One port per client keeps the API clean and easy to use.
    
2. **Consistency**: Matches the `MessageEvent` pattern (even if only one port is used).
    
3. **Security**: Prevents accidental complexity or leaks.
    
4. **Bidirectional**: A single `MessagePort` supports two-way messaging, eliminating the need for more.

If you need **multi-channel communication**, you can simulate it by sending structured messages (e.g., `{ type: "channelA", data: ... }`) over the single port. 🚀

## I have two JavaScript scripts that need to use a same web worker, if I declare that web worker as dedicated web worker in each of those JavaScript, do 4 threads will be occupied ( 2 for scripts and 2 for each time that dedicated web worker invokes), and if I declare this web worker as shared web worker, do only 3 threads gets used? (2 for JavaScript scripts and 1 for shared web worker)

### **Thread Usage: Dedicated vs. Shared Web Workers**

Your understanding is **mostly correct**, but let's clarify how threads are allocated in both scenarios.

---

## **Case 1: Dedicated Web Workers (2 Separate Workers)**

- **Each `DedicatedWorker` runs in its own thread.**
    
- If two scripts (e.g., from different tabs or iframes) create their own instances of the **same worker file**, they **do not share the worker**.
    
- **Thread allocation:**
    
    - **Main Thread (UI Thread)** → Runs the JavaScript of each tab (`script1.js`, `script2.js`).
        
    - **Worker Thread 1** → Dedicated to `script1.js`'s worker.
        
    - **Worker Thread 2** → Dedicated to `script2.js`'s worker.
        

✅ **Total Threads Used = 3** (1 main thread + 2 worker threads).  
_(Not 4, since the main thread is shared by both scripts but serialized per tab.)_

#### **Why Not 4 Threads?**

- The **main thread** is shared (but each tab runs its own instance of the script sequentially).
    
- Each `DedicatedWorker` spawns **one new background thread**.
    

---

## **Case 2: Shared Web Worker (1 Shared Worker)**

- **A `SharedWorker` allows multiple scripts to connect to the same worker instance.**
    
- **Thread allocation:**
    
    - **Main Thread (UI Thread)** → Runs `script1.js` and `script2.js`.
        
    - **Shared Worker Thread** → Only **one thread** for the worker, shared by both scripts.
        

✅ **Total Threads Used = 2** (1 main thread + 1 shared worker thread).

_(If you had 3 scripts connecting to the same `SharedWorker`, it would still use only **2 threads**.)_

---

### **Key Takeaways**

| Scenario            | Main Thread | Worker Threads   | Total Threads |
| ------------------- | ----------- | ---------------- | ------------- |
| 2 Dedicated Workers | 1 (shared)  | 2 (1 per worker) | 3             |
| 1 Shared Worker     | 1 (shared)  | 1 (shared)       | 2             |

- **Shared Workers are more efficient** when multiple scripts need the same background task.
    
- **Dedicated Workers are isolated**, so they use more threads (but are simpler to manage).
    

### **Threading Behavior in Browsers**

- Browsers **do not guarantee true parallelism** (due to CPU core limits and optimizations).
    
- JavaScript is **single-threaded per context**, but workers run in **separate threads**.
    
- A `SharedWorker` **reduces thread duplication** compared to multiple `DedicatedWorkers`.
    
## when we use web workers i.e. threads to implement our tasks, what computer component usage increases? CPU, RAM or any other component?

When you use **Web Workers** (threads) in JavaScript, several **computer hardware components** experience increased usage, primarily:

### **1. CPU (Processor) Usage Increases**

- **Why?**
    
    - Each Web Worker runs in a **separate thread**, allowing parallel computation.
        
    - If workers perform heavy calculations, **multiple CPU cores** may be engaged (if available).
        
- **Impact:**
    
    - High CPU usage if workers run intensive tasks (e.g., data processing, simulations).
        
    - Better utilization of multi-core CPUs (compared to single-threaded JS).
        

### **2. RAM (Memory) Usage Increases**

- **Why?**
    
    - Each worker has **its own memory space** (isolated from the main thread).
        
    - Data passed between threads via `postMessage` is **copied** (not shared), increasing memory consumption.
        
- **Impact:**
    
    - More workers = more memory overhead.
        
    - Large data transfers (e.g., big arrays) can spike RAM usage.
        

### **3. GPU Usage (Indirectly Affected)**

- **Why?**
    
    - Workers **do not directly use the GPU**, but:
        
        - If workers offload rendering tasks (e.g., WebGL calculations), the GPU may be used more.
            
        - Some WASM-based workers (e.g., with WebGPU) can utilize GPU acceleration.
            
- **Impact:**
    
    - Depends on the task (e.g., image/video processing may engage GPU).
        

### **4. Disk I/O (If Workers Access Files)**

- **Why?**
    
    - Workers can fetch files (`fetch()`, `FileReader`), increasing disk activity.
        
    - Service Workers (a type of Web Worker) cache data, leading to disk reads/writes.
        
- **Impact:**
    
    - More disk usage if workers handle file operations.
        

### **5. Network Usage (If Workers Make API Calls)**

- **Why?**
    
    - Workers can run **background network requests** (e.g., polling APIs, WebSockets).
        
- **Impact:**
    
    - Increased bandwidth consumption if workers frequently fetch data.
        

---

### **Summary: What Hardware is Impacted?**

| Component   | Usage Increase? | Reason                                        |
| ----------- | --------------- | --------------------------------------------- |
| **CPU**     | ✅ Yes (Major)   | Parallel threads use multiple cores.          |
| **RAM**     | ✅ Yes (Major)   | Each worker has its own memory space.         |
| **GPU**     | ⚠️ Sometimes    | Only if workers handle rendering/WASM/WebGPU. |
| **Disk**    | ⚠️ Sometimes    | If workers read/write files or cache data.    |
| **Network** | ⚠️ Sometimes    | If workers make API calls or sync data.       |

---

### **Optimization Tips**

1. **Avoid excessive workers** (too many threads waste memory).
    
2. **Use `Transferable Objects`** (for large data to avoid copying).
    
3. **Limit heavy computations** if targeting low-end devices.
    
4. **Monitor performance** with `performance.memory` and DevTools.

## what's the difference of using `self` keyword before `onmessage` method in JavaScript web worker and not using it?

In JavaScript Web Workers, the `self` keyword refers to the global scope of the worker (similar to `window` in the main thread). When defining the `onmessage` handler, there are two common ways to do it:

### 1. **Using `self.onmessage`**
   ```javascript
   self.onmessage = function(event) {
       console.log("Message received:", event.data);
   };
   ```
   - `self` explicitly refers to the worker's global scope.
   - This is useful for clarity, especially in nested contexts where `this` might not refer to the global scope.

### 2. **Using `onmessage` directly (without `self`)**
   ```javascript
   onmessage = function(event) {
       console.log("Message received:", event.data);
   };
   ```
   - Since `onmessage` is a property of the worker's global scope, you can omit `self` (it implicitly refers to `self.onmessage`).
   - This works because the worker's top-level scope is the global scope (`self`).

### **Key Differences**
| Approach         | Behavior                                                | Clarity                          | Potential Issues                                                 |
| ---------------- | ------------------------------------------------------- | -------------------------------- | ---------------------------------------------------------------- |
| `self.onmessage` | Explicitly sets the handler on the global worker scope. | More explicit, avoids ambiguity. | Slightly more verbose.                                           |
| `onmessage`      | Implicitly sets the handler on the global scope.        | Shorter, but less explicit.      | Could be ambiguous if `onmessage` is shadowed in a nested scope. |

### **Which One Should You Use?**
- If you're working in a simple worker script, both are functionally equivalent.
- If your worker code has nested functions or modules, using `self.onmessage` is safer to avoid scope-related issues.
- Some developers prefer `self.onmessage` for consistency with other worker APIs like `self.postMessage()`.

### Example with `addEventListener` (Alternative Approach)
Instead of assigning to `onmessage`, you can also use:
```javascript
self.addEventListener('message', function(event) {
    console.log("Message received:", event.data);
});
```
This is more flexible (allows multiple listeners) and is often preferred in modern code.

### Conclusion
There's no functional difference in simple cases, but `self.onmessage` is more explicit and avoids potential scope issues. If you're writing modular or complex worker code, `self.onmessage` is a safer choice.

## what is shared web workers in JavaScript (the correct one not the ambiguous and incorrect one)

imagine you have two scripts that want to perform same operation in the background i.e. web workers, lets imagine this background operation is multiplication of two numbers, if you want to declare a dedicated web worker for each of these scripts, 2 threads will be occupied for each of the scripts (if we run them in separate live servers by running multiple VS code apps) and 2 threads are required for each web worker, but if we declare these web workers as shared web worker, 2 threads will be occupied because of the scripts and only one thread will be occupied because of the shared web worker, the word `shared` in `shared web worker` term refers to that threads that gets shared by the worker unlike the dedicated worker that each time the app reached the `new Worker()` code, the code allocates a thread to that dedicated web worker but everything is different for shared web worker which is explained below based on [stackoverflow reference](https://stackoverflow.com/questions/6778360/whats-the-difference-between-shared-worker-and-worker-in-html5#answer-62487272):

>Shared worker allow all front page context script, which call constructor:                                  `new SharedWorker("path-to-shared-worker-file.js")` to share the same instance of shared worker file running in the background context(another thread of running JavaScript in the back).`
for example, when webpage #1 calling that constructor, if found there is no shared worker loaded up in the back yet, it will cause the background context to download the file and load it up, then later when webpage #2 calling that same constructor(same file path), it found there is an existing shared worker running, it will just using the same one. When `worker.port.start()` function invoked, it will cause shared worker file `onconnect` event handler invoked to register caller and obtain the handle to communicate the client port(for `postMessage` back for example).
However worker, every webpage above will load up one worker file in the background for every single front page, which is not shared the same worker.js instance.

so basically the code execution and everything is same between shared web workers and dedicated web workers, but for the scripts which want to perform the same process and task in their workers, we have to use shared web workers which helps to save resources in our CPU and RAM.

you can't expect shared web worker to have access the other script data and shared state that AI tells you which shared web workers can provide, is a myth (all of those pushing `message objects` from different connection into an array is non-sense), as we said above, every process in shared web worker is like dedicated web worker.

shared web worker doesn't work properly in all of the browsers, in chrome, sent messages to shared workers from scripts won't be displayed, but in Mozilla Firefox, everything is fine ( but be careful, there is still a chance for any error and malfunction)

please use `onmessage` for using `message`  event in shared web workers and ***DO NOT USE `addEventListener()` for using `message` event in shared web workers*** because if you use  `addEventListener` you have to use `start()` method to make the communication active which using this `start()` makes everything convoluted.

in a nutshell for better performance, when you want to offload a same task from multiple scripts, you better you put that heavy task code inside a shared web worker and not a dedicated web worker but if you have scripts which they need to offload different task (not same) you should use dedicated web workers.

## what happens if the scripts which want to access to shared worker, are not from the same origin?

### **Cross-Origin Restrictions for Shared Workers**
If scripts from different origins (domains, protocols, or ports) try to access a **`SharedWorker`**, they will **fail due to the browser's Same-Origin Policy (SOP)**. This is a security measure to prevent malicious websites from interacting with workers running in another origin's context.

---

### **Key Behaviors & Errors**
1. **`SecurityError` is thrown**  
   - If a script from `https://example.com` tries to access a `SharedWorker` created by `https://another-site.com`, the browser blocks it with:
     ```
     Uncaught DOMException: Failed to construct 'SharedWorker':
     Script at 'https://another-site.com/worker.js' cannot be accessed from origin 'https://example.com'.
     ```

2. **Worker script must be same-origin**  
   - The `SharedWorker` script (`worker.js`) must be served from the **same origin** as the page trying to use it.  
   - Example:
     - ✅ **Allowed**: `https://example.com/page.html` → `https://example.com/worker.js`  
     - ❌ **Blocked**: `https://example.com/page.html` → `https://other.com/worker.js`

3. **No CORS headers can bypass this**  
   - Unlike regular fetch/XHR requests (where CORS headers like `Access-Control-Allow-Origin` can relax restrictions), `SharedWorker` **does not support CORS**.  
   - Even if `worker.js` sends permissive CORS headers, the browser will still block cross-origin access.

---

### **Workarounds (If You Control Both Origins)**
If you need cross-origin communication, consider:
1. **`postMessage` + `iframe`**  
   - Use `window.postMessage` to communicate between windows/iframes from different origins (with proper origin checks).

2. **Proxy via the Backend**  
   - Have your server relay messages between clients (e.g., via WebSockets or HTTP requests).

3. **Service Workers (for limited cases)**  
   - Service Workers can sometimes act as a proxy, but they also follow strict origin restrictions.

---

### **Key Takeaways**
- **`SharedWorker` is strictly same-origin.**  
- **No CORS support** for worker scripts.  
- **Alternatives** like `postMessage` or backend proxying are needed for cross-origin communication.  

## does shared web worker, work in a JavaScript file (linked to html via script tag) when we open that html file as local file?

### **Do Shared Web Workers Work with Local Files (`file://` Protocol)?**  
**Short answer:** **No**, Shared Workers (and often even Dedicated Workers) **fail** when used in HTML files opened locally (`file://`) due to browser security restrictions.  

---

### **Why Doesn’t It Work?**
1. **Same-Origin Policy (SOP) Restrictions**  
   - Browsers treat each `file://` path as a **separate origin**.  
   - Example:  
     - `file:///C:/project/page1.html` and `file:///C:/project/page2.html` are considered **different origins** (even in the same folder).  
     - Thus, they **cannot** share a `SharedWorker`.  

2. **Security Restrictions on `file://`**  
   - Most browsers (Chrome, Firefox, Edge) **block Web Workers** entirely when running from `file://` for security reasons.  
   - You’ll typically see errors like:  
     ```
     Uncaught DOMException: Failed to construct 'SharedWorker':
     The script has an unsupported MIME type ('') when running locally.
     ```
     (This happens because the browser refuses to load worker scripts from local files.)

---
### **Testing Shared Workers Locally**
If you try this:
```html
<!-- page1.html -->
<script>
  const worker = new SharedWorker('worker.js');
  worker.port.start();
</script>
```
```javascript
// worker.js
onconnect = (e) => {
  const port = e.ports[0];
  port.postMessage("Connected!");
};
```
**Result:**  
- **Chrome/Firefox/Edge:** ❌ Fails with security errors.  
- **Safari:** Sometimes allows Dedicated Workers but blocks Shared Workers.  

---
### **How to Make It Work?**
To test `SharedWorker` properly, you must:  
1. **Use a Local HTTP Server**  
   - Run a server (e.g., `http-server`, `live-server`, Python `http.server`) so the pages are served under `http://localhost` (same origin).  
   - Example (Python 3):  
     ```sh
     python -m http.server 8000
     ```
     Then access `http://localhost:8000/page1.html`.  

2. **Test in a Browser with Relaxed Security (Not Recommended for Production)**  
   - **Chrome** can be launched with `--allow-file-access-from-files` (deprecated and unsafe).  
   - **Firefox** may allow Dedicated Workers but still blocks Shared Workers.  
---

### **Key Takeaways**
- **Shared Workers do not work with `file://`** due to strict browser security policies.  
- **Use `http://localhost`** (via a local server) for proper testing.  
- **Avoid disabling browser security flags** (unsafe for real usage).  

in a nutshell opening html files that links to a JavaScript file containing web workers (either shared or dedicated) via local file, is a bad practice.

## why it takes time for `onconnct` event in shared worker to establish?

The `onconnect` event in a Shared Worker can take time to establish for several reasons:

1. Script Execution Time: The code within the Shared Worker needs to be executed before it can handle connections. If there are any synchronous operations or heavy computations in the worker's initialization code, this can delay the `onconnect` event.

## why The code within the Shared Worker needs to be executed before it can handle connections?

In a Shared Worker environment, the code within the worker needs to be executed before it can handle connections for several reasons:

1. Concurrency Management: Shared Workers are designed to handle multiple connections from different scripts running in different browsing contexts (like tabs or iframes). The worker needs to manage these connections effectively, which requires that its internal logic is fully loaded and operational before any connection attempts are made.

## multiple `onconnect`, `onmessage` and `postMessage`
when we have multiple `onconnect` in our shared web worker, always the one comes last has priority, for example one of the `onconnect` is in line 47 and other one is in line  69, the one in line 69 has priority and one in line 47 gets ignored, same rule applies to `onmessage`, and for `postMessage()` you can send multiple messages and all of them get sent, so there is no problem for multiple postMessages.

## event listener function parameter

in `addEventListener()` when we have code like this

```javascript
lome.addEventListener("click",(e /*or event*/)=>console.log("hi");
```

 the `e` or `event` parameter we have in the `addEventListener` call back function, can be anything i.e. it can be `what` or `peter` instead of `e`, this parameter gives information about our specific event e.g. in `connect` event, you can have access to communication via `ports` property of event, or in `message` event, you can access the message sent from/ to main thread via data property of the event like `event.data`, (these two examples was for web workers.)

## I have two `onconnect` events in my shared worker, why the first `onconnect` gets ignored?

In a Shared Worker, the `onconnect` event is triggered whenever a new connection is made to the worker. If you have multiple `onconnect` event handlers defined, only the last one will be executed because each assignment to `onconnect` overwrites the previous one.

Here’s a brief explanation of how to handle multiple connections properly:

1. Single Event Handler: You should define a single `onconnect` handler that can manage multiple connections. Inside this handler, you can differentiate between different connections and handle them accordingly.

If you're experiencing issues where it seems like the first connection is ignored, ensure that you're not overwriting your `onconnect` handler and that you're correctly managing each connection within that single handler.

## I have two `onmessage` events in my shared worker, why the first `onmessage` gets ignored?

n a Shared Worker, the onmessage event handler is designed to handle messages sent from multiple clients (e.g., different tabs or windows) that connect to the same worker. If you have two onmessage event handlers defined in your Shared Worker, only one of them will be active at a time, and the other will be ignored. This is because the onmessage property can only hold a single function reference.

Here are some common reasons why your first onmessage might seem to get ignored:

1. Overwriting the Handler: If you define onmessage twice, the second definition will overwrite the first one.

## what's the difference between using click event in addeventlistener and as onclick in javascript file or onclick in html as inline?

In JavaScript, there are several ways to handle click events on elements, and each method has its own characteristics and use cases. Here’s a breakdown of the differences between using `addEventListener`, the `onclick` property in a JavaScript file, and inline `onclick` attributes in HTML:



1. Using `addEventListener()`:

```javascript
const button = document.getElementById('myButton');
button.addEventListener('click', function() {
    console.log('Button clicked!');
});
```

Advantages:
- Multiple Handlers: You can attach multiple event listeners to the same element for the same event type without overwriting existing ones.
- Event Options: You can specify options like capture, once, and passive.
- Separation of Concerns: Keeps JavaScript separate from HTML, promoting cleaner code and better maintainability.
- Dynamic Binding: You can add or remove event listeners dynamically at runtime.

Disadvantages:
- Slightly more verbose than inline handlers.

2. Using the `onclick` Property in a JavaScript File

```javascript

const button = document.getElementById('myButton');
button.onclick = function() {
    console.log('Button clicked!');
};
```

Advantages:
- Simple syntax for adding a single click handler.
- Keeps JavaScript separate from HTML.

Disadvantages:
- Single Handler Limitation: If you assign a new function to `onclick`, it will overwrite any existing handler. Only one handler can be assigned at a time.
- Less flexibility compared to `addEventListener`.

3. Using Inline `onclick` in HTML:

```html
<button id="myButton" onclick="console.log('Button clicked!')">Click me</button>
```

Advantages:
- Very straightforward for simple cases; easy to understand at a glance.
- No need to wait for DOM content to load since the handler is defined directly in the HTML.

Disadvantages:
- Mixing Concerns: It mixes HTML with JavaScript, which can lead to less maintainable code.
- Harder to manage if you have many event handlers or complex logic; it can clutter your HTML.
- Limited debugging capabilities compared to external scripts (e.g., you can't easily set breakpoints).
  
Summary

1. Use addEventListener when you need flexibility (multiple handlers, options) and want clean separation of concerns.
2. Use the onclick property when you only need one handler and prefer simplicity without mixing with HTML.
3. Use inline onclick attributes for very simple cases or quick prototypes but avoid them in production code due to maintainability issues.

Choosing between these methods often depends on your specific use case, coding style preferences, and project requirements.

## can we only use `onclick` event as inline in our HTML code?

No, the onclick event is not the only event that can be used inline in HTML. While onclick is one of the most commonly used events for handling click actions, there are many other events that can also be specified inline. Here are some examples of other events that can be used inline:

1. Mouse Events:
   - `onmouseover`: Triggered when the mouse pointer moves over an element.
   - `onmouseout`: Triggered when the mouse pointer moves out of an element.
   - `onmousedown`: Triggered when a mouse button is pressed down on an element.
   - `onmouseup`: Triggered when a mouse button is released over an element.

2. Keyboard Events:
   - `onkeydown`: Triggered when a key is pressed down.
   - `onkeyup`: Triggered when a key is released.
   - `onkeypress`: Triggered when a key is pressed (deprecated in favor of keydown and keyup).

3. Form Events:
   - `onsubmit`: Triggered when a form is submitted.
   - `onchange`: Triggered when the value of an input changes.
   - `onfocus`: Triggered when an input gains focus.
   - `onblur`: Triggered when an input loses focus.

4. Window Events:
   - `onload`: Triggered when the page has finished loading.
   - `onresize`: Triggered when the window is resized.

5. Touch Events (for mobile devices):
   - `ontouchstart`, `ontouchmove`, and `ontouchend`.

Example of Inline Event Handlers

Here’s how you might use some of these events inline in HTML:

```HTML
<button onclick="alert('Button clicked!')">Click Me</button>
<input type="text" onfocus="this.style.backgroundColor='yellow'" onblur="this.style.backgroundColor='white'">
<div onmouseover="this.style.color='red'" onmouseout="this.style.color='black'">Hover over me!</div>
```

Best Practices

While using inline event handlers can be convenient for small scripts or quick prototypes, it’s generally recommended to separate JavaScript from HTML for better maintainability and readability. This can be done by adding event listeners using JavaScript:

```HTML
<button id="myButton">Click Me</button>

<script>
  document.getElementById('myButton').onclick = function() {
    alert('Button clicked!');
  };
</script>```

This approach keeps your HTML clean and separates concerns, making your code easier to manage and debug.

## can we use all the javascript event as inline in our HTML code?

Yes, you can use JavaScript events inline in your HTML code by adding event attributes directly to HTML elements. This approach allows you to specify JavaScript code that should run when a particular event occurs on that element. Here are some common examples of inline event handling:

Example of Inline Event Handling

<!DOCTYPE html>
```HTML
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inline Event Handling</title>
</head>
<body>

    <button onclick="alert('Button clicked!')">Click Me</button>

    <input type="text" onfocus="this.style.backgroundColor='yellow'" onblur="this.style.backgroundColor='white'">

    <a href="#" onmouseover="this.style.color='red'" onmouseout="this.style.color='blue'">Hover over me!</a>

</body>
</html>
```

Common Inline Event Attributes

Here are some common JavaScript events that can be used inline:

- `onclick`: Triggered when an element is clicked.
- `onmouseover`: Triggered when the mouse pointer moves over an element.
- `onmouseout`: Triggered when the mouse pointer moves out of an element.
- `onfocus`: Triggered when an element gains focus (e.g., input fields).
- `onblur`: Triggered when an element loses focus.
- `onchange`: Triggered when the value of an input changes.
- `onsubmit`: Triggered when a form is submitted.

## In the context of web workers, the distinction between dedicated workers and shared workers is crucial for understanding how communication works?

Dedicated Workers
- Dedicated Workers are tied to a single script and can communicate directly with the main thread that created them. The communication happens through the `postMessage` method, which allows messages to be sent back and forth without needing to manage any ports.
- Since there is a one-to-one relationship between the main thread and a dedicated worker, there's no need for additional complexity in managing connections. The main thread can simply send messages directly to the worker, and the worker can respond back using `postMessage()`.

Shared Workers
- Shared Workers, on the other hand, can be accessed by multiple scripts (from different windows or tabs) simultaneously. This introduces a need for more complex communication management because multiple clients may be sending messages to the same worker.
- To handle this complexity, Shared Workers use `event.ports`. When a shared worker is instantiated, it receives an event object that contains `event.ports`, which are `MessagePort` objects that allow for direct communication channels between the worker and each client.
- Each client that connects to a shared worker gets its own port (or ports), allowing them to communicate independently with the worker without interfering with each other. This way, messages from different clients can be managed separately.

Summary
- Dedicated Worker: Simple one-to-one communication; no need for ports since there's only one sender (the main thread) and one receiver (the dedicated worker).
- Shared Worker: More complex many-to-one communication; requires ports to manage multiple clients communicating with a single shared instance of the worker.

Using `event.ports` in shared workers ensures that each client has its own channel for sending and receiving messages, maintaining clear separation of communications among potentially many clients interacting with the same shared resource.

## when we want to connect to a shared web worker from client, we use a `port` before our `postMessage` and `onmessage`, what does that `port` property do?


In the context of using a `SharedWorker` in web development, the port property refers to a `MessagePort` object that is used for communication between the main thread (or other contexts) and the `SharedWorker`. Here's how it works:

1. Creating a `SharedWorker`: When you create a `SharedWorker`, you typically do so using the new `SharedWorker()` constructor. This creates an instance of the worker that can be shared across multiple browsing contexts (like different tabs or iframes).

2. Establishing Communication: To communicate with the `SharedWorker`, you need to use message passing. This is done through the `postMessage()` method, which sends messages to the worker.

3. Using `MessagePort`: When you connect to a `SharedWorker`, you can obtain a `MessagePort` object by calling the `connect()` method on your worker instance. This `port` is used for sending and receiving messages between your main thread and the worker.

4. `postMessage()` and `onmessage`:
   - The `postMessage()` method is called on this port to send messages from your client (the main thread) to the worker.
   - The worker listens for incoming messages using an event listener for the "message" event, which allows it to handle messages sent from any connected clients.

1. Benefits of Using `MessagePort`:
   - Direct Communication: Using ports allows for direct communication between multiple clients and a single shared worker.
   - Isolation: Each client has its own port, which helps in isolating message streams, making it easier to manage communication without interference from other clients.
   - Performance: Message ports can improve performance by allowing more efficient data transfer compared to traditional message passing methods.

Example

Here’s a simple example of how this works:

In your main JavaScript file:

```javascript
const worker = new SharedWorker('worker.js');
const port = worker.port;

port.start(); // Start communication

// Send a message to the SharedWorker
port.postMessage({ type: 'greeting', text: 'Hello, Worker!' });

// Listen for messages from SharedWorker
port.onmessage = function(event) {
    console.log('Received from Worker:', event.data);
};

In your Shared Worker (worker.js):

onconnect = function(event) {
    const port = event.ports[0];

    // Listen for messages from connected clients
    port.onmessage = function(event) {
        console.log('Received from Client:', event.data);
        
        // Respond back to client
        port.postMessage({ type: 'response', text: 'Hello, Client!' });
    };
};
```

In this example:
- The main script connects to a shared worker and obtains its message port.
- It sends a message using that port and sets up an event listener for incoming messages.
- The shared worker listens for connections and handles incoming messages accordingly.

This mechanism allows efficient communication between multiple clients and their shared workers while maintaining clear separation of message channels through individual ports.

## can we use web storage code inside a web worker (dedicated or shared or service)? how about `indexdb`?

No, you cannot use web storage (such as `localStorage` or `sessionStorage`) directly inside a web worker, whether it's a dedicated worker or a shared worker or a service worker but `indexdb` can be used in three of them. Web workers run in a separate global context and do not have access to the DOM or the window object, which are required for web storage APIs.

However, you can communicate between the main thread and the web worker using the `postMessage` method. You can send messages from the worker to the main thread, and the main thread can then access web storage and send any necessary data back to the worker.

Here's a simple example of how you might implement this:

### Main Thread
```javascript
// Create a new worker
const worker = new Worker('worker.js');

// Function to save data to localStorage
function saveToLocalStorage(data) {
    localStorage.setItem('myData', data);
}

// Listen for messages from the worker
worker.onmessage = function(event) {
    if (event.data.action === 'save') {
        saveToLocalStorage(event.data.value);
    }
};

// Send a message to the worker
worker.postMessage({ action: 'process', value: 'Hello, Worker!' });
```

### Worker (worker.js)
```javascript
// Listen for messages from the main thread
self.onmessage = function(event) {
    if (event.data.action === 'process') {
        // Process the data
        const processedData = event.data.value + ' processed';
        
        // Send a message back to the main thread to save data
        self.postMessage({ action: 'save', value: processedData });
    }
};
```

In this example, the worker processes some data and then sends a message back to the main thread to save it to `localStorage`. This way, you can effectively use web storage in conjunction with web workers, even though the workers themselves cannot access the storage directly.

I couldn't find any reasonable reason why we can use `indexdb` in workers but not web storages, the basic answer is, it's designed in this way because the application of these methods says, but there were some reason for it which I bring it on:

## why we can't use web storage directly inside of an web worker?

Web storage (like `localStorage` and `sessionStorage`) is designed to be used in the context of the main browser window or tab, where it has access to the Document Object Model (DOM) and the window object. Here are the main reasons why web storage cannot be used directly inside a web worker:

1. **Separate Execution Context**: Web workers run in a separate global context that is isolated from the main thread. This means they do not have access to the DOM or any of the APIs that are tied to the window object, including web storage.

2. **Security and Isolation**: The design of web workers emphasizes security and isolation. By preventing access to the DOM and web storage, the browser can ensure that workers do not interfere with the user interface or access sensitive data directly. This isolation helps maintain a clear separation between background processing and the user interface.

## why `indexdb` can be used in web workers but not web storages?

The ability to use `IndexedDB` in web workers while web storage (like `localStorage` and `sessionStorage`) is not accessible is primarily due to the design and intended use cases of these storage mechanisms. Here are the key reasons:

### 1. **Isolation and Security**
- **Web Workers**: Web workers run in a separate global context that is isolated from the main thread. This isolation is crucial for security and performance. Allowing direct access to web storage could lead to potential security risks, such as race conditions or unintended data manipulation, since web storage is tied to the DOM and the user interface.
- **`IndexedDB`**: It is designed to be more robust and secure for complex data transactions. It allows for structured data storage and retrieval, which is more suitable for the background processing that web workers perform.

### 2. **Use Cases**
- **`IndexedDB`**: It is intended for scenarios where applications need to store significant amounts of structured data, such as caching resources for offline use, storing user-generated content, or managing application state. This aligns well with the capabilities of web workers, which are often used for heavy computations or data processing tasks.
- **Web Storage**: It is more suited for simple key-value storage needs that are directly tied to the user interface. Since web workers do not interact with the DOM, the use of web storage in this context is not practical.


## what is I/O tasks in programming?

In programming, I/O tasks (Input/Output tasks) refer to operations that involve the transfer of data between a program and external entities, such as files, databases, networks, or user interfaces. These tasks are fundamental to how programs interact with the outside world and are essential for performing a wide range of functionalities.

### Key Aspects of I/O Tasks in Programming:

1. Types of I/O Operations:
   - File I/O: Reading from and writing to files on a storage medium (e.g., hard drives, SSDs). This includes operations like opening a file, reading its contents, writing data to it, and closing the file.
   - Network I/O: Sending and receiving data over a network. This includes operations like making HTTP requests, sending and receiving data through sockets, and interacting with web services or APIs.
   - Database I/O: Interacting with databases to perform operations such as querying data, inserting records, updating entries, and deleting data.
   - User I/O: Handling input from users (e.g., keyboard input, mouse events) and outputting data to users (e.g., displaying information on a screen).

2. Blocking vs. Non-blocking I/O:
   - Blocking I/O: The program execution is halted until the I/O operation completes. This can lead to inefficiencies, especially in applications that require responsiveness, as the program cannot perform other tasks while waiting.
   - Non-blocking I/O: The program can continue executing while the I/O operation is in progress. This is often implemented using callbacks, promises, or async/await patterns, allowing for more efficient use of resources.

3. Synchronous vs. Asynchronous I/O:
   - Synchronous I/O: The program executes I/O operations in a sequential manner, waiting for each operation to complete before proceeding to the next one. This can simplify code but may lead to performance bottlenecks.
   - Asynchronous I/O: The program initiates an I/O operation and continues executing other code without waiting for the operation to finish. Once the operation is complete, a callback or promise is used to handle the result, allowing for more responsive applications.

4. Error Handling: I/O operations can fail for various reasons (e.g., file not found, network issues, permission errors). Proper error handling is crucial to ensure that the program can gracefully handle such situations.

### Examples of I/O Tasks in Programming:

- File I/O: Reading a configuration file at the start of an application or writing logs to a file.
- Network I/O: Downloading data from a web API or sending data to a server.
- Database I/O: Querying a database for user information or updating records based on user input.
- User I/O: Capturing user input from a form and displaying results on a web page.

### Importance of I/O Tasks:

I/O tasks are critical for the functionality of applications, as they enable interaction with external systems and resources. Efficient handling of I/O operations is essential for building responsive and performant applications, especially in environments where latency and resource management are critical, such as web servers, real-time applications, and data processing systems. Properly managing I/O tasks can significantly enhance the user experience and overall performance of software applications.


## can you name some of I/O tasks in javascript?

 In JavaScript, I/O tasks can involve various operations related to reading from and writing to files, interacting with networks, and handling user input/output. Here are some common I/O tasks in JavaScript:

### 1. File I/O (Node.js)
In a Node.js environment, you can perform file I/O operations using the built-in fs (File System) module:

- Reading a File:
 
```javascript
  const fs = require('fs');

  fs.readFile('example.txt', 'utf8', (err, data) => {
      if (err) {
          console.error(err);
          return;
      }
      console.log(data);
  });
  
- Writing to a File:
 
  const fs = require('fs');

  fs.writeFile('output.txt', 'Hello, World!', (err) => {
      if (err) {
          console.error(err);
          return;
      }
      console.log('File has been written');
  });
```
  
### 2. Network I/O
JavaScript can perform network I/O tasks using the fetch API in the browser or libraries like axios in Node.js:

- Making an HTTP GET Request:
 
 ```javascript

  fetch('https://api.example.com/data')
      .then(response => response.json())
      .then(data => console.log(data))
      .catch(error => console.error('Error:', error));
  
- Making an HTTP POST Request:
 
  fetch('https://api.example.com/data', {
      method: 'POST',
      headers: {
          'Content-Type': 'application/json',
      },
      body: JSON.stringify({ key: 'value' }),
  })
      .then(response => response.json())
      .then(data => console.log(data))
      .catch(error => console.error('Error:', error));
```

  
### 3. Database I/O
In a Node.js environment, you can interact with databases using libraries like mongoose for MongoDB or pg for PostgreSQL:

- Querying a MongoDB Database:

 ```javascript
  const mongoose = require('mongoose');

  mongoose.connect('mongodb://localhost:27017/mydatabase', { useNewUrlParser: true, useUnifiedTopology: true });

  const User = mongoose.model('User', { name: String });

  User.find({}, (err, users) => {
      if (err) {
          console.error(err);
          return;
      }
      console.log(users);
  });
  ```
  
### 4. User Input/Output
In a web browser, you can handle user input and output using the DOM:

- Capturing User Input:
 
```html
  <input type="text" id="userInput" />
  <button id="submitButton">Submit</button>
  <div id="output"></div>

  <script>
      document.getElementById('submitButton').addEventListener('click', () => {
          const input = document.getElementById('userInput').value;
          document.getElementById('output').innerText = `You entered: ${input}`;
      });
  </script>
```


### 5. WebSocket I/O
You can use WebSockets for real-time communication between the client and server:

- Creating a WebSocket Connection:
```javascript 
  const socket = new WebSocket('ws://example.com/socket');

  socket.onopen = () => {
      console.log('WebSocket connection opened');
      socket.send('Hello Server!');
  };

  socket.onmessage = (event) => {
      console.log('Message from server:', event.data);
  };

  socket.onerror = (error) => {
      console.error('WebSocket error:', error);
  };
  ```
  
### Summary
These examples illustrate various I/O tasks in JavaScript, including file operations, network requests, database interactions, user input handling, and real-time communication. Each of these tasks is essential for building interactive and data-driven applications.

## What is the difference between module and web worker in JavaScript?

In JavaScript, modules and Web Workers serve very different purposes, even though both can be used to organize and run code. Here's a detailed comparison to clarify their differences:

---

### 1. Modules
Modules are a way to organize and structure JavaScript code by splitting it into separate files. They allow you to:
   - Encapsulate Code: Each module has its own scope, preventing pollution of the global namespace.
   - Reuse Code: Modules can export functions, objects, or variables for use in other modules.
   - Dependency Management: Modules can import functionality from other modules, making it easier to manage dependencies.

#### Key Features of Modules:
   - **import/export Syntax**: Modules use import and export to share code between files.
 Static Loading: Modules are loaded statically (at parse time) in most environments.
 Main Thread Execution: Modules run on main thread, just like regular JavaScript code.

#### Example of a Module:

```JavaScript
// math.js (module)
export function add(a, b) {
    return a + b;
}

// main.js (main script)
import { add } from './math.js';
console.log(add(2, 3)); // Output: 5
```
---

2. Web Workers
Web Workers are a browser feature that allows you to run JavaScript code in backgroundnd** on a separate thread. They are used to:
 Offload Heavy Tasksks**: Perform computationally expensive tasks without blocking the main thread.
 Concurrencycy**: Run code in parallel with the main thread.
 Isolationon**: Workers run in a separate global context and cannot access the DOM or window object.

#### Key Features of Web Workers:
 Separate Threadad**: Workers run on a separate thread, independent of the main thread.
 Message Passingng**: Workers communicate with the main thread via postMessage and onmessage.
 No DOM Accessss**: Workers cannot directly manipulate the DOM or access the window object.
 Dynamic Loadingng**: Workers are loaded dynamically (at runtime).

#### Example of a Web Worker:
```javascript
// worker.js (worker script)


self.onmessage = (event) => {
    const result = event.data * 2;
    self.postMessage(result);
};

// main.js (main script)
const worker = new Worker('worker.js');
worker.postMessage(5);
worker.onmessage = (event) => {
    console.log('Result from worker:', event.data); // Output: 10
};
```
---


---

When to Use Modules
- Use modules when you want to:
  - Organize your code into reusable components.
  - Manage dependencies between different parts of your application.
  - Encapsulate functionality to avoid polluting the global namespace.

---

When to Use Web Workersrs
- Use Web Workers when you want to:
  - Perform heavy computations or tasks without blocking the main thread.
  - Run code in parallel to improve performance.
  - Handle background tasks like data processing, image manipulation, or fetching large amounts of data.

---
### Can Modules and Web Workers Work Together?
Yes! You can use modules inside Web Workers to organize worker code. Modern browsers support module workers, which allow you to use import/export syntax in workers.

#### Example of a Module Worker:
```javascript
// worker.js (module worker)
import { add } from './math.js';

self.onmessage = (event) => {
    const result = add(event.data.a, event.data.b);
    self.postMessage(result);
};

// main.js (main script)
const worker = new Worker('worker.js', { type: 'module' });
worker.postMessage({ a: 2, b: 3 });
worker.onmessage = (event) => {
    console.log('Result from worker:', event.data); // Output: 5
};
```
---

### Conclusion
- Modules are for organizing and structuring code on the main thread.
- Web Workers are for running code in the background on a separate thread.
- They serve different purposes but can be used together to build efficient and well-structured applications.

## what's the difference between single threaded and multi-threaded language in terms of performance?

The difference between single-threaded and multi-threaded languages in terms of performance primarily revolves around how they handle tasks and utilize system resources. Here’s a breakdown of the key differences:

Single-Threaded Languages

1. Execution Model: In a single-threaded environment, only one thread of execution runs at a time. This means that tasks are executed sequentially.

2. Performance:
   - Simplicity: Easier to implement and debug since there is no need to manage multiple threads.
   - Blocking Operations: If a task takes a long time (like I/O operations), it can block the entire execution, leading to inefficiencies.
   - CPU Utilization: Limited to one core at a time, which can lead to underutilization of multi-core processors.

3. Use Cases: Suitable for applications where tasks are simple and do not require concurrent execution, such as small scripts or applications with minimal I/O operations.

Multi-Threaded Languages

1. Execution Model: Multi-threaded languages allow multiple threads to run concurrently, enabling parallel execution of tasks.

2. Performance:
   - Concurrency: Can perform multiple operations simultaneously, which can significantly improve performance for CPU-bound tasks on multi-core processors.
   - Responsiveness: Better responsiveness in applications (e.g., GUIs) since one thread can handle user input while others perform background processing.
   - Complexity: More complex to implement due to potential issues like race conditions, deadlocks, and the need for synchronization mechanisms.

3. Use Cases: Ideal for applications that require high performance and responsiveness, such as web servers, real-time data processing systems, and applications with heavy I/O operations.

Summary

- Single-threaded languages are simpler but may suffer from performance bottlenecks due to blocking operations and limited CPU utilization.
- Multi-threaded languages, while more complex, can leverage modern multi-core architectures for better performance through concurrent execution but require careful management of threads.

In practice, the choice between single-threaded and multi-threaded approaches depends on the specific requirements of the application being developed.

## What is synchoronous and asynchronous in programming?

Synchronous and asynchronous code are two different paradigms for handling operations, particularly in programming and software development. They primarily relate to how tasks are executed and how the program handles waiting for those tasks to complete.

Synchronous Code

- Definition: In synchronous programming, tasks are executed one after another. Each task must complete before the next one begins. This means that if a task takes a long time to complete (like reading a file or making a network request), the entire program will wait (or block) until that task is finished.

- Characteristics:
  - Easier to understand and reason about since the flow of execution is linear.
  - Can lead to performance issues if long-running tasks block the main thread, especially in user interfaces or server applications.
  
- Example:
  
```python
  def fetch_data():
      data = read_file()  This blocks until the file is read
      process_data(data)   This only runs after fetch_data completes

  fetch_data()
 ```

Asynchronous Code

- Definition: In asynchronous programming, tasks can be initiated and then run independently of the main program flow. The program can continue executing other code while waiting for these tasks to complete. When an asynchronous task finishes, it typically uses callbacks, promises, or async/await syntax to handle the result.

- Characteristics:
  - More complex than synchronous code but allows for better performance in I/O-bound applications (like web servers).
  - Helps prevent blocking of the main thread, which is crucial for maintaining responsiveness in applications.
  
- Example (using Python's async/await):
  
```python
  import asyncio

  async def fetch_data():
      data = await read_file_async()  This does not block; it returns immediately
      await process_data_async(data)   This also runs asynchronously

  asyncio.run(fetch_data())
 ``` 

Key Differences

1. Execution Flow:
   - Synchronous: Sequential execution; each operation waits for the previous one to finish.
   - Asynchronous: Non-blocking; operations can start and continue without waiting.

2. Use Cases:
   - Synchronous: Suitable for CPU-bound tasks where operations need to be completed in order.
   - Asynchronous: Ideal for I/O-bound tasks like network requests or file operations where waiting times can be significant.

3. Complexity:
   - Synchronous code is generally simpler and easier to debug.
   - Asynchronous code can introduce complexity due to callbacks or state management but offers better performance in certain scenarios.

Understanding when to use synchronous versus asynchronous programming is crucial for building efficient applications that respond well under load or during long-running operations.

## do single threaded languages get considered to be synchronous?

Yes, single-threaded languages are often considered to be synchronous because they typically execute code in a sequential manner, processing one operation at a time. In a single-threaded environment, when a function is called, the program must complete that function before moving on to the next one. This means that if an operation takes time (like I/O operations), the entire program waits for that operation to finish before continuing.

In contrast, asynchronous programming allows for non-blocking operations where the program can initiate an operation and continue executing other code while waiting for that operation to complete. This is often achieved through callbacks, promises, or async/await constructs.

However, it's important to note that some single-threaded languages (like JavaScript) can still support asynchronous programming patterns through event loops and callbacks. In these cases, while the language itself is single-threaded, it can handle asynchronous operations by allowing certain tasks to be executed in a non-blocking manner.

In summary:

- Single-threaded languages: Generally synchronous due to sequential execution.
- Asynchronous capabilities: Some single-threaded languages can implement asynchronous patterns despite being single-threaded.

## how JavaScript is single threaded but asynchronous?
JavaScript is often described as a single-threaded language, which means that it has a single call stack and executes one operation at a time. However, it also supports asynchronous programming, allowing it to handle operations like I/O tasks (e.g., network requests, file reading) without blocking the execution of other code. This might seem contradictory at first, but here's how it works:

Single-Threaded Nature

1. Call Stack: JavaScript uses a call stack to manage function calls. When a function is invoked, it's added to the stack; when it returns, it's removed from the stack. Since there's only one call stack, only one piece of code can execute at any given time.

2. Event Loop: The event loop is a mechanism that allows JavaScript to perform non-blocking operations despite being single-threaded. It continuously checks the call stack and the message queue (or task queue) for tasks that need to be executed.

Asynchronous Programming

1. `Callbacks`: Functions can be passed as arguments to other functions and executed later (callbacks). For example, you might pass a callback function to handle the result of an asynchronous operation.

2. `Promises`: Promises provide a more powerful way to handle asynchronous operations by representing values that may be available now or in the future. They allow chaining of operations and better error handling.

3. `Async/Await`: Introduced in ES2017 (ES8), async and await syntax allows writing asynchronous code in a more synchronous style while still being non-blocking under the hood.

How It Works Together

1. Non-Blocking I/O: When an asynchronous operation (like fetching data from an API) is initiated, JavaScript sends this request off and continues executing subsequent code without waiting for the response.

2. Message Queue: Once the asynchronous operation completes (e.g., data is received), its callback or promise resolution is placed in the message queue.

3. Event Loop Processing: The event loop continuously checks if the call stack is empty:
   - If it is empty, it takes the first task from the message queue and pushes it onto the call stack for execution.
   - This process allows JavaScript to handle multiple asynchronous operations efficiently while still maintaining its single-threaded nature.

Example

Here's an example illustrating this concept:

```javascript
console.log("Start");

setTimeout(() => {
    console.log("Timeout 1");
}, 1000);

setTimeout(() => {
    console.log("Timeout 2");
}, 500);

console.log("End");
```

```
Output:
Start
End
Timeout 2
Timeout 1
```

In this example:
- "Start" and "End" are logged immediately because they are synchronous.
- The two `setTimeout` calls are asynchronous; they don't block further execution.
- After about 500 milliseconds, "Timeout 2" gets logged followed by "Timeout 1" after another 500 milliseconds because they were placed in the message queue when their timers expired.

Conclusion

JavaScript's single-threaded nature means that only one piece of code runs at any given time within its main thread; however, through mechanisms like callbacks, promises, and async/await combined with an event loop and message queue system, JavaScript can efficiently manage multiple asynchronous tasks without blocking execution flow.

## what's the difference between JavaScript and a                multi-threaded language like java in terms of performance?

The performance differences between JavaScript and a multi-threaded language like Java can be attributed to several factors, including their execution models, concurrency handling, and typical use cases. Here’s a breakdown of the key differences:

1. Execution Model:
   - JavaScript:
     - JavaScript is primarily single-threaded and runs in an event-driven environment (like the browser or Node.js). It uses an event loop to handle asynchronous operations.
     - While it can handle asynchronous tasks (like I/O operations) without blocking the main thread, it does not natively support multi-threading in the same way as Java.
     - Web Workers allow for some level of parallelism, but they are limited in terms of shared state and communication overhead.

   - Java:
     - Java is designed with multi-threading in mind. It allows multiple threads to run concurrently, which can lead to better CPU utilization on multi-core processors.
     - Java threads are managed by the JVM (Java Virtual Machine), which provides robust support for synchronization and inter-thread communication.

2. Concurrency Handling:
   - JavaScript:
     - Uses callbacks, promises, and async/await for handling asynchronous operations. This model can lead to "callback hell" if not managed properly.
     - The single-threaded nature means that long-running tasks can block the main thread, leading to performance issues in UI applications.

   - Java:
     - Provides built-in support for threading with classes like Thread, Runnable, and higher-level abstractions like ExecutorService.
     - Offers synchronization mechanisms (like synchronized blocks and locks) to manage shared resources between threads effectively.

3. Performance Characteristics:
   - JavaScript:
     - Generally faster for I/O-bound tasks due to its non-blocking nature.
     - Performance may degrade with CPU-bound tasks since they can block the event loop.
     - The JIT (Just-In-Time) compilation used by modern JavaScript engines (like V8) optimizes execution speed but still operates within a single thread.

   - Java:
     - Better suited for CPU-bound tasks due to its ability to utilize multiple cores through threading.
     - The JVM also employs JIT compilation, optimizing performance over time as it learns from execution patterns.

4. Use Cases:
   - JavaScript: 
     - Ideal for web development where responsiveness is crucial. It excels in scenarios requiring quick I/O operations or real-time updates (e.g., web applications).
   
   - Java: 
     - Commonly used in enterprise applications, backend services, and systems requiring heavy computation or complex data processing where multi-threading can significantly enhance performance.

Conclusion:
In summary, while both languages have their strengths and weaknesses regarding performance, they cater to different types of applications. Java's multi-threading capabilities make it more suitable for CPU-intensive tasks that benefit from parallel execution. In contrast, JavaScript's non-blocking I/O model makes it ideal for responsive web applications but may struggle with CPU-bound processes due to its single-threaded nature. The choice between them should depend on the specific requirements of your application rather than purely on performance metrics.

## What's CPU-bound task in programming?

A CPU-bound task in programming refers to a type of computation that is limited by the processing power of the CPU (Central Processing Unit). In other words, the performance of a CPU-bound task is primarily constrained by how fast the CPU can execute instructions, rather than by other factors such as I/O operations (disk or network access) or memory bandwidth.

Characteristics of CPU-Bound Tasks:

1. High Computation Requirement: These tasks involve intensive calculations or data processing, such as mathematical computations, simulations, or complex algorithms.

2. Limited I/O Operations: Unlike I/O-bound tasks, which spend a significant amount of time waiting for input/output operations to complete (like reading from disk or network), CPU-bound tasks keep the CPU busy with computations.

3. Performance Scaling: The performance of CPU-bound tasks can often be improved by using more powerful CPUs or optimizing algorithms to reduce computational complexity.

4. Multithreading Potential: Many CPU-bound tasks can benefit from parallel processing and multithreading, allowing them to utilize multiple cores of a processor effectively.

Examples:

- Image processing and rendering
- Video encoding/decoding
- Scientific simulations (e.g., physics simulations)
- Data analysis and machine learning model training

In summary, when optimizing for performance in programming, identifying whether a task is CPU-bound helps developers choose appropriate strategies for improvement, such as algorithm optimization or leveraging multi-core processors.

## What's the application of web workers in JavaScript? 

Web Workers in JavaScript are a powerful feature that allows you to run scripts in background threads, separate from the main execution thread of a web application. This is particularly useful for performing computationally intensive tasks without blocking the user interface, leading to a smoother user experience.

Applications of Web Workers

1. Heavy Computation: Offloading heavy calculations (like image processing, data analysis, etc.) to a worker thread.
2. Data Fetching: Performing network requests without freezing the UI.
3. Real-time Data Processing: Handling real-time data streams (like WebSocket messages) efficiently.
4. Parallel Processing: Splitting tasks into smaller chunks and processing them concurrently.

Examples

1. Basic Example of a Web Worker

Here’s how you can create a simple web worker that performs a calculation:

```javascript
//main.js
// Check if the browser supports Web Workers
if (window.Worker) {
    const myWorker = new Worker('worker.js');

    // Send data to the worker
    myWorker.postMessage(10); // Sending number 10 to worker

    // Listen for messages from the worker
    myWorker.onmessage = function(e) {
        console.log('Result from worker:', e.data);
    };
}
```

```javascript
//worker.js
// Listen for messages from the main script
onmessage = function(e) {
    const result = e.data * 2; // Perform some computation (e.g., double the number)
    postMessage(result); // Send result back to main script
};
```

2. Fetching Data with Web Workers

You can use web workers to fetch data without blocking the UI:

```javascript
//main.js
if (window.Worker) {
    const fetchWorker = new Worker('fetchWorker.js');

    fetchWorker.onmessage = function(e) {
        console.log('Fetched data:', e.data);
    };

    fetchWorker.postMessage('https://api.example.com/data'); // URL to fetch data from
}
```

```javascript
//fetchWorker.js
onmessage = function(e) {
    const url = e.data;

    fetch(url)
        .then(response => response.json())
        .then(data => {
            postMessage(data); // Send fetched data back to main script
        })
        .catch(error => {
            postMessage({ error: 'Failed to fetch data' });
        });
};
```

3. Real-time Data Processing Example

This example shows how you might handle real-time updates using WebSockets in a worker:

```javascript
//main.js
if (window.Worker) {
    const socketWorker = new Worker('socketWorker.js');

    socketWorker.onmessage = function(e) {
        console.log('Processed message:', e.data);
    };

    socketWorker.postMessage('ws://example.com/socket'); // URL of your WebSocket server
}
```

```javascript
//socketWorker.js
let socket;

onmessage = function(e) {
    const url = e.data;
    
    socket = new WebSocket(url);

    socket.onmessage = function(event) {
        const messageData = JSON.parse(event.data);
        
        // Process incoming message and send it back to main thread
        postMessage(processData(messageData));
    };
};

function processData(data) {
   // Perform some processing on incoming data here...
   return Processed: ${data};
}
```

Conclusion

Web Workers are an essential tool for improving performance in web applications by allowing heavy computations and I/O operations to run off the main thread, thus keeping the UI responsive. They are particularly useful in scenarios involving large datasets, complex calculations, or real-time updates where performance is critical.

## what is message queue in JavaScript?

the data which we transfer between the main thread and workers called ***message*** (we've elaborated about message definition earlier), we have **message queue** which stores messages, this queue is located in macro task (based on some references), whenever we reach an `onmessage` event in our code, that `onmessage` event stores in message queue and waits for messages to be triggered, it doesn't have a precise execution order and only execute the `onmessage` that the message is received. `onconnect` I think stores in this section (message queue) but I couldn't find any approval for this statement, hence this is my personal deduction.

## We have a core i3 CPU which obviously has 3 cores, as far as I know each core has 2 threads which makes it 6 threads, if we create 10 web workers in JavaScript, how that code is going to execute?

spec says that it takes time to let those workers that their order exceeds the possible amount of cores to get executed but in real world experience, they all executed all together and no problem occurred.

## I have a javascript file which contains web workers, it works fine when I run jn browsers through script tag in an HTML file but when I want to run it from terminal of visual studio code, it doesn't show any output, why this occurs?

When you run a JavaScript file that uses Web Workers in a browser environment, the browser provides the necessary context and APIs to support Web Workers. However, when you try to run the same JavaScript file directly from the terminal (like in Visual Studio Code) using Node.js or another JavaScript runtime, it won't work as expected for several reasons:

1. Web Worker API: Web Workers are part of the web platform and are not available in Node.js or other non-browser environments. The Worker constructor and related APIs are specific to browsers.

2. Environment Differences: Browsers have a DOM (Document Object Model) and other web APIs that are not present in Node.js. When you run your script in a terminal, it lacks these browser-specific features.

3. File Context: In a browser, scripts can be loaded as part of an HTML document, which provides the necessary context for running Web Workers. Running a standalone JavaScript file from the terminal does not provide this context.

Solutions

If you want to test or run code that uses Web Workers outside of a browser environment, consider these options:

1. Use a Local Server: Instead of running your script directly from the terminal, set up a local server (like using http-server, live-server, or similar tools) and access your HTML file through that server in your web browser.

    
  `npm install -g http-server`

2. Browser Development Tools: Use tools like Chrome DevTools or Firefox Developer Edition to debug and test your code with Web Workers directly in the browser.

3. Testing Frameworks: If you're looking to write tests for your worker code, consider using testing frameworks that support web environments like Jest with jsdom or Mocha with Chai.

4. Node.js Worker Threads: If you need similar functionality in Node.js, consider using Worker Threads (worker_threads module). This is different from Web Workers but allows for multi-threading within Node.js applications.

Example of Using Worker Threads

Here’s how you might use worker threads in Node.js:
```javascript
// main.js
const { Worker } = require('worker_threads');

const worker = new Worker('./worker.js');

worker.on('message', message => {
    console.log(Received from worker: ${message});
});

worker.postMessage('Hello Worker!');
```

```javascript
// worker.js
const { parentPort } = require('worker_threads');

parentPort.on('message', message => {
    console.log(Received from main thread: ${message});
    parentPort.postMessage('Hello Main!');
});
```

In summary, if you're working with Web Workers specifically designed for browsers, you'll need to run them within an HTML context served by a web server rather than directly through Node.js or any terminal command line interface.

## Why web workers in js are browser specific and they cannot be run with node.js? what's going on under the hood which cannot be done with node.js?

Web Workers in JavaScript are designed to run in the context of a web browser, and they provide a way to execute scripts in background threads. This allows for parallel execution of code without blocking the main thread, which is particularly useful for tasks that require significant computation or that would otherwise cause the user interface to become unresponsive.

Why Web Workers are Browser-Specific

1. Environment Context: Web Workers are part of the web platform API, which is specifically designed for browsers. They rely on the Document Object Model (DOM) and other browser-specific features that are not present in Node.js. For example, Web Workers can interact with window, document, and other browser APIs.

2. Thread Management: Browsers manage their own threading model and provide a specific implementation of Web Workers that allows them to run scripts concurrently with the main UI thread. This management includes handling communication between workers and the main thread via message passing.

3. Security Model: The security model of browsers includes restrictions on what workers can access (e.g., no direct access to the DOM). This is important for maintaining security and performance in a multi-threaded environment where different scripts may be running concurrently.

Node.js and Worker Threads

Node.js does support multi-threading through its own mechanism called "Worker Threads," which was introduced in Node.js 10.5.0 as an experimental feature and became stable in later versions. However, these worker threads are different from Web Workers:

1. Different APIs: The API for Worker Threads in Node.js is different from that of Web Workers in browsers. While both allow for concurrent execution, they do not share the same context or API surface area.

2. No DOM Access: Worker Threads do not have access to any browser-specific features like the DOM or window object because Node.js operates outside of a browser environment.

3. Use Cases: The use cases for Worker Threads in Node.js often revolve around I/O-bound tasks or CPU-intensive operations that need to be offloaded from the main event loop, while Web Workers are primarily used for enhancing user experience by keeping UI responsive during heavy computations.

Summary

In summary, while both Web Workers (in browsers) and Worker Threads (in Node.js) serve similar purposes regarding concurrency, they operate within different environments with distinct APIs and capabilities tailored to their respective contexts—browsers versus server-side JavaScript execution environments like Node.js.

## What is self in web workers?

self is for accessing something like window in web workers since we can't access window keyword in web workers and if we want to use window keywords in places that we need such a functionality, we have to use self keyword, and bear in mind if you want to have almost same experience which you have with window in main thread in workers, you have to use self and there is no other solution and using things like `DedicatedWorkerGlobalScope` won't work.

self job is to give a identical version of windows, you can even use self in a main thread and there is no difference between self and windows in main thread but the useful application I found for self is to use it as a window in workers.

## Why web workers run in another global context than the main thread in JavaScript?

**Isolation**: Each Web Worker has its own global scope, which means that variables and functions defined in a worker do not interfere with those in the main thread or other workers. This isolation helps prevent issues related to variable collisions and makes it easier to manage state in complex applications.

 **Security**: Running in a separate context enhances security by limiting the access that workers have to the main thread's environment. Workers cannot directly manipulate the DOM or access certain APIs that could compromise the security of the main thread. This separation helps to mitigate risks associated with running untrusted code.

## An interesting case for web workers and html `script` tag

for instance the test.js is your main thread and worker.js is worker, in your html file if you put `test.js` as your `src` in script tag and you use document key word in worker.js, you can't access the document, since we don't have access to DOM in workers but if I insert `worker.js` as `src` in script tag, document keyword works in worker.js because in this case worker.js is not the worker and it's the main thread because in the first scenario, the worker.js is the worker because it is passed as the script in `new Worker()` in tets.js and test.js is the main thread also, `test.js` is the main thread because it is passed as `src` in script tag of html, is the main thread.

## What's the difference of window in main thread and self in a web worker in term of their methods?

The window object in the main thread and the self object in a Web Worker both serve as the global context for their respective environments, but they have different methods and properties available due to the distinct roles they play. Here are the key differences:

### 1. DOM Access
- `window`: The window object provides access to the Document Object Model (DOM) and allows manipulation of HTML elements, styles, and events. It includes methods like document.getElementById(), window.alert(), and window.location.
- `self`: The self object in a Web Worker does not have access to the DOM. It cannot manipulate HTML elements or access any DOM-related methods or properties. This is by design to ensure that workers remain isolated and focused on computation.

### 2. Event Handling
- `window`: The window object can handle a wide range of events, including user interface events (like clicks and keyboard events), load events, and more. It has methods like addEventListener() for attaching event listeners.
- `self`: The self object can handle specific events related to the worker, such as onmessage, onerror, and oninstall (for service workers). It does not handle UI events since it does not have a user interface.

### 3. Timers
- Both window and self provide methods for timers:
  - `window`: Methods like setTimeout(), setInterval(), and clearTimeout() are available.
  - `self`: The same timer methods (setTimeout(), setInterval(), and clearTimeout()) are available in the worker context, but they operate independently of the main thread.

### 4. Web APIs
- `window`: The window object has access to a wide range of Web APIs, including the Fetch API, Web Storage (localStorage and sessionStorage), and the Geolocation API, among others.
- `self`: The self object in a Web Worker has access to some Web APIs, but not all. For example, it can use the Fetch API and IndexedDB, but it cannot use APIs that require a DOM context, such as the Canvas API or the Web Audio API (in certain contexts).

### 5. Global Scope
- `window`: In the main thread, window is the global object, and any global variables or functions are properties of window.
- `self`: In a Web Worker, self serves a similar purpose, but it does not include any DOM-related properties or methods. Global variables and functions defined in the worker are properties of self.

### Summary
In summary, while both window and self serve as the global context for their respective environments, window provides access to the DOM and a broader range of Web APIs, while self is focused on computation and does not have access to the DOM. This design helps maintain the separation of concerns between the main thread and Web Workers, allowing for efficient background processing without interfering with the user interface.

## Why it takes time for `onconnct` in shared worker to establish?

The `onconnect` event in a Shared Worker can take time to establish for several reasons:

1. Browser Initialization: When a Shared Worker is created, the browser needs to initialize the worker environment. This includes setting up the JavaScript execution context and allocating resources.

2. Network Latency: If the Shared Worker is being loaded from a remote server, network latency can affect how quickly the worker script is fetched and executed.

3. Script Execution Time: The code within the Shared Worker needs to be executed before it can handle connections. If there are any synchronous operations or heavy computations in the worker's initialization code, this can delay the `onconnect` event.

4. Event Loop and Concurrency: JavaScript runs on a single-threaded event loop. If there are other tasks queued in the event loop (like UI updates or other scripts), they may delay the processing of events, including `onconnect`.

5. Multiple Connections: If multiple clients are trying to connect to the same Shared Worker simultaneously, there may be some queuing involved as each connection is established one after another.

6. Resource Contention: If your application is resource-intensive or if there are many workers running concurrently, this could lead to contention for CPU and memory resources, slowing down initialization.

7. Garbage Collection: The JavaScript engine may also be performing garbage collection during this time, which can introduce delays.

8. Security Contexts: Depending on how your application is structured (e.g., different origins), establishing a connection might involve additional security checks that could add overhead.

To mitigate some of these delays, you can optimize your worker's initialization code by minimizing synchronous operations and ensuring that any heavy computations are offloaded appropriately or handled asynchronously where possible.

## why The code within the Shared Worker needs to be executed before it can handle connections?

In a Shared Worker environment, the code within the worker needs to be executed before it can handle connections for several reasons:

1. Initialization: The Shared Worker may need to perform certain initialization tasks before it can accept connections. This could include setting up data structures, initializing variables, or establishing connections to other resources (like databases or APIs). Until these tasks are completed, the worker may not be ready to handle incoming messages or requests.

2. Event Listeners: The Shared Worker must set up event listeners to handle incoming connections and messages. If the worker's code hasn't executed yet, these listeners won't be in place, and any attempts to connect will fail or go unhandled.

3. Context Setup: The execution of the worker's code establishes its execution context. This includes defining how it will respond to messages from connected clients and what data it will share among them. Without this context being set up first, the worker cannot properly manage its responsibilities.

4. Concurrency Management: Shared Workers are designed to handle multiple connections from different scripts running in different browsing contexts (like tabs or iframes). The worker needs to manage these connections effectively, which requires that its internal logic is fully loaded and operational before any connection attempts are made.

5. Error Handling: If there are errors in the initialization code (e.g., syntax errors or runtime exceptions), those need to be caught and handled appropriately before the worker starts accepting connections. Otherwise, clients might connect only to encounter unexpected behavior or crashes.

6. Lifecycle Management: The lifecycle of a Shared Worker involves various states (e.g., starting, running, terminating). Ensuring that the worker is fully started and ready helps maintain a predictable interaction model for connected clients.

In summary, executing the code within a Shared Worker before handling connections ensures that it is properly initialized and ready to manage communication effectively with all connected clients.

## What's the difference between using click event in `addEventListener` and as `onclick` in JavaScript file or `onclick` in html as inline?

In JavaScript, there are several ways to handle click events on elements, and each method has its own characteristics and use cases. Here’s a breakdown of the differences between using `addEventListener`, the `onclick` property in a JavaScript file, and inline `onclick` attributes in HTML:

1. Using addEventListener

```javascript
const button = document.getElementById('myButton');
button.addEventListener('click', function() {
    console.log('Button clicked!');
});
```

Advantages:
- Multiple Handlers: You can attach multiple event listeners to the same element for the same event type without overwriting existing ones.
- Event Options: You can specify options like capture, once, and passive.
- Separation of Concerns: Keeps JavaScript separate from HTML, promoting cleaner code and better maintainability.
- Dynamic Binding: You can add or remove event listeners dynamically at runtime.

Disadvantages:
- Slightly more verbose than inline handlers.

2. Using the `onclick` Property in a JavaScript File
```javascript
const button = document.getElementById('myButton');
button.onclick = function() {
    console.log('Button clicked!');
};
```
Advantages:
- Simple syntax for adding a single click handler.
- Keeps JavaScript separate from HTML.

Disadvantages:
- Single Handler Limitation: If you assign a new function to `onclick`, it will overwrite any existing handler. Only one handler can be assigned at a time.
- Less flexibility compared to `addEventListener`.

3. Using Inline onclick in HTML

```HTML
<button id="myButton" onclick="console.log('Button clicked!')">Click me</button>
```
Advantages:
- Very straightforward for simple cases; easy to understand at a glance.
- No need to wait for DOM content to load since the handler is defined directly in the HTML.

Disadvantages:
- Mixing Concerns: It mixes HTML with JavaScript, which can lead to less maintainable code.
- Harder to manage if you have many event handlers or complex logic; it can clutter your HTML.
- Limited debugging capabilities compared to external scripts (e.g., you can't easily set breakpoints).
  
Summary

1. Use `addEventListener` when you need flexibility (multiple handlers, options) and want clean separation of concerns.
2. Use the `onclick` property when you only need one handler and prefer simplicity without mixing with HTML.
3. Use inline `onclick` attributes for very simple cases or quick prototypes but avoid them in production code due to maintainability issues.

Choosing between these methods often depends on your specific use case, coding style preferences, and project requirements.

## Can we only use `onclick` event as inline in our HTML code?

No, the `onclick` event is not the only event that can be used inline in HTML. While `onclick` is one of the most commonly used events for handling click actions, there are many other events that can also be specified inline. Here are some examples of other events that can be used inline:

1. Mouse Events:
   - `onmouseover`: Triggered when the mouse pointer moves over an element.
   - `onmouseout`: Triggered when the mouse pointer moves out of an element.
   - `onmousedown`: Triggered when a mouse button is pressed down on an element.
   - `onmouseup`: Triggered when a mouse button is released over an element.

2. Keyboard Events:
   - `onkeydown`: Triggered when a key is pressed down.
   - `onkeyup`: Triggered when a key is released.
   - `onkeypress`: Triggered when a key is pressed (deprecated in favor of keydown and keyup).

3. Form Events:
   - `onsubmit`: Triggered when a form is submitted.
   - `onchange`: Triggered when the value of an input changes.
   - `onfocus`: Triggered when an input gains focus.
   - `onblur`: Triggered when an input loses focus.

4. Window Events:
   - `onload`: Triggered when the page has finished loading.
   - `onresize`: Triggered when the window is resized.

5. Touch Events (for mobile devices):
   - `ontouchstart`, `ontouchmove`, and `ontouchend`.

Example of Inline Event Handlers

Here’s how you might use some of these events inline in HTML:
```html
<button onclick="alert('Button clicked!')">Click Me</button>
<input type="text" onfocus="this.style.backgroundColor='yellow'" onblur="this.style.backgroundColor='white'">
<div onmouseover="this.style.color='red'" onmouseout="this.style.color='black'">Hover over me!</div>
```

Best Practices

While using inline event handlers can be convenient for small scripts or quick prototypes, it’s generally recommended to separate JavaScript from HTML for better maintainability and readability. This can be done by adding event listeners using JavaScript:

```html
<button id="myButton">Click Me</button>

<script>
  document.getElementById('myButton').onclick = function() {
    alert('Button clicked!');
  };
</script>
```

This approach keeps your HTML clean and separates concerns, making your code easier to manage and debug.

## what is race condition in a multi-threaded language like java?

In a multi-threaded language like Java, a race condition occurs when two or more threads access shared resources concurrently, and at least one of the threads modifies that resource. The outcome of the program can depend on the timing and order of thread execution, leading to unpredictable behavior and potential bugs.


### Example of a Race Condition in Java

Consider a simple example where two threads increment a shared counter:

```java
public class Counter {
    private int count = 0;

    public void increment() {
        count++; // This is not atomic
    }

    public int getCount() {
        return count;
    }
}

public class RaceConditionExample {
    public static void main(String[] args) throws InterruptedException {
        Counter counter = new Counter();
        
        Thread thread1 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) {
                counter.increment();
            }
        });

        Thread thread2 = new Thread(() -> {
            for (int i = 0; i < 1000; i++) {
                counter.increment();
            }
        });

        thread1.start();
        thread2.start();
        thread1.join();
        thread2.join();

        System.out.println("Final count: " + counter.getCount());
    }
}
```

In this example, both `thread1` and `thread2` increment the `count` variable 1000 times. However, the `increment()` method is not synchronized, which means that both threads can read and write to `count` simultaneously. This can lead to a situation where increments are lost, resulting in a final count that is less than 2000.

### Preventing Race Conditions

To prevent race conditions in Java, you can use synchronization mechanisms:

1. **Synchronized Methods**: You can declare the `increment()` method as synchronized, which ensures that only one thread can execute it at a time.

   ```java
   public synchronized void increment() {
       count++;
   }
   ```

2. **Synchronized Blocks**: You can use synchronized blocks to limit the scope of synchronization to specific sections of code.

   ```java
   public void increment() {
       synchronized (this) {
           count++;
       }
   }
   ```

3. **Atomic Variables**: Java provides atomic classes in the `java.util.concurrent.atomic` package, such as `AtomicInteger`, which can be used for thread-safe operations without explicit synchronization.

   ```java
   import java.util.concurrent.atomic.AtomicInteger;

   public class Counter {
       private AtomicInteger count = new AtomicInteger(0);

       public void increment() {
           count.incrementAndGet();
       }

       public int getCount() {
           return count.get();
       }
   }
   ```

By using these techniques, you can ensure that your multi-threaded Java applications behave predictably and avoid race conditions.

## why DOM is blocked and we can't access DOM in web workers in JavaScript?

because consider DOM elements like `P` or `img` as variables in JavaScript, so we should be able to access this variables only from one thread and not multiple threads because if we were able to access and manipulate these variables from different threads, race condition would appear which results in unpredictable outputs and bugs, so JavaScript limits access of DOM only to main thread and access to DOM is restricted in web workers due to race conditions possibility and the reason we can't use `window` in web workers is, `window` contains DOM methods, so we shouldn't be allowed to have them in workers, hence another object we have called `DedicatedWorkerGlobalScope` which can be utilized with `self` keyword.

# 20. when we can stop using `{}` in arrow functions?

In JavaScript, when using arrow functions, the use of curly braces `{}` depends on how you want to structure the function body. Here are the guidelines:

1. **Single Expression (Implicit Return)**:
   - If the arrow function consists of a single expression, you can omit the curly braces, and the expression will be returned implicitly.
   ```javascript
   const add = (a, b) => a + b; // Implicit return
   ```

2. **Multiple Statements (Explicit Return)**:
   - If the function body contains multiple statements, you must use curly braces. In this case, you also need to use the `return` statement to return a value.
   ```javascript
   const add = (a, b) => {
       const sum = a + b;
       return sum; // Explicit return
   };
   ```

3. **No Parameters**:
   - If there are no parameters, you can use empty parentheses `()` and still use curly braces if you have multiple statements.
   ```javascript
   const greet = () => {
       console.log("Hello!");
   };
   ```

4. **Single Parameter**:
   - If there is a single parameter, you can omit the parentheses, but you can still use curly braces if needed.
   ```javascript
   const square = x => {
       return x * x; // Explicit return
   };
   ```

In summary, use curly braces when you have multiple statements in the function body or when you need to explicitly return a value. If you have a single expression that you want to return, you can omit the braces for a more concise syntax.

remember when you have only one **expression** not **statement**, you're allowed to omit the `{}` and `return` keyword, when you have only one **expression**, you can use `{}` and `return` keyword but whenever you use `{}`, you have to use `return` keyword, even it's just one expression and you used `{}` arbitrarily.
if you have even only one statement you have to use `{}`.

`return` keyword is not mandatory in all of the situations but if you don't use it, what you are going to return? 

so using `{}` is based on number of expression not number of lines, you may have one expression which is typed in multiple lines, that's where you don't need `{}` for instance:

```jsx
import { useState } from "react";
import hello from "./Test.module.css";
import { FaAllergies } from "react-icons/fa";
import { Bs8Circle } from "react-icons/bs";
import { produce } from "immer";

function Test() {
  const [person, setPerson] = useState({
    firstName: "lome",
    age: 24,
    address: {
      street: "22 bakers",
      plateNumber: 18,
    },
  });

  let [arr, setArr] = useState([
    { id: 1, bug: "crash", fixed: false },
    { id: 2, bug: "crash", fixed: false },
  ]);

  let [count, setCount] = useState(0);

  return (
    <>
      {arr.map((ind) =>
   <p key={ind.id}>
            {ind.bug}
            {ind.fixed ? "fixed" : "sicktir"}
          </p>
        )}
        
        {/*in here `p` tag and inner body is just an expression, so we didin't use {} despite of being multiple lines for this single expression*/} 

      <button
        onClick={() => {
          setArr(
            produce((draft) => {
              const finder = draft.find((bug) => bug.id === 1);

              if (finder) {
                finder.fixed = true;
              }
            })
          );
        }}
      >
        clickert
      </button>
    </>
  );
}

export default Test;
```


In arrow functions, you can omit the curly braces `{}` only when you have a single expression, not just a single statement. Here's the distinction:

1. **Single Expression**:
   - If the arrow function consists of a single expression, you can omit the curly braces, and the result of that expression will be returned implicitly.
   ```javascript
   const add = (a, b) => a + b; // Implicit return of the expression
   ```

2. **Single Statement**:
   - If you have a single statement (which may include a block of code), you must use curly braces. In this case, you also need to use the `return` statement if you want to return a value.
   ```javascript
   const add = (a, b) => {
       const sum = a + b; // This is a statement
       return sum; // Explicit return
   };
   ```

In summary, you can omit the curly braces only for single expressions. If you have a single statement (even if it's just one line of code), you need to use curly braces and include a `return` statement if you want to return a value.

# 21. Substring in JavaScript

The **`substring()`** method of `String` values returns the part of this string from the start index up to and excluding the end index, or to the end of the string if no end index is supplied.

```javascript
const str = "Mozilla";

console.log(str.substring(1, 3));
// Expected output: "oz"

console.log(str.substring(2));
// Expected output: "zilla"

```

`substring()` extracts characters from `indexStart` up to _but not including_ `indexEnd`. In particular:

- If `indexEnd` is omitted or `undefined`, `substring()` extracts characters to the end of the string.
- If `indexStart` is equal to `indexEnd`, `substring()` returns an empty string.
- If `indexStart` is greater than `indexEnd`, then the effect of `substring()` is as if the two arguments were swapped; see example below.

Any argument value that is less than `0` or greater than `str.length` is treated as if it were `0` and `str.length`, respectively.

Any argument value that is `NaN` is treated as if it were `0`.

```javascript
const anyString = "Mozilla";

console.log(anyString.substring(0, 1)); // "M"
console.log(anyString.substring(1, 0)); // "M"

console.log(anyString.substring(0, 6)); // "Mozill"

console.log(anyString.substring(4)); // "lla"
console.log(anyString.substring(4, 7)); // "lla"
console.log(anyString.substring(7, 4)); // "lla"

console.log(anyString.substring(0, 7)); // "Mozilla"
console.log(anyString.substring(0, 10)); // "Mozilla"
```



