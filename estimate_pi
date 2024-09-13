import random


def get_random_sample():
   """Gets a random sample from the uniform distribution on the square with   
   centre (0,0) and side length 2."""
   a = random.uniform(-1, 1)
   b = random.uniform(-1, 1)
   return (a, b)


def estimate_pi(num_samples=100000):
   """The area of a circle with radius 1 centred as 0,0 is pi
   The area of a square with side length 2 is 4

   Hence, implement a method which estimates pi using n random samples"""
   inside_circle = 0
   total_samples = num_samples

   for _ in range(total_samples):
      x, y = get_random_sample()
      if x*x + y*y <= 1:
            inside_circle += 1

   pi_estimate = 4 * inside_circle / total_samples
   return pi_estimate

# Example usage
estimated_pi = estimate_pi()
print(f"Estimated value of pi: {estimated_pi}")
