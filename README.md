# Azure_Webapp
# API CRUD com .NET 7 e Banco Oracle

## Descrição do Projeto
Este projeto consiste em uma API desenvolvida em .NET 7 para realizar operações CRUD (Criar, Ler, Atualizar e Excluir) em um banco de dados Oracle. A API está hospedada como um WebApp no Azure, enquanto o banco de dados reside em uma máquina virtual configurada para acesso remoto. 

A solução é projetada para ser robusta, escalável e fácil de gerenciar, permitindo o gerenciamento eficiente de dados e suporte a integrações futuras.

---

## Benefícios para o Negócio

### **1. Melhoria na Eficiência Operacional**
- **Automação de Processos**: A API elimina tarefas manuais relacionadas ao gerenciamento de dados, reduzindo erros e economizando tempo.
- **Velocidade e Precisão**: Operações CRUD centralizadas e otimizadas aumentam a confiabilidade do sistema.

### **2. Escalabilidade**
- Hospedada no Azure, a API suporta o aumento na carga de usuários e dados conforme o negócio cresce, sem impacto significativo na performance.

### **3. Redução de Custos**
- **Infraestrutura Moderna**: O uso do Azure para hospedagem reduz custos de manutenção de servidores locais.
- **Eficiência Operacional**: Processos rápidos e automatizados economizam recursos de TI e suporte.

### **4. Integração com o Ecossistema Atual**
- **Interoperabilidade**: A solução permite fácil integração com sistemas legados e futuros através de padrões de APIs RESTful.

### **5. Segurança e Conformidade**
- Com o banco de dados Oracle configurado em uma VM protegida, os dados permanecem seguros e em conformidade com regulamentações, como LGPD.


FOTO DA SOLUÇÃO.
![image](https://github.com/user-attachments/assets/b252812c-5e5f-4108-b0ae-db8e7bfa0490)



---

## Requisitos do Ambiente

### Ferramentas Necessárias
1. **Visual Studio Code**
   - Extensões recomendadas:
     - C# (Microsoft)
     - Azure Tools
     - Oracle Developer Tools (se necessário)
2. **.NET 7 SDK**: Necessário para compilar, executar e testar a API localmente.
3. **Sistema Operacional**: Windows (recomendado).
4. **Conexão com a Internet**: Para acessar o Azure e a máquina virtual com o banco de dados.

---

## Estrutura do Projeto

- **/Controllers**: Contém os endpoints da API.
- **/Models**: Define as classes de modelo que representam as tabelas do banco de dados.
- **/Services**: Implementa a lógica de negócio para operações CRUD.
- **/Configurations**: Inclui configurações para o banco de dados e integração com o Azure.

---

## Configuração e Deploy

### 1. Clone o Repositório
```bash
https://github.com/VitorOnofreRamos/Challenge_Odontoprev_API.git
```

### 2. Configure as Dependências
- Certifique-se de que o .NET 7 SDK está instalado.
- Configure a string de conexão com o banco Oracle no `appsettings.json`:
  ```json
  {
    "ConnectionStrings": {
      "OracleDb": "<STRING_DE_CONEXAO>"
    }
  }
  ```

### 3. Publicação no Azure
- Utilize as ferramentas do Azure para publicar o projeto como um WebApp.
- Configure a conexão com o banco de dados na VM pelo painel de administração do Azure.

  ### ADD AS SEGUINTES DEPENDECIAS.
  ASPNETCORE_ENVIRONMENT	Development
  DOTNET_USE_POLLING_FILE_WATCHER	1
  WEBSITE_NODE_DEFAULT_VERSION	~18


### EXEMPLO DE ADD NO SWAGGER

{
  "nome": "felipe",
  "data_Nascimento": "2000-03-20T23:56:13.725Z",
  "cpf": "524.388.298-89",
  "endereco": "rua ",
  "telefone": "(11) 96315-1706",
  "carteirinha": 50509
}




### 4. Teste
- Use o Swagger UI para testar os endpoints da API.

---



---

**LINK DO VIDEO**

https://youtu.be/XCXg6H7XyDg
