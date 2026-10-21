# Lab_numpy.py
import numpy as np

tableau_1d = np.array([1, 2, 3, 4, 5])
print("Tableau 1D :", tableau_1d)

tableau_2d = np.array([[1, 2, 3], [4, 5, 6]])
print("Tableau 2D :\n", tableau_2d)

zeros = np.zeros((2, 3))
print("Zeros :\n", zeros)

ones = np.ones((3, 2))
print("Ones :\n", ones)

progression = np.arange(0, 10, 2)
print("np.arange :", progression)

linspace = np.linspace(0, 1, 5)
print("np.linspace :", linspace)

print("dtype :", tableau_1d.dtype)
print("ndim :", tableau_1d.ndim)
print("shape :", tableau_1d.shape)
print("size :", tableau_1d.size)

vecteur = np.arange(1, 10)
print("Vecteur :", vecteur)

matrice = vecteur.reshape((3, 3))
print("Matrice 3x3 :\n", matrice)
print("Shape :", matrice.shape)
print("Size :", matrice.size)

matrice_auto = vecteur.reshape((3, -1))
print("Shape auto :", matrice_auto.shape)

tab_float = np.array([1, 2, 3], dtype=np.float32)
tab_int = tab_float.astype(np.int32)
print("Bytes float:", tab_float.nbytes, "Bytes int:", tab_int.nbytes)

mat_id = np.eye(4)
print("Identite :\n", mat_id)

mat_const = np.full((2, 2), 7)
print("Constante :\n", mat_const)

print("Matrice * 10 :\n", matrice * 10)
print("Racine carree :", np.sqrt(vecteur))
