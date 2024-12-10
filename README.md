
# Nitro Downloader 2024

## Sobre
Este script foi desenvolvido para baixar arquivos `.nitro` baseados nos dados obtidos de um arquivo JSON hospedado em uma URL. Ele cria automaticamente as pastas necessárias e organiza os arquivos baixados em um diretório especificado.

Produzido por: **Victor**  
Versão: **2024**

---

## Funcionalidades
- Baixa um arquivo JSON a partir de uma URL fornecida.
- Extrai informações do JSON para buscar arquivos `.nitro` online.
- Salva os arquivos `.nitro` em um diretório especificado.
- Gera mensagens de erro amigáveis para arquivos não encontrados ou problemas de conexão.

---

## Pré-requisitos
- **Python 3.6+**
- Bibliotecas Python:
  - `requests`
  - `json`
  - `configparser`
  - `os`
  - `pathlib`

Para instalar as dependências, use:
```bash
pip install requests
```

---

## Configuração
Antes de executar o script, crie um arquivo chamado `config.ini` na mesma pasta do script. O arquivo deve conter o seguinte formato:

```ini
[Settings]
JsonUrl = https://url-do-json.com/exemplo.json
FolderPath = caminho/para/salvar/arquivos
BaseUrl = https://url-base-dos-arquivos.com/
```

### Parâmetros
- **`JsonUrl`**: URL de onde será baixado o arquivo JSON.
- **`FolderPath`**: Diretório local onde os arquivos `.nitro` serão salvos.
- **`BaseUrl`**: URL base para buscar os arquivos `.nitro`.

---

## Como Usar
1. Certifique-se de que o Python esteja instalado em sua máquina.
2. Configure o arquivo `config.ini` com as informações corretas.
3. Execute o script com o comando:
   ```bash
   python script.py
   ```

---

## Mensagens de Log
O script exibe mensagens no terminal indicando o progresso:
- **Arquivo JSON baixado com sucesso.**  
  Indica que o arquivo JSON foi baixado corretamente.  
- **Arquivo '.nitro' baixado com sucesso.**  
  Indica que o arquivo `.nitro` foi baixado e salvo corretamente.  
- **Arquivo não encontrado: (Erro 404)**  
  Indica que o arquivo `.nitro` não existe na URL fornecida.  
- **Erro ao baixar o arquivo:**  
  Mensagem detalhada sobre erros de conexão ou outros problemas.  

---

## Personalização
Você pode personalizar o script para atender às suas necessidades específicas, como:
- Alterar o formato ou local de salvamento dos arquivos.
- Adicionar tratamento para outros tipos de erros.

---

## Licença
Este projeto é de código aberto. Sinta-se à vontade para usar e modificar. Se redistribuir, mencione o autor original.

---

Aproveite o **Nitro Downloader 2024** e facilite o gerenciamento de seus arquivos `.nitro`!
