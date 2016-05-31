# Python Crypto Libraries Tutorial


Tutorial on how to use different crypto libraries in Python for
  [Network Security](http://www.ccs.neu.edu/home/amirali/teaching/Summer16/).

  **Instructor**: [Amirali Sanatinia](http://www.ccs.neu.edu/home/amirali)

  **Email**: amirali@ccs.neu.edu


## Requirements

 * Python 2.6+
 * [IPython Notebook](http://ipython.org/notebook.html)
 * [PyCrypto](https://www.dlitz.net/software/pycrypto/)
 * [cryptography](http://cryptography.io/)


## OpenSSL

To create *RSA* key pairs you can use the following commands:

```
$ openssl genrsa -out private_key.pem 2048
$ openssl pkcs8 -topk8 -inform PEM -outform DER -in private_key.pem -out private_key.der -nocrypt
$ openssl rsa -in private_key.pem -pubout -outform DER -out public_key.der
```
