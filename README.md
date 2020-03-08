# Leiva, the definitive low-level programming language
## Download & Installation
There are not actual releases, since this language is a prototype. 
## Compilation

#### If you want to interpret your code use:
```
leiva main.lei
```

#### If you want to compile and create an executable of your code use:
```
leivac main.lei -o
```

## Examples
#### Hello World:
```julia
println("Hello World!!!")
```
#### Fibbonacci numbers:
```julia
fn fibb(n)
  if n == 0 or n == 1
    return 1
  else 
    return fibb(n - 1) + fibb(n - 2)

fn main()
  for i in range 10
    if i == 10 print(fibb(i)) else print(fibb(i) + ", ")


```

#### Object Oriented:
```julia
struct OwnArray<T>
  priv data: []T
  
  pub constr(data: []T)
    self.data = data
  
  pub constr(seq: Seq<T>)
    self.data = []seq // Transforms from 'Seq<T>' to 'Array<T>'
    
  pub size()
    return data.size()
    
  pub operator self()
    return self.data
    
    
fn main()
  a = OwnArray<i32>([1, 2, 3]) // 1st constructor
  b = OwnArray<i32>(1, 2, 3) // 2nd constructor
  
  println(a + ", " + b)
  
```
```
[1, 2, 3], [1, 2, 3]
```
A hipotetical new programming language. Syntax and functions are prototypes.
