# CatologoJogos
Backend de um catálogo de jogos desenvolvido em C# e .NET durante o Take Blip Fullstack Developer.

---
## Formas de armazenamento dos dados
### SQL Server
A aplicação está confugurada para utilizar o SQL Server, no entanto, é necessário iserir a string de conexão no arquivo appsettings.json, no Default. Para simplificar, insira a seguinte string:

- Data Source=NOME_DO_SEU_COMPUTADOR\\SQLEXPRESS;Initial Catalog=CatalogoJogos;Integrated Security=True;Connect Timeout=30

Basta substituir NOME_DO_SEU_COMPUTADOR para realizar um uso de um servidor local.

Caso utilize o banco de dados, não se esqueaça de criar o database e a tabela no servidor antes de inicializar a aplicação. Para isso, está disponíve os dois códigos SQL criadores, sendo eles o DataBaseCreation.sql e TableCreation.sql, respectivamente.

### Memória local
Também há uma versão local, já com cinco jogos cadastrados, para caso não possua o SQL Server ou não deseje usar esse banco de dados. Para tanto, descomente a linha 36 e comente a 37 do arquivo Atartup.cs.
