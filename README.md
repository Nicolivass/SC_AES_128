# SC_AES_128

## Intro

Este relatório descreve a implementação da cifra de bloco AES e o modo de operação CTR (contador), tendo três partes: implementação da cifra, do modo de operação e teste. O padrão de criptografia avançada - advanced encryption standard (AES), é uma especificação para a criptografia de dados eletrônicos um subconjunto da cifra de bloco.  O algoritmo descrito pelo AES é um algoritmo de chave simétrica, o que significa que a mesma chave é usada para criptografar e descriptografar os dados. 


#### Encrypting

```bash
$ python AES.py -e -in text.txt -out text.enc -k 2b7e151628aed2a6abf7158809cf4f3c -iv 00112233445566778899aabbccddeeff -v
```

#### Decrypting

```bash
$ python AES.py -d -in text.enc -out text.txt -k 2b7e151628aed2a6abf7158809cf4f3c -iv 00112233445566778899aabbccddeeff -v
```
## Usage

```bash
usage: AES.py [-h] -in INPUT_FILE -out OUTPUT_FILE [-e] [-d] -k KEY [-iv IV] [-r ROUNDS] [-m {ECB,CTR}] [-v]

options:
  -h, --help show this help message and exit
  -in INPUT_FILE, --input_file INPUT_FILE
  -out OUTPUT_FILE, --output_file OUTPUT_FILE
  -e, --encrypt
  -d, --decrypt
  -k KEY, --key KEY
  -iv IV
  -r ROUNDS, --rounds ROUNDS
  -m {ECB,CTR}, --mode {ECB,CTR}
  -v, --verbose
```