# Fitness Buddy

A proposta do projeto é ser um assistente que acompanha sua saúde.


# Como?

Por questão de simplicidade, esta aplicação usa o localStorage do navegador para armazenar todos os dados - por isso não há login.
A vantagem é a simplicidade e a desvantagem é que, caso haja uma limpeza de cache, os dados serão perdidos.


# Como usar?

Acesse a URL [do projeto](https://wellintoncr.github.io/fitness-buddy) e pronto. Haverá builds novas a cada push em **main**.

Caso queira executar localmente: apesar de serem apenas arquivos estáticos, os navegadores podem considerar cada arquivo como um domínio, então não seria possível acessar o mesmo localStorage em todas as telas.
Para resolver isso, basta levantar um servidor local que sirva os dados. Com Python 3, basta:
```sh
cd este-projeto
python3 -m http.server
```

# Tarefas

- [x] [ *Bug* ] Ao selecionar a dificuldade do treino, apenas um treino está sendo selecionado por vez (ex. marco "Difícil" no treino A e, ao marcar "Fácil" no treino B, a dificuldade do treino A é perdida);

- [ ] [ *Melhoria* ] Visualizar histórico de treinos

- [ ] [ *Melhoria* ] Sugerir carga - indicar se o treino do dia deve manter ou aumentar a carga;

- [ ] [ *Melhoria* ] Editar e apagar treinos;

- [ ] [ *Melhoria* ] Exportar e importar dados - por se tratar de localStorage, seria interessante haver alguma forma de fazer e restaurar backups;

- [ ] [ *Melhoria* ] Ao cadastrar um treino, inserir as cargas disponíveis para que o assistente consiga sugerir a carga do dia;

- [ ] [ *Melhoria* ] Assistente de métricas corporais - registrar peso e medidas corporais;

- [ ] [ *Melhoria* ] Visualizar histórico de métricas corporais
