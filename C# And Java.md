|           | C#                                                           | Java                                                        |
| --------- | ------------------------------------------------------------ | ----------------------------------------------------------- |
| Function  | `Func<int, int> square = x => x * x;`                        | `Function<Integer, Integer> square = x -> x * x;`           |
|           | `square(5);`                                                 | `square.apply(5);`                                          |
|           |                                                              |                                                             |
| Predicate | `var cheapBooks = books.findAll(b => b.Price < 10);`         | `var cheapBooks = books.steam().filter(b -> b.Price < 10);` |
| Delegates | `public delegate void MyDelegate();`                         | `@FunctionalInterface`                                      |
|           | `MyDelegate variable = () => Console.Write("First delegate");` | `public interface MyInterface {`                            |
|           | `variable += () => Console.Write("Another delegate");`       | ` void invoke();`                                           |
|           | `variable();`                                                | `}`                                                         |
|           |                                                              | `MyInterface mi = () -> System.out.print("Hello");`         |
|           |                                                              | `mi.invoke();`                                              |
|           | In C# Delegate can be one or more lambdas(functions)         |                                                             |

