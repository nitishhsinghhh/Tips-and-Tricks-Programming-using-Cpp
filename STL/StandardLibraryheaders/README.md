# C++ Standard Library headers
The C++ standard library encompasses a comprehensive set of components and functionalities, including support for language features, concepts, memory management, metaprogramming, utilities, strings, containers, algorithms, numerics, time, localization, input/output, regular expressions, and thread management. Each category offers specific tools and resources for various aspects of C++ programming.

- The concepts library in C++ provides components that allow programs to validate template arguments at compile time and perform function dispatch based on the properties of types.
- The diagnostics library in C++ offers a consistent framework for reporting errors within a program, including predefined exception classes.
- The memory management library in C++ offers components for managing memory, including smart pointers and scoped allocators (introduced in C++11).
- The metaprogramming library includes features for use in templates and during constant evaluation, such as type traits, integer sequence (introduced in C++14), and rational arithmetic.
- The general utilities library encompasses components utilized by other library elements, including a predefined storage allocator for dynamic storage management, as well as infrastructure components in C++ programs, such as tuples and function wrappers (introduced in C++11).
- The strings library offers support for manipulating text represented as homogeneous sequences of characters, including char, char8_t (introduced in C++20), char16_t, char32_t (introduced in C++11), wchar_t, and other character-like types.
- The containers, iterators, ranges (introduced in C++20), and algorithms libraries grant a C++ program access to a subset of the most commonly used algorithms and data structures.
- The numerics library offers numeric algorithms and complex number components that enhance support for numeric processing. The valarray component provides support for n-at-a-time processing, potentially implemented as parallel operations on platforms that support such processing. Additionally, the random number component offers facilities for generating pseudo-random numbers (introduced in C++11).
- The time library provides generally useful time utilities.
- The localization library offers extended internationalization support for text processing.
- The input/output library provides the iostream components, which serve as the primary mechanism for input and output in C++ programs. These components can be used with other elements of the library, particularly strings, locales, and iterators.
- The regular expressions library offers functionality for regular expression matching and searching.
- The thread support library provides components for creating and managing threads, including atomic operations, mutual exclusion, and inter-thread communication.

The interface of C++ standard library is defined by the following collection of headers.

| Category                | Header(s)                                                                                   | Description                                           |
|-------------------------|---------------------------------------------------------------------------------------------|-------------------------------------------------------|
| Concepts library        | `<concepts>` _(C++20)_                                                                       |  Fundamental library concepts                         |
| Coroutines library      | `<coroutine>` _(C++20)_                                                                       |   Coroutine support library                           |
| Utilities library       | `<any>` _(C++17)_                                                                           |      std::any class                                   |
|                         | `<bitset>`                                                                                 | std::bitset class template                             |
|                          | `<chrono>`  _(C++11)_                                                                               |  C++ time utilities                              |
|                          | `<compare>` _(C++20)_                                                                              | Three-way comparison operator support           |
|                          | `<csetjmp>`                                                                                | Macro (and function) that saves (and jumps) to an execution context |
|                          | `<csignal>`                                                                                | Functions and macro constants for signal management    |
|                          | `<cstdarg>`                                                                                | Handling of variable length argument lists             |
|                          | `<cstddef>`                                                                                | Standard macros and typedefs                           |
|                          | `<cstdlib>`                                                                                | General purpose utilities: program control, dynamic memory allocation, random numbers, sort and search |
|                          | `<ctime>`                                                                                  | C-style time/date utilities                            |
|                          | `<debugging>` _(C++26)_                                                                      | Debugging library                               |
|                          | `<expected>`  _(C++23)_                                                                      | std::expected class template                    |
|                          | `<functional>`                                                                             | Function objects, Function invocations, Bind operations and Reference wrappers |
|                          | `<initializer_list>` _(C++11)_ | std::initializer_list class template             |
|                          | `<optional>` _(C++17)_ | std::optional class template                    |
|                          | `<source_location>` _(C++20)_ | Supplies means to obtain source code location   |
|                          | `<tuple>`  _(C++11)_ | std::tuple class template                        |
|                          | `<type_traits>`  _(C++11)_                                                                          |  Compile-time type information                   |
|                          | `<typeindex>`    _(C++11) _                                                                         |  std::type_index                                 |
|                          | `<typeinfo>`                                                                               | Runtime type information utilities                     |
|                          | `<utility>`                                                                                | Various utility components                             |
|                          | `<variant>` _(C++17)_                                                                               |  std::variant class template                     |
|                          | `<version>`   _(C++20)_                                                                             | Supplies implementation-dependent library information |
| Dynamic memory management | `<memory>`                                                                                 | High-level memory management utilities                 |
|                          | `<memory_resource>`  _(C++17)_                                                                     |  Polymorphic allocators and memory resources     |
|                          | `<new>`                                                                                    | Low-level memory management utilities                   |
|                          | `<scoped_allocator>` _(C++11)_                                                                       |  Nested allocator class                          |
| Numeric limits           | `<cfloat>`                                                                                 | Limits of floating-point types                         |
|                          | `<cinttypes>`   _(C++11)_                                                                             | Formatting macros, intmax_t and uintmax_t math and conversions |
|                          | `<climits>`                                                                                | Limits of integral types                               |
|                          | `<cstdint>`      _(C++11)_                                                                            | Fixed-width integer types and limits of other types |
|                          | `<limits>`                                                                                 | Uniform way to query properties of arithmetic types     |
|                          | `<stdfloat>`     _(C++23)_                                                                            | Optional extended floating-point types          |
| Error handling           | `<cassert>`                                                                                | Conditionally compiled macro that compares its argument to zero |
|                          | `<cerrno>`                                                                                 | Macro containing the last error number                 |
|                          | `<exception>`                                                                              | Exception handling utilities                            |
|                          | `<stacktrace>`   _(C++23)_                                                                           | Stacktrace library                               |
|                          | `<stdexcept>`                                                                              | Standard exception objects                             |
|                          | `<system_error>`        _(C++11)_                                                                | Defines std::error_code, a platform-dependent error |
| Strings library         | `<cctype>`                                                                                 | Functions to determine the category of narrow characters |
|                         | `<charconv>` _(C++17)_                                                                               |  std::to_chars and std::from_chars             |
|                         | `<cstring>`                                                                                | Various narrow character string handling functions    |
|                         | `<cuchar>`  _(C++11)_                                                                               |  C-style Unicode character conversion functions |
|                         | `<cwchar>`                                                                                 | Various wide and multibyte string handling functions  |
|                         | `<cwctype>`                                                                                | Functions to determine the category of wide characters |
|                         | `<format>`     _(C++20)_                                                                            | Formatting library including std::format      |
|                         | `<string>`                                                                                 | std::basic_string class template                     |
|                         | `<string_view>`      _(C++17)_                                                                      | std::basic_string_view class template         |
| Containers library      | `<array>` _(C++11)_                                                                                 |  std::array container                          |
|                         | `<deque>`                                                                                  | std::deque container                                 |
|                         | `<flat_map>`  _(C++23)_                                                                             | std::flat_map and std::flat_multimap container adaptors |
|                         | `<flat_set>`             _(C++23)_                                                                    |  std::flat_set and std::flat_multiset container adaptors |
|                         | `<forward_list>`       _(C++11)_                                                                      | std::forward_list container                   |
|                         | `<list>`                                                                                   | std::list container                                  |
|                         | `<map>`                                                                                    | std::map and std::multimap associative containers    |
|                         | `<mdspan>`  _(C++23)_                                                                                 |  std::mdspan view                              |
|                         | `<queue>`                                                                                  | std::queue and std::priority_queue container adaptors |
|                         | `<set>`                                                                                    | std::set and std::multiset associative containers    |
|                         | `<span>` _(C++20)_                                                                                    |  std::span view                                |
|                         | `<stack>`                                                                                  | std::stack container adaptor                         |
|                         | `<unordered_map>` _(C++11)_                                                                            | std::unordered_map and std::unordered_multimap unordered associative containers |
|                         | `<unordered_set>`  _(C++11)_                                                                          | std::unordered_set and std::unordered_multiset unordered associative containers |
|                         | `<vector>`                                                                                 | std::vector container                                |
| Iterators library       | `<iterator>`  _(C++23)_                                                                               | Range iterators                                      |
| Ranges library          | `<generator>` _(C++20)_                                                                                |  std::generator class template                 |
|                         | `<ranges>`                                                                                 |  Range access, primitives, requirements, utilities and adaptors |
| Algorithms library      | `<algorithm>`                                                                              | Algorithms that operate on ranges                     |
|                         | `<execution>`   _(C++17)_                                                                             | Predefined execution policies for parallel versions of the algorithms |
| Numerics library        | `<bit>`     _(C++20)_                                                                                 | Bit manipulation functions                    |
|                         | `<cfenv>`    _(C++11)_                                                                                | Floating-point environment access functions   |
|                         | `<cmath>`                                                                                  | Common mathematics functions                         |
|                         | `<complex>`   _(C++26)_                                                                               | Complex number type                                  |
|                         | `<linalg>`     _(C++20)_                                                                              | Basic linear algebra algorithms               |
|                         | `<numbers>`                                                                                | Math constants                                |
|                         | `<numeric>`                                                                                | Numeric operations on values in ranges               |
|                         | `<random>`    _(C++11)_                                                                               | Random number generators and distributions    |
|                         | `<ratio>`            _(C++11)_                                                                        | Compile-time rational arithmetic              |
|                         | `<valarray>`                                                                               | Class for representing and |
| Localization library    | `<clocale>`                                                                                | C localization utilities                              |
|                         | `<codecvt>`     _(C++11) (deprecated in C++17)(removed in C++26)_                           | Unicode conversion facilities |
|                         | `<locale>`                                                                                 | Localization utilities                                |
|                         | `<text_encoding>`       _(C++26)_                                                                     |  Text encoding identifications                  |
| Input/output library    | `<cstdio>`                                                                                 | C-style input-output functions                        |
|                         | `<fstream>`                                                                                | std::basic_fstream, std::basic_ifstream, std::basic_ofstream class templates and several typedefs |
|                         | `<iomanip>`                                                                                | Helper functions to control the format of input and output |
|                         | `<ios>`                                                                                    | std::ios_base class, std::basic_ios class template and several typedefs |
|                         | `<iosfwd>`                                                                                 | Forward declarations of all classes in the input/output library |
|                         | `<iostream>`                                                                               | Several standard stream objects                       |
|                         | `<istream>`                                                                                | std::basic_istream class template and several typedefs |
|                         | `<ostream>`                                                                                | std::basic_ostream, std::basic_iostream class templates and several typedefs |
|                         | `<print>`            _(C++23)_                                                                        | Formatted output library including std::print  |
|                         | `<spanstream>`        _(C++23)_                                                                       | std::basic_spanstream, std::basic_ispanstream, std::basic_ospanstream class templates and typedefs |
|                         | `<sstream>`                                                                                | std::basic_stringstream, std::basic_istringstream, std::basic_ostringstream class templates and several typedefs |
|                         | `<streambuf>`                                                                              | std::basic_streambuf class template                   |
|                         | `<strstream>`                                                                              | (deprecated in C++98), std::strstream, std::istrstream, std::ostrstream |
|                         | `<syncstream>`  _(C++20)_                                                                             | std::basic_osyncstream, std::basic_syncbuf, and typedefs |
| Filesystem library      | `<filesystem>`         _(C++17)_                                                                      | std::path class and supporting functions       |
| Regular Expressions library | `<regex>`              _(C++11)_                                                                  | Classes, algorithms and iterators to support regular expression processing |
| Atomic Operations library | `<atomic>`                _(C++11)_                                                                | Atomic operations library                      |
| Thread support library  | `<barrier>`                      _(C++20)_                                                            | Barriers                                       |
|                         | `<condition_variable>`                _(C++11)_                                                       | Thread waiting conditions                      |
|                         | `<future>`                                      _(C++11)_                                             | Primitives for asynchronous computations       |
|                         | `<hazard_pointer>`                                         _(C++20)_                                 | Hazard pointers                                |
|                         | `<latch>`     _(C++20)_                                                                              |  Latches                                        |
|                         | `<mutex>`                                _(C++11)_                                                   |  Mutual exclusion primitives                    |
|                         | `<rcu>`                                  _(C++26)_                                                   |  Read-copy update mechanisms                    |
|                         | `<semaphore>`                            _(C++20)_                                                   |  Semaphores                                     |
|                         | `<shared_mutex>`                       _(C++14)_                                                   |  Shared mutual exclusion primitives             |
|                         | `<stop_token>`                           _(C++20)_                                                   |  Stop tokens for std::jthread                   |
|                         | `<thread>`                            _(C++11)_                                                   |  std::thread class and supporting functions     |


# C compatibility headers

The C compatibility headers are a set of headers that provide interoperability between C and C++. For many of the C standard library headers of the form xxx.h, the C++ standard library provides an identically-named header and another header of the form cxxx. The headers of the form xxx.h are intended for use when interoperability with C is needed. When not writing code that needs to be compatible with C, one should use the cxxx headers.

Here's a summary of the C compatibility headers and their descriptions:
| C Header       | Corresponding C++ Header | Description                                                                                   |
|----------------|--------------------------|-----------------------------------------------------------------------------------------------|
| `<assert.h>`   | `<cassert>`              | Behaves the same as `<cassert>`                                                               |
| `<ctype.h>`    | `<cctype>`               | Behaves as if each name from `<cctype>` is placed in the global namespace                    |
| `<errno.h>`    | `<cerrno>`               | Behaves the same as `<cerrno>`                                                                |
| `<fenv.h>`     | `<cfenv>`                | C++11, Behaves as if each name from `<cfenv>` is placed in the global namespace              |
| `<float.h>`    | `<cfloat>`               | Behaves the same as `<cfloat>`                                                                |
| `<inttypes.h>` | `<cinttypes>`            | C++11, Behaves as if each name from `<cinttypes>` is placed in the global namespace          |
| `<limits.h>`   | `<climits>`              | Behaves the same as `<climits>`                                                               |
| `<locale.h>`   | `<clocale>`              | Behaves as if each name from `<clocale>` is placed in the global namespace                   |
| `<math.h>`     | `<cmath>`                | Behaves as if each name from `<cmath>` is placed in the global namespace (except some names) |
| `<setjmp.h>`   | `<csetjmp>`              | Behaves as if each name from `<csetjmp>` is placed in the global namespace                   |
| `<signal.h>`   | `<csignal>`              | Behaves as if each name from `<csignal>` is placed in the global namespace                   |
| `<stdarg.h>`   | `<cstdarg>`              | Behaves as if each name from `<cstdarg>` is placed in the global namespace                   |
| `<stddef.h>`   | `<cstddef>`              | Behaves as if each name from `<cstddef>` is placed in the global namespace                   |
| `<stdint.h>`   | `<cstdint>`              | C++11, Behaves as if each name from `<cstdint>` is placed in the global namespace            |
| `<stdio.h>`    | `<cstdio>`               | Behaves as if each name from `<cstdio>` is placed in the global namespace                    |
| `<stdlib.h>`   | `<cstdlib>`              | Behaves as if each name from `<cstdlib>` is placed in the global namespace                   |
| `<string.h>`   | `<cstring>`              | Behaves as if each name from `<cstring>` is placed in the global namespace                   |
| `<time.h>`     | `<ctime>`                | Behaves as if each name from `<ctime>` is placed in the global namespace                     |
| `<uchar.h>`    | `<cuchar>`               | C++11, Behaves as if each name from `<cuchar>` is placed in the global namespace             |
| `<wchar.h>`    | `<cwchar>`               | Behaves as if each name from `<cwchar>` is placed in the global namespace                    |
| `<wctype.h>`   | `<cwctype>`              | Behaves as if each name from `<cwctype>` is placed in the global namespace                   |
## Special C compatibility headers
The header <stdatomic.h> declares names which are also provided in the C standard library, and defines the _Atomic macro which is a keyword in C. Unlike other xxx.h headers, corresponding <cstdatomic> is not provided.

| Category                      | Header(s)       | Description                                                                                         |
|-------------------------------|-----------------|-----------------------------------------------------------------------------------------------------|
| Special C Compatibility Header | `<stdatomic.h>` | C++23, Defines `_Atomic` and provides corresponding components in the C standard library             |

## Empty C headers
The headers <complex.h>, <ccomplex>, <tgmath.h>, and <ctgmath> do not contain any content from the C standard library and instead merely include other headers from the C++ standard library.
| Category        | Header(s)      | Description                                                                                     |
|-----------------|----------------|-------------------------------------------------------------------------------------------------|
| Empty C Headers | `<ccomplex>`   | C++11 (deprecated in C++17)(removed in C++20), Simply includes the header `<complex>`           |
|                 | `<complex.h>`  | C++11, Simply includes the header `<complex>`                                                   |
|                 | `<ctgmath>`    | C++11 (deprecated in C++17)(removed in C++20), Simply includes the headers `<complex>` and `<cmath>` |
|                 | `<tgmath.h>`   | C++11, Simply includes the headers `<complex>` and `<cmath>`                                    |

## Meaningless C headers
The headers <ciso646>, <cstdalign>, and <cstdbool> are meaningless in C++ because the macros they provide in C are language keywords in C++.
| Category                   | Header(s)       | Description                                                                                   |
|----------------------------|-----------------|-----------------------------------------------------------------------------------------------|
| Meaningless C Headers      | `<ciso646>`     | (removed in C++20), Empty header. The macros that appear in iso646.h in C are keywords in C++ |
|                            | `<cstdalign>`   | C++11 (deprecated in C++17)(removed in C++20), Defines one compatibility macro constant       |
|                            | `<cstdbool>`    | C++11 (deprecated in C++17)(removed in C++20), Defines one compatibility macro constant       |
| C Compatibility Headers    | `<iso646.h>`    | Has no effect                                                                                  |
|                            | `<stdalign.h>`  | C++11, Defines one compatibility macro constant                                                |
|                            | `<stdbool.h>`   | C++11, Defines one compatibility macro constant                                                |


## Unsupported C headers
The C headers <stdatomic.h>, (until C++23) <stdnoreturn.h>, and <threads.h> are not included in C++ and have no cxxx equivalents.
