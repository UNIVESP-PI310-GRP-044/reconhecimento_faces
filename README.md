# reconhecimento_faces
Aqui está o módulo que realiza o reconhecimento de faces para a plataforma.

# Instalação do pacote [deepface](https://github.com/serengil/deepface):

Abra o Anaconda Prompt, ative o ambiente do PI com o seguinte comando:
```
conda activate pi
```

Agora instale o pacote deepface com o seguinte comando:

```
pip install git+https://github.com/serengil/deepface.git
```

# Preparação dos arquivos com as fotos

Você precisa pegar os arquivos das fotos que estão no OneDrive e colocar no diretório `database`, cada pessoa tem uma pasta e cada pasta pode conter várias fotos.

O resultado da detecção é o nome da pasta da pessoa. Depois podemos trocar a convensão e ao invés de usar Nome usar a Matrícula e assim conseguimos fazer a ligação com os dados no banco.

```
└── reconhecimento_faces/
    ├── app.py
    ├── database/
       ├── [nome 1]
           ├── Foto-1.jpg
           ├── ...
           └── Foto-n.jpg
       ├── [nome ...]
           ├── Foto-1.jpg
           ├── ...
           └── Foto-n.jpg
       ├── [nome n]
           ├── Foto-1.jpg
           ├── ...
           └── Foto-n.jpg
```

# Execução do aplicativo

Por hora o aplicativo "só" mostra o nome da pessoa que foi reconhecida, integrar com o restante do webapp é uma questão de convensão e criar o código.

Para abrir o app execute:

```
python app.py
```
