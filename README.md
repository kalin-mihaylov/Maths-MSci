# Maths-MSci
My project repository. Includes Python code for:

1). CUDA Euler-Maruyama constant time-step integration of an Overdamped Langevin System <br />
2). CPU Autocorrelation Function plotting given (M,N)-shape trajectory data (np -> cp for GPU) <br /> 
2+1). CUDA + CPU full implementation of ACF plot for given Overdamped Langevin system potential <br />
    * This is not an ideal piece of code - the better way of handling the X-data would be to keep it on the device and run the ACF code with CuPy FFT, but this is not currently feasible for me because the two libraries are incompatible. You cannot easily convert between Numba and CuPy arrays and there seems to be some C-level magic including memory pointers that allows you to convert, but that eludes me.
