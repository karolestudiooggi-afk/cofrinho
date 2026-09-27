# 🫙 Cofrinho
 
App para criar metas e registrar cada valor guardado.
 
- Cada meta vira um pote que enche conforme você guarda dinheiro
- Registro de depósitos e retiradas com data, origem e anotação
- Cálculo de quanto guardar por mês/semana para bater a meta no prazo
- Backup e restauração em arquivo `.json`
## Dados e segurança
Login com e-mail e senha (Supabase Auth). Metas e registros ficam nas tabelas
`goals` e `entries` do Supabase, com Row Level Security: cada usuário só lê e altera os próprios dados.
A chave no `index.html` é a chave pública (anon), feita para ficar no navegador.
Nunca coloque a chave secret/service_role neste repositório.