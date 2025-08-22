# 📦 Instalação do Miniconda no Linux (Ubuntu/WSL)

Este guia explica como instalar e configurar o **Miniconda** no Linux, permitindo gerenciar ambientes virtuais com `conda`.

---

## 🔹 1. Baixar o instalador do Miniconda
No terminal:
```bash
cd ~/Downloads
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```

---

## 🔹 2. Executar o instalador
```bash
bash Miniconda3-latest-Linux-x86_64.sh
```

Durante a instalação:
- Aceite a licença → digite `yes`
- Confirme o local de instalação (padrão recomendado)
- Pergunte se deseja adicionar ao `.bashrc` → digite `yes`

---

## 🔹 3. Recarregar o terminal
```bash
source ~/.bashrc
```

Verifique se o Conda foi instalado corretamente:
```bash
conda --version
```

---

## 🔹 4. Criar e ativar um ambiente Conda
Crie um ambiente chamado `my_app` com Python 3.10:
```bash
conda create -n my_app python=3.10
```

Ative o ambiente:
```bash
conda activate my_app
```

Você verá o `(my_app)` no início do terminal, indicando que o ambiente está ativo.

---

✅ Agora você pode instalar pacotes dentro do ambiente com:
```bash
conda install numpy pandas matplotlib
```

E para sair do ambiente:
```bash
conda deactivate
```
