# Soal
Carilah solusi dua persamaan berikut

1. 3 + x^3 - x = 4
2. 2x - 4 = 8

# Solusi
1. Untuk mencari solusi persamaan non-linear 3 + x^3 - x = 4 dapat menggunakan metode numerik seperti metode Newton-Raphson.
Berikut implementasi dalam Phyton untuk mencari persamaan ini:

def fungsi(x):
def f(x):
    return 3 + x**3 - x - 4

def f_prime(x):
    return 3*x**2 - 1

def newton_raphson(initial_guess, tolerance=1e-6, max_iterations=100):
    x = initial_guess
    for i in range(max_iterations):
        x_next = x - f(x) / f_prime(x)
        if abs(x_next - x) < tolerance:
            return x_next
        x = x_next
    return None  # Return None if the method doesn't converge within the specified iterations

a. Menggunakan metode Newton-Raphson dengan tebakan awal x=1
result = newton_raphson(initial_guess=1)

if result is not None:
    print(f"Solusi persamaan adalah x = {result}")
else:
    print("Metode tidak konvergen dalam iterasi maksimum yang ditentukan.")
b. Menggunakan metode Newton-Raphson dengan tebakan awal x=1
result = newton_raphson(initial_guess=1)

if result is not None:
    print(f"Solusi persamaan adalah x = {result}")
else:
    print("Metode tidak konvergen dalam iterasi maksimum yang ditentukan.")
    
Output:

Solusi persamaan adalah x = 1.3247179572447898

2. Persamaan linear 2x − 4 = 8 dapat dipecahkan dengan mudah tanpa memerlukan metode numerik seperti Newton-Raphson.
Berikut implementasi dalam Python untuk mencari persamaan ini:
# Definisikan persamaan linear
def persamaan_linear(x):
    return 2*x - 4

# Tentukan nilai sebelah kanan persamaan
sebelah_kanan = 8

# Hitung nilai x
x = (sebelah_kanan + 4) / 2

# Cetak solusi
print("Solusi persamaan: x =", x)

Output:
Solusi persamaan: x = 6.0
