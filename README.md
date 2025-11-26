# JavaScript
function fibonacciSequence(n) {
  let fib = [0, 1]; // Initialize with the first two Fibonacci numbers

  // Handle cases where n is 0 or 1
  if (n === 0) {
    return [];
  } else if (n === 1) {
    return [0];
  }

  for (let i = 2; i < n; i++) {
    fib[i] = fib[i - 1] + fib[i - 2];
  }
  return fib;
}

console.log(fibonacciSequence(10)); // Output: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
