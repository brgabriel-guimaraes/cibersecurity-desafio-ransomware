### Descrição do Projeto: **Simulador de Ransomware em Python**

Este projeto é uma demonstração prática e controlada do funcionamento básico de um ransomware. Desenvolvido com fins educacionais, o simulador criptografa e descriptografa arquivos `.txt` utilizando a linguagem **Python** e a biblioteca **pyaes**. A ideia é mostrar como um ransomware opera em ambiente seguro, aumentando a conscientização sobre a importância da cibersegurança.

---

#### **Como funciona**
O projeto é composto por dois scripts: **encrypter** e **decrypter**, cada um com funções específicas no ciclo de um ransomware.

##### 1. **Encrypter (Criptografia do Arquivo)**
Este script simula o ataque inicial de um ransomware:
- **Entrada**: Seleciona um arquivo `.txt` para ser criptografado.
- **Processo**:
  - Lê o conteúdo do arquivo em modo binário.
  - Remove o arquivo original para simular o comportamento de exclusão dos dados.
  - Utiliza a chave `testeransomwares` e a biblioteca **pyaes** para criptografar o conteúdo.
- **Saída**: Cria um novo arquivo com extensão `.ransomwaretroll`, contendo os dados criptografados.

##### 2. **Decrypter (Descriptografia do Arquivo)**
Este script simula a recuperação dos dados mediante a chave correta:
- **Entrada**: Lê o arquivo criptografado com a extensão `.ransomwaretroll`.
- **Processo**:
  - Usa a mesma chave de criptografia para reverter o processo e descriptografar os dados.
  - Remove o arquivo criptografado.
- **Saída**: Restaura o arquivo original com o nome e conteúdo intactos.

---

#### **Tecnologias Utilizadas**
- **Python**: Para a implementação do script.
- **Biblioteca `os`**: Manipulação do sistema de arquivos, incluindo remoção de arquivos.
- **Biblioteca `pyaes`**: Aplicação do algoritmo AES (Advanced Encryption Standard) para criptografia e descriptografia.

---

#### **Destaques Técnicos**
- **Simulação de exclusão**: O arquivo original é apagado após a criptografia, replicando o comportamento real de ransomwares.
- **Criptografia AES**: Um dos algoritmos mais utilizados em segurança da informação para proteger dados.
- **Recuperação com chave correta**: Demonstra a dependência de uma chave válida para recuperar os dados, enfatizando a segurança do processo.


---

#### **Aviso Importante**
Este projeto é exclusivamente para fins **educacionais** e **éticos**. Ele **não deve ser utilizado para atividades maliciosas** ou ilegais. A responsabilidade pelo uso correto do código é do usuário.
