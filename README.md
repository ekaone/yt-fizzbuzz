Fizz buzz collection in programming languages

## JavaScript

```
function fizzBuzz(n) {
  for (let i = 1; i <= n; i++) {
    let output = '';

    if (i % 3 === 0) {
      output += 'Fizz';
    }

    if (i % 5 === 0) {
      output += 'Buzz';
    }

    console.log(output || i);
  }
}

// Example usage:
fizzBuzz(100); // Print Fizz, Buzz, or FizzBuzz for numbers 1 to 100
```

OR

```
function fizzBuzz(n) {
  for (let i = 1; i <= n; i++) {
    const output = (i % 3 === 0 ? 'Fizz' : '') + (i % 5 === 0 ? 'Buzz' : '');
    console.log(output || i);
  }
}

// Example usage:
fizzBuzz(100); // Print Fizz, Buzz, or FizzBuzz for numbers 1 to 100
```

## TypeScript

```
function fizzBuzz(n: number): void {
  for (let i = 1; i <= n; i++) {
    let output: string = '';

    if (i % 3 === 0) {
      output += 'Fizz';
    }

    if (i % 5 === 0) {
      output += 'Buzz';
    }

    console.log(output || i);
  }
}

// Example usage:
fizzBuzz(100); // Print Fizz, Buzz, or FizzBuzz for numbers 1 to 100

```

## Golang

```
package main

import "fmt"

func fizzBuzz(n int) {
    for i := 1; i <= n; i++ {
        output := ""

        if i%3 == 0 {
            output += "Fizz"
        }

        if i%5 == 0 {
            output += "Buzz"
        }

        if output == "" {
            fmt.Println(i)
        } else {
            fmt.Println(output)
        }
    }
}

func main() {
    fizzBuzz(100)
}

```

## C++

```
#include <iostream>

void fizzBuzz(int n) {
    for (int i = 1; i <= n; i++) {
        std::string output = "";

        if (i % 3 == 0) {
            output += "Fizz";
        }

        if (i % 5 == 0) {
            output += "Buzz";
        }

        if (output.empty()) {
            std::cout << i << std::endl;
        } else {
            std::cout << output << std::endl;
        }
    }
}

int main() {
    fizzBuzz(100);
    return 0;
}
```

## Python

```
def fizzBuzz(n):
    for i in range(1, n + 1):
        output = ""

        if i % 3 == 0:
            output += "Fizz"

        if i % 5 == 0:
            output += "Buzz"

        if not output:
            print(i)
        else:
            print(output)

# Example usage:
fizzBuzz(100)
```

## Rush

```
fn fizz_buzz(n: u32) {
    for i in 1..=n {
        let mut output = String::new();

        if i % 3 == 0 {
            output += "Fizz";
        }

        if i % 5 == 0 {
            output += "Buzz";
        }

        if output.is_empty() {
            println!("{}", i);
        } else {
            println!("{}", output);
        }
    }
}

fn main() {
    fizz_buzz(100);
}
```

## Java

```
public class FizzBuzz {
    public static void fizzBuzz(int n) {
        for (int i = 1; i <= n; i++) {
            String output = "";

            if (i % 3 == 0) {
                output += "Fizz";
            }

            if (i % 5 == 0) {
                output += "Buzz";
            }

            if (output.isEmpty()) {
                System.out.println(i);
            } else {
                System.out.println(output);
            }
        }
    }

    public static void main(String[] args) {
        fizzBuzz(100);
    }
}
```

## Ruby

```
def fizz_buzz(n)
  (1..n).each do |i|
    output = ''

    output += 'Fizz' if i % 3 == 0
    output += 'Buzz' if i % 5 == 0

    puts output.empty? ? i : output
  end
end

# Example usage:
fizz_buzz(100)
```

## Swift

```
func fizzBuzz(_ n: Int) {
    for i in 1...n {
        var output = ""
        
        if i % 3 == 0 {
            output += "Fizz"
        }
        
        if i % 5 == 0 {
            output += "Buzz"
        }
        
        if output.isEmpty {
            print(i)
        } else {
            print(output)
        }
    }
}

// Example usage:
fizzBuzz(100)
```

## Kotlin

```
fun fizzBuzz(n: Int) {
    for (i in 1..n) {
        var output = ""
        
        if (i % 3 == 0) {
            output += "Fizz"
        }
        
        if (i % 5 == 0) {
            output += "Buzz"
        }
        
        if (output.isEmpty()) {
            println(i)
        } else {
            println(output)
        }
    }
}

fun main() {
    fizzBuzz(100)
}
```

## PHP

```
<?php
function fizzBuzz($n) {
    for ($i = 1; $i <= $n; $i++) {
        $output = '';

        if ($i % 3 == 0) {
            $output .= 'Fizz';
        }

        if ($i % 5 == 0) {
            $output .= 'Buzz';
        }

        if (empty($output)) {
            echo $i . "\n";
        } else {
            echo $output . "\n";
        }
    }
}

// Example usage:
fizzBuzz(100);
?>
```

## Scala

```
object FizzBuzz {
  def fizzBuzz(n: Int): Unit = {
    for (i <- 1 to n) {
      var output = ""

      if (i % 3 == 0) {
        output += "Fizz"
      }

      if (i % 5 == 0) {
        output += "Buzz"
      }

      if (output.isEmpty) {
        println(i)
      } else {
        println(output)
      }
    }
  }

  def main(args: Array[String]): Unit = {
    fizzBuzz(100)
  }
}
```

## Lisp

```
(defun fizz-buzz (n)
  (dotimes (i n)
    (let ((output ""))
      (if (zerop (mod (1+ i) 3))
          (setf output (concatenate 'string output "Fizz")))
      (if (zerop (mod (1+ i) 5))
          (setf output (concatenate 'string output "Buzz")))
      (if (string= output "")
          (format t "~a~%" (1+ i))
          (format t "~a~%" output)))))

;; Example usage:
(fizz-buzz 100)
```

## Fortran

```
program fizzbuzz
  implicit none
  integer :: i
  do i = 1, 100
     if (mod(i, 3) == 0) then
        write(*, '(A)', advance='no') 'Fizz'
     end if
     if (mod(i, 5) == 0) then
        write(*, '(A)', advance='no') 'Buzz'
     end if
     if (mod(i, 3) /= 0 .and. mod(i, 5) /= 0) then
        write(*, '(I0)') i
     else
        write(*, *)
     end if
  end do
end program fizzbuzz
```

## Haskell

```
fizzBuzz :: Int -> IO ()
fizzBuzz n = mapM_ putStrLn [if | i `mod` 3 == 0 && i `mod` 5 == 0 -> "FizzBuzz"
                                | i `mod` 3 == 0 -> "Fizz"
                                | i `mod` 5 == 0 -> "Buzz"
                                | otherwise -> show i
                            | i <- [1..n]]

main :: IO ()
main = fizzBuzz 100

```

## Cobol

```
IDENTIFICATION DIVISION.
PROGRAM-ID. FizzBuzz.

DATA DIVISION.
WORKING-STORAGE SECTION.
01 I PIC 9(3) VALUE 1.

PROCEDURE DIVISION.
    PERFORM VARYING I FROM 1 BY 1 UNTIL I > 100
        DISPLAY ' '
        IF I MOD 3 = 0 THEN
            DISPLAY 'Fizz'
        END-IF
        IF I MOD 5 = 0 THEN
            DISPLAY 'Buzz'
        END-IF
        IF I MOD 3 <> 0 AND I MOD 5 <> 0 THEN
            DISPLAY I
        END-IF
    END-PERFORM.

    STOP RUN.
```

## Matlab

```
function fizzBuzz(n)
    for i = 1:n
        output = '';

        if mod(i, 3) == 0
            output = 'Fizz';
        end

        if mod(i, 5) == 0
            output = [output 'Buzz'];
        end

        if isempty(output)
            disp(i);
        else
            disp(output);
        end
    end
end

% Example usage:
fizzBuzz(100);
```

## Ada

```
with Ada.Text_IO;

procedure FizzBuzz is
   N : constant Integer := 100;
begin
   for I in 1..N loop
      declare
         Output : String(1..10);
      begin
         Output := "";

         if I mod 3 = 0 then
            Output := "Fizz";
         end if;

         if I mod 5 = 0 then
            Output := Output & "Buzz";
         end if;

         if Output = "" then
            Ada.Text_IO.Put(I);
         else
            Ada.Text_IO.Put_Line(Output);
         end if;
      end;
   end loop;
end FizzBuzz;
```

## C#

```
using System;

class Program
{
    static void Main()
    {
        FizzBuzz(100);
    }

    static void FizzBuzz(int n)
    {
        for (int i = 1; i <= n; i++)
        {
            string output = "";

            if (i % 3 == 0)
            {
                output += "Fizz";
            }

            if (i % 5 == 0)
            {
                output += "Buzz";
            }

            if (string.IsNullOrEmpty(output))
            {
                Console.WriteLine(i);
            }
            else
            {
                Console.WriteLine(output);
            }
        }
    }
}
```
