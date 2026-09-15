# -ai-astra_ph_star.-
def fibonacci(n, memo={}):     if n in memo:         return memo[n]     if n &lt;= 1:         memo[n] = n     else:         memo[n] = fibonacci(n-1, memo) + fibonacci(n-2, memo)     return memo[n]  def fibonacci_iter(n):     if n &lt;= 1:         return n     a, b = 0, 1     for _ in range(2, n+1):         a, b = b, a + b     return b
